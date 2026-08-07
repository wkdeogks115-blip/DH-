# C0033 Apply value helper patch

## Before — C0032 defect

```js
const field = form.elements.namedItem(name);
return field && typeof field.value === "string" ? field.value.trim() : "";
```

For a single checkbox, `.value` remains `confirmed` even when `.checked === false`.

## After — C0033

```js
const field = form.elements.namedItem(name);
if (field instanceof HTMLInputElement && (field.type === "checkbox" || field.type === "radio")) {
  return field.checked ? field.value.trim() : "";
}
return field && typeof field.value === "string" ? field.value.trim() : "";
```

## Runtime acceptance

- unchecked `safety_ack` + `scope_ack` must produce exactly two acknowledgement errors once all other required data is valid;
- checking only `safety_ack` leaves only `scope_ack`;
- checking both allows summary generation;
- prior values must be preserved after blocked submission.

Parent defect and candidate behavior are recorded under `audits/`.

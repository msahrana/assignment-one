In TypeScript, any is called a “type safety hole” because it disables all type checks, letting bugs slip into runtime. On the other hand, unknown forces you to validate data using type narrowing.

Examples:
function handle(value: unknown) {
if (typeof value === "number") {
console.log(value.toFixed(2));
}
}

N.B: Type narrowing refines unknown into specific types, preserving reliability and preventing runtime errors.

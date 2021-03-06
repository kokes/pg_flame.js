# pg_flame.js - postgres plan flame graphs

Paste your execution plan, get a flame graph out. This project is heavily inspired by [pg_flame](https://github.com/mgartner/pg_flame), the one big difference is that we don't do any server side data manipulation, everything happens on the client.

[**Try a live demo**](https://kokes.github.io/pg_flame.js/index.html)

There are still quite a few rough edges. These will eventually morph into issues:

- we might not be parsing InitPlan nodes correctly
- we don't support cost-based plans, only those with explicit timing (`EXPLAIN ANALYZE`)
- there are some rounding issues (you can see it in the example)
- any errors are emitted in the console, not in the UI

Contributions welcome.

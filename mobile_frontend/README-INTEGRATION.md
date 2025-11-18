# Mobile Frontend Integration Notes

- Base API URL:
  - Configure via `.env` at project root of mobile_frontend.
  - Key: `API_BASE_URL` (default fallback http://localhost:3001)
  - Example: see `.env.example`.

- Navigation:
  - Bottom navigation with three tabs: Dashboard, Transactions, Budgets.

- Providers/Services:
  - Uses Provider for state management.
  - ApiClient centralizes REST calls (http).
  - Services:
    - TransactionService: /transactions CRUD
    - BudgetService: /budgets CRUD
    - DashboardService: /dashboard/categories for category summaries

- Forms:
  - Transactions: add/edit with type, amount, category, description, date.
  - Budgets: add/edit with category, limitAmount, month (YYYY-MM).

- Run:
  - `flutter pub get`
  - `flutter run`

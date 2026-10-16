# Zenmoney MCP

**Connect your financial data to AI for insights, forecasts, and smarter ways to spend and save.**

Zenmoney gives your AI assistant access to financial data from the accounts you track in Zenmoney. Ask about your transactions, explore spending patterns, find recurring charges, estimate future cash flow, and discover ways to spend or save more efficiently.

The connector gives your assistant access to data stored in Zenmoney. It can analyze your records and, when you ask, add, edit, or delete transactions and manage accounts and categories. It cannot move money or make payments.

## Connect to Claude

To use the connector, you need a [Zenmoney account](https://zenmoney.app/) with an **active subscription**. Connect your banks or add transactions in Zenmoney first.

1. Open **Customize → Connectors** and search for **Zenmoney** in the connector directory.
2. Select Zenmoney and click **Connect**.
3. Sign in to Zenmoney and approve access.
4. Enable Zenmoney in your chat under **+ → Connectors**.

Try: “Show my current Zenmoney account balances.”

## Example requests

- “Where did my money go last month?”
- “Find my subscriptions and flag any price increases.”
- “Compare my spending by category over the last six months.”
- “Find possible duplicate transactions.”
- “What payments do I have planned for the next two weeks?”
- “Estimate how much I’ll have left at the end of the month.”
- “Where could I realistically save more?”

## Data and access

The assistant can read your accounts, balances, transactions, categories, merchants, budgets, planned payments, and exchange rates, and search Zenmoney help. When you ask, it can also add, edit, or delete transactions and create or edit accounts, categories, and merchants.

It works with the records in your current Zenmoney space, including records shared with family members. It cannot move money, make payments, or connect and sync banks, so the data is only as current as your last bank sync.

Your financial data is sent to your chosen AI provider for processing under that provider’s terms and privacy settings. Access uses OAuth, so never paste passwords or access tokens into chat.

### Read tools

- `get_user` — main currency, month start day, and planning settings.
- `list_accounts` — all accounts, including archived and debt accounts, with current balances.
- `get_account_balances` — account balances at the start or end of specific dates.
- `list_categories` — categories and tags.
- `list_transactions` — transactions for a date range, filtered by account, category, tag, merchant, comment, or amount.
- `list_scheduled_transactions` — planned and processed scheduled operations.
- `get_monthly_report` — monthly income and spending by category, transfers, budgets, and plan vs. actual for up to 24 months.
- `get_instrument_rates` — exchange rates for specific dates.
- `search_merchants` — your saved counterparties and public brands.
- `search_financial_institutions` — banks, brokers, and payment services.
- `search_help` — Zenmoney help materials and support answers about app features and settings.

### Write tools

Write tools change your Zenmoney records and are meant to be used only when you ask for a change.

- `upsert_transactions` — add or edit transactions, transfers, and debts.
- `delete_transactions` — delete selected transactions. Deleted transactions can’t be restored through the connector.
- `upsert_accounts` — create, edit, or archive accounts.
- `upsert_categories` — create, edit, or archive categories.
- `create_merchant` — add a new counterparty.

## Disconnect

In Claude, open Zenmoney under **Connectors** and disconnect or remove it. This stops future access but does not delete data already shared in your chats.

To revoke all existing Zenmoney authorizations, change your Zenmoney password.

## Help and privacy

- **Connection error?** Try to reconnect.
- **Missing transactions?** Check bank sync in Zenmoney.
- **Large request failing?** Try requesting a shorter period.

[Contact support](mailto:support@zenmoney.app) with the error details and the name of your AI client. Do not send passwords, access tokens, or unredacted screenshots containing financial data.

[Privacy Policy](https://zenmoney.app/legal/privacy/)

Last updated: October 7, 2026.

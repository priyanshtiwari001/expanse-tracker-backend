## Backend 
📦 Core Features
✅ 1. User Authentication
Sign-up/Login (JWT)
Session caching in Redis (e.g., for quick auth checks)
💸 2. Add/View Expenses
Add expense: category, amount, date, note
View expenses list (filter by date range, category)
Store in MongoDB
<hr/>
 2. Monthly Summary (Redis Cache)
Calculate monthly totals per category
Store in Redis for fast retrieval
Invalidate/update cache on new expense or deletion
<hr/>
3. Email Summary (RabbitMQ)
Queue email job weekly or on button click
Worker pulls from queue, compiles summary, sends email
Store logs/status in Redis (optional)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dynamic Expense Tracker</title>
    <style>
        :root { --primary: #2563eb; --secondary: #64748b; --bg: #f1f5f9; }
        body { font-family: sans-serif; background: var(--bg); padding: 20px; color: #333; }
        .container { max-width: 900px; margin: 0 auto; background: white; padding: 30px; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); }
        
        .input-section { display: grid; grid-template-columns: 2fr 1fr 1fr auto; gap: 10px; margin-bottom: 20px; background: #f8fafc; padding: 15px; border-radius: 8px; }
        input, select { padding: 10px; border: 1px solid #cbd5e1; border-radius: 6px; }
        
        button { cursor: pointer; border: none; border-radius: 6px; padding: 10px 15px; transition: 0.2s; }
        .btn-add { background: var(--primary); color: white; font-weight: bold; }
        .btn-add:hover { background: #1d4ed8; }
        .btn-delete { background: #ef4444; color: white; padding: 5px 10px; }

        table { width: 100%; border-collapse: collapse; margin-top: 20px; }
        th { text-align: left; border-bottom: 2px solid #e2e8f0; padding: 12px; color: var(--secondary); }
        td { padding: 12px; border-bottom: 1px solid #f1f5f9; }

        .summary-boxes { display: flex; gap: 20px; margin-top: 30px; }
        .box { flex: 1; padding: 20px; border-radius: 10px; text-align: center; color: white; }
        .monthly-box { background: var(--primary); }
        .yearly-box { background: #0f172a; }
        .box h3 { margin: 0; font-size: 0.9rem; opacity: 0.9; }
        .box p { margin: 10px 0 0; font-size: 1.8rem; font-weight: bold; }
    </style>
</head>
<body>

<div class="container">
    <h2>Expense Tracker 2026</h2>
    
    <div class="input-section">
        <input type="text" id="expense-name" placeholder="Expense Head (e.g. Rent, Food)">
        <select id="expense-month">
            <option value="1">Monthly</option>
            <option value="12">Yearly (One-time)</option>
        </select>
        <input type="number" id="expense-amount" placeholder="Amount ($)">
        <button class="btn-add" onclick="addExpense()">Add Entry</button>
    </div>

    <table>
        <thead>
            <tr>
                <th>Expense Head</th>
                <th>Frequency</th>
                <th>Amount</th>
                <th>Action</th>
            </tr>
        </thead>
        <tbody id="expense-list">
            </tbody>
    </table>

    <div class="summary-boxes">
        <div class="box monthly-box">
            <h3>Total Monthly Expense</h3>
            <p id="total-monthly">$0.00</p>
        </div>
        <div class="box yearly-box">
            <h3>Projected Yearly Total</h3>
            <p id="total-yearly">$0.00</p>
        </div>
    </div>
</div>

<script>
    let expenses = [];

    function addExpense() {
        const name = document.getElementById('expense-name').value;
        const freq = document.getElementById('expense-month').value;
        const amount = parseFloat(document.getElementById('expense-amount').value);

        if (name && amount) {
            expenses.push({ name, freq, amount });
            updateUI();
            // Clear inputs
            document.getElementById('expense-name').value = '';
            document.getElementById('expense-amount').value = '';
        } else {
            alert("Please fill in all fields");
        }
    }

    function deleteExpense(index) {
        expenses.splice(index, 1);
        updateUI();
    }

    function updateUI() {
        const list = document.getElementById('expense-list');
        list.innerHTML = '';
        
        let monthlyTotal = 0;
        let yearlyTotal = 0;

        expenses.forEach((item, index) => {
            // Logic: If it's a monthly expense, yearly = monthly * 12
            // If it's a yearly expense, monthly = yearly / 12
            const mAmount = item.freq == "1" ? item.amount : (item.amount / 12);
            const yAmount = item.freq == "1" ? (item.amount * 12) : item.amount;

            monthlyTotal += mAmount;
            yearlyTotal += yAmount;

            list.innerHTML += `
                <tr>
                    <td>${item.name}</td>
                    <td>${item.freq == "1" ? "Monthly" : "Yearly"}</td>
                    <td>$${item.amount.toLocaleString()}</td>
                    <td><button class="btn-delete" onclick="deleteExpense(${index})">Remove</button></td>
                </tr>
            `;
        });

        document.getElementById('total-monthly').innerText = `$${monthlyTotal.toLocaleString(undefined, {minimumFractionDigits: 2})}`;
        document.getElementById('total-yearly').innerText = `$${yearlyTotal.toLocaleString(undefined, {minimumFractionDigits: 2})}`;
    }
</script>

</body>
</html>

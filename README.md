<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Expense Tracker</title>
    <style>
        :root {
            --primary: #2563eb;
            --bg: #f8fafc;
            --text: #1e293b;
            --card-bg: #ffffff;
            --border: #e2e8f0;
        }

        body {
            font-family: 'Inter', system-ui, sans-serif;
            background-color: var(--bg);
            color: var(--text);
            margin: 0;
            padding: 40px 20px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
        }

        header {
            margin-bottom: 30px;
            border-bottom: 2px solid var(--border);
            padding-bottom: 10px;
        }

        .dashboard-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 24px;
        }

        .card {
            background: var(--card-bg);
            padding: 24px;
            border-radius: 12px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
            border: 1px solid var(--border);
        }

        h2 { margin-top: 0; font-size: 1.25rem; color: var(--primary); }

        /* Table Styling */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }

        th {
            text-align: left;
            padding: 12px;
            background: #f1f5f9;
            font-weight: 600;
        }

        td {
            padding: 12px;
            border-bottom: 1px solid var(--border);
        }

        .amount { text-align: right; font-family: monospace; font-size: 1.1em; }
        
        .total-row {
            font-weight: bold;
            background: #f8fafc;
        }

        .badge {
            padding: 4px 8px;
            border-radius: 6px;
            background: #dbeafe;
            color: #1e40af;
            font-size: 0.85rem;
        }

        @media (max-width: 768px) {
            .dashboard-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Financial Overview <span style="font-weight: 300; color: #64748b;">2026</span></h1>
    </header>

    <div class="dashboard-grid">
        <div class="card">
            <h2>Monthly Expense Breakdown</h2>
            <p>Current Month: <strong>February</strong></p>
            <table>
                <thead>
                    <tr>
                        <th>Expense Head</th>
                        <th>Category</th>
                        <th class="amount">Amount</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Office Rent</td>
                        <td><span class="badge">Fixed</span></td>
                        <td class="amount">$1,200.00</td>
                    </tr>
                    <tr>
                        <td>Cloud Services</td>
                        <td><span class="badge">Sub</span></td>
                        <td class="amount">$45.00</td>
                    </tr>
                    <tr>
                        <td>Marketing Ads</td>
                        <td><span class="badge">Variable</span></td>
                        <td class="amount">$350.00</td>
                    </tr>
                    <tr class="total-row">
                        <td colspan="2">Monthly Total</td>
                        <td class="amount">$1,595.00</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="card">
            <h2>Yearly Summary</h2>
            <table>
                <tr>
                    <td>Q1 Total</td>
                    <td class="amount">$4,785</td>
                </tr>
                <tr>
                    <td>Q2 Total</td>
                    <td class="amount">$0</td>
                </tr>
                <tr>
                    <td>Q3 Total</td>
                    <td class="amount">$0</td>
                </tr>
                <tr>
                    <td>Q4 Total</td>
                    <td class="amount">$0</td>
                </tr>
                <tr class="total-row" style="color: var(--primary);">
                    <td>Annual Total</td>
                    <td class="amount">$4,785</td>
                </tr>
            </table>
            <p style="font-size: 0.8rem; color: #64748b; margin-top: 20px;">
                * Data updated as of Feb 28, 2026.
            </p>
        </div>
    </div>
</div>

</body>
</html>

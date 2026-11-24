<!DOCTYPE html>
<html lang="zh-HK">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>審題小偵探｜香港小三數學應用題深度變奏版</title>
  <style>
    :root {
      --bg: #f4f7fb;
      --card: #ffffff;
      --primary: #2563eb;
      --primary-dark: #1d4ed8;
      --accent: #f59e0b;
      --accent-soft: #fef3c7;
      --success: #16a34a;
      --success-soft: #dcfce7;
      --danger: #dc2626;
      --danger-soft: #fee2e2;
      --text: #1e293b;
      --muted: #64748b;
      --border: #e2e8f0;
      --radius: 16px;
      --shadow: 0 10px 25px -5px rgba(15, 23, 42, 0.08);
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "PingFang HK", "Microsoft JhengHei", sans-serif;
      background: linear-gradient(180deg, #eef4ff 0%, var(--bg) 260px);
      color: var(--text);
      line-height: 1.65;
    }

    .container {
      max-width: 920px;
      margin: 0 auto;
      padding: 20px 16px 60px;
    }

    header {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 20px 24px;
      box-shadow: var(--shadow);
      margin-bottom: 18px;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
    }

    .brand h1 {
      margin: 0 0 4px;
      font-size: 1.5rem;
      color: var(--primary-dark);
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .brand p {
      margin: 0;
      color: var(--muted);
      font-size: 0.95rem;
    }

    .stats {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
    }

    .stat-pill {
      background: #f8fafc;
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 8px 14px;
      text-align: center;
      min-width: 88px;
    }

    .stat-pill .num {
      font-size: 1.2rem;
      font-weight: 800;
      color: var(--primary);
      display: block;
    }

    .stat-pill .lbl {
      font-size: 0.78rem;
      color: var(--muted);
    }

    .toolbar {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 14px 18px;
      margin-bottom: 18px;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      box-shadow: var(--shadow);
    }

    .toolbar-group {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px;
    }

    label {
      font-size: 0.9rem;
      font-weight: 600;
      color: var(--text);
    }

    select, button, input[type="number"], input[type="text"] {
      font-family: inherit;
      font-size: 0.95rem;
      border-radius: 10px;
      border: 1px solid #cbd5e1;
      padding: 8px 12px;
      background: #fff;
      color: var(--text);
    }

    button {
      cursor: pointer;
      font-weight: 600;
      transition: all 0.15s ease;
    }

    button:hover:not(:disabled) {
      transform: translateY(-1px);
    }

    button:disabled {
      opacity: 0.45;
      cursor: not-allowed;
    }

    .btn-primary {
      background: var(--primary);
      color: #fff;
      border-color: var(--primary);
    }

    .btn-primary:hover:not(:disabled) {
      background: var(--primary-dark);
    }

    .btn-accent {
      background: var(--accent);
      color: #fff;
      border-color: var(--accent);
    }

    .btn-outline {
      background: #fff;
      color: var(--text);
    }

    .btn-success {
      background: var(--success);
      color: #fff;
      border-color: var(--success);
    }

    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 24px;
      box-shadow: var(--shadow);
      margin-bottom: 18px;
    }

    .badge-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;

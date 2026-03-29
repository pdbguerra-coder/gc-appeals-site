<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>GC Appeals Center</title>  
  <style>  
    body {  
      font-family: Arial, sans-serif;  
      background: #0f172a;  
      color: white;  
      display: flex;  
      justify-content: center;  
      align-items: center;  
      height: 100vh;  
      margin: 0;  
    }  
  
    .container {  
      background: #1e293b;  
      padding: 25px;  
      border-radius: 12px;  
      width: 400px;  
      box-shadow: 0 10px 25px rgba(0,0,0,0.5);  
    }  
  
    h1 {  
      text-align: center;  
      margin-bottom: 15px;  
    }  
  
    label {  
      display: block;  
      margin-top: 10px;  
      font-size: 14px;  
    }  
  
    input, select, textarea {  
      width: 100%;  
      padding: 8px;  
      margin-top: 5px;  
      border-radius: 6px;  
      border: none;  
      outline: none;  
    }  
  
    textarea {  
      resize: none;  
      height: 80px;  
    }  
  
    button {  
      margin-top: 15px;  
      width: 100%;  
      padding: 10px;  
      border: none;  
      border-radius: 8px;  
      background: #3b82f6;  
      color: white;  
      font-weight: bold;  
      cursor: pointer;  
    }  
  
    button:hover {  
      background: #2563eb;  
    }  
  
    .note {  
      font-size: 12px;  
      margin-top: 10px;  
      color: #94a3b8;  
      text-align: center;  
    }  
  </style>  
</head>  
<body>  
  
  <div class="container">  
    <h1>Appeal Ticket</h1>  
  
    <form onsubmit="submitAppeal(event)">  
      <label>Username / Display Name</label>  
      <input type="text" required>  
  
      <label>Date of Incident</label>  
      <input type="date" required>  
  
      <label>Type of Action</label>  
      <select required>  
        <option value="">Select</option>  
        <option>Warning</option>  
        <option>Temporary Ban</option>  
        <option>Permanent Ban</option>  
      </select>  
  
      <label>Reason for Appeal</label>  
      <textarea required></textarea>  
  
      <label>Additional Evidence (optional)</label>  
      <input type="file">  
  
      <button type="submit">Submit Appeal</button>  
    </form>  
  
    <div class="note">  
      Review time: 24–72 hours. Decisions are final.  
    </div>  
  </div>  
  
  <script>  
    function submitAppeal(e) {  
      e.preventDefault();  
      alert("Your appeal has been submitted for review.");  
    }  
  </script>  
  
</body>  
</html>  

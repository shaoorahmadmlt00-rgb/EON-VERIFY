<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<title>EON Verify</title>
<style>
body{font-family:sans-serif;text-align:center;padding:40px;background:#f7f7f7}
.card{max-width:380px;margin:auto;background:white;border-radius:16px;padding:24px;box-shadow:0 4px 12px rgba(0,0,0,0.1)}
.ok{color:green;font-size:22px}
.bad{color:red;font-size:22px}
</style>
</head>
<body>
<div class="card">
<h2 id="result">Scanning…</h2>
<p id="details"></p>
</div>
<script>
const url = new URL(window.location.href);
const code = url.searchParams.get("code");
const validCodes = ["PRIM001","PRIM002","PRIM003"]; // add your real codes here
if(validCodes.includes(code)){
  result.textContent = "✅ Original PRIM";
  details.textContent = "Serial: "+code;
  result.className="ok";
}else{
  result.textContent = "❌ Fake / Invalid Code";
  details.textContent = "This product may be counterfeit.";
  result.className="bad";
}
</script>
</body>
</html>
# EON-VERIFY

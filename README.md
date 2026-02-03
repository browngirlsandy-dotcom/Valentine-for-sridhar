# Valentine-for-sridhar
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Sridhar Nishant ❤️</title>

<style>
body {
  margin: 0;
  height: 100vh;
  background: linear-gradient(135deg, #ff6f91, #ff9a9e);
  font-family: 'Courier New', monospace;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

/* Floating hearts */
.heart {
  position: fixed;
  bottom: -20px;
  font-size: 22px;
  animation: floatUp 7s linear infinite;
}
@keyframes floatUp {
  0% { transform: translateY(0) scale(1); opacity: 1; }
  100% { transform: translateY(-110vh) scale(1.4); opacity: 0; }
}

/* Card */
.card {
  position: relative;
  background: white;
  padding: 34px;
  border-radius: 24px;
  text-align: center;
  box-shadow: 0 30px 60px rgba(0,0,0,0.35);
  max-width: 460px;
  z-index: 2;
  animation: popIn 1.2s ease;
}

@keyframes popIn {
  from { transform: scale(0.8); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

h1 {
  color: #e63946;
  margin-bottom: 10px;

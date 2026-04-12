# Live

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Live Pulse Loader</title>

<style>
body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #0f172a;
    font-family: Arial, sans-serif;
}

/* Pulse Circle */
.pulse-circle {
    position: relative;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: #38bdf8;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 26px;
    font-weight: bold;
    letter-spacing: 3px;
}

/* Pulse effect */
.pulse-circle::before,
.pulse-circle::after {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    border-radius: 50%;
    background: #38bdf8;
    opacity: 0.6;
    animation: pulse 2s infinite;
}

.pulse-circle::after {
    animation-delay: 1s;
}

/* Animation */
@keyframes pulse {
    0% {
        transform: scale(1);
        opacity: 0.6;
    }
    100% {
        transform: scale(2);
        opacity: 0;
    }
}
</style>

</head>
<body>

<div class="pulse-circle">
    LIVE
</div>

</body>
</html>

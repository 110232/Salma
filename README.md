<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Página Rosa Pastel</title>
  <style>
    body {
      font-family: 'Poppins', Arial, sans-serif;
      background: linear-gradient(to bottom right, #ffe6f0, #fff5fa);
      color: #333;
      margin: 0;
      padding: 0;
      text-align: center;
      overflow-x: hidden;
      height: 100vh;
    }

    /* Pantalla inicial */
    #pantalla-inicial {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(to bottom right, #ffc1d9, #fff0f5);
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      z-index: 200;
      animation: fadeOut 1s ease 6s forwards;
    }

    #pantalla-inicial h1 {
      color: #ff4d79;
      font-size: 2em;
      text-shadow: 1px 1px 3px #ff91a4;
      animation: parpadeo 1.5s infinite;
      font-weight: 600;
    }

    @keyframes parpadeo {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.6; }
    }

    @keyframes fadeOut {
      to { opacity: 0; visibility: hidden; }
    }

    header {
      background-color: #ffb6c1;
      color: white;
      padding: 20px 0;
      font-size: 2em;
      font-weight: 700;
      letter-spacing: 0.5px;
      text-shadow: 1px 1px 3px #ff91a4;
    }

    section {
      display: none;
      padding: 40px 20px;
      min-height: calc(100vh - 150px);
      box-sizing: border-box;
      overflow-y: auto;
      max-height: calc(100vh - 150px);
      scrollbar-width: thin;
      scrollbar-color: #ffb6c1 #ffe6f0;
    }

    section::-webkit-scrollbar {
      width: 8px;
    }

    section::-webkit-scrollbar-thumb {
      background-color: #ffb6c1;
      border-radius: 10px;
    }

    section.active {
      display: block;
      animation: fadeIn 0.5s ease-in-out;
    }

    p {
      max-width: 600px;
      margin: 0 auto 20px;
      line-height: 1.6;
      font-size: 1.1em;
      color: #444;
    }

    nav {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100%;
      background-color: #ffd6e0;
      display: flex;
      justify-content: space-around;
      padding: 12px 0;
      border-top: 2px solid #ffb6c1;
      z-index: 100;
    }

    nav button {
      background-color: #ffb6c1;
      border: none;
      border-radius: 50%;
      width: 45px;
      height: 45px;
      font-size: 1.1em;
      color: white;
      font-weight: 600;
      cursor: pointer;
      t

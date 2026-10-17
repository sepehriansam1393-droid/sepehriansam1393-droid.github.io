# sepehriansam1393-droid.github.io
Official website of Sam Sepehrian | Karting × Volleyball<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#101010">
<meta name="description" content="Official sports profile of Sam Sepehrian — Karting and Volleyball.">
<title>SAM SEPEHRIAN | Official</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --orange: #ff6a00;
  --black: #0b0b0d;
  --panel: #151518;
  --white: #f5f5f5;
  --gray: #a3a3aa;
}

html {
  scroll-behavior: smooth;
}

body {
  background: var(--black);
  color: var(--white);
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.6;
}

a {
  color: inherit;
  text-decoration: none;
}

header {
  position: sticky;
  top: 0;
  z-index: 10;
  background: rgba(11,11,13,.94);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid #29292d;
}

nav {
  max-width: 1150px;
  margin: auto;
  padding: 18px 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}

.logo {
  font-weight: 900;
  letter-spacing: 2px;
  font-size: 19px;
}

.logo span {
  color: var(--orange);
}

.nav-links {
  display: flex;
  gap: 22px;
  font-size: 13px;
  color: #ddd;
}

.nav-links a:hover {
  color: var(--orange);
}

.hero {
  min-height: 88vh;
  display: flex;
  align-items: center;
  position: relative;
  overflow: hidden;
  background:
    radial-gradient(ellipse at 90% 45%, #47200e 0%, transparent 40%),
    linear-gradient(120deg, #0b0b0d 45%, #17110e);
}

.hero::after {
  content: "S";
  position: absolute;
  right: 5%;
  top: 0;
  font-size: clamp(250px, 43vw, 620px);
  font-weight: 900;
  line-height: 1;
  color: rgba(255,106,0,.055);
  pointer-events: none;
}

.hero-inner {
  width: 1150px;
  max-width: 100%;
  padding: 80px 24px;
  margin: auto;
  position: relative;
  z-index: 1;
  animation: enter 1s ease both;
}

.eyebrow {
  color: var(--orange);
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 5px;
  text-transform: uppercase;
}

h1 {
  font-size: clamp(46px, 8vw, 100px);
  line-height: .98;
  letter-spacing: -4px;
  margin: 24px 0;
  font-weight: 900;
}

h1 span {
  color: var(--orange);
}

.hero p {
  color: #c2c2c8;
  max-width: 520px;
  font-size: 17px;
}

.buttons {
  display: flex;
  gap: 14px;
  flex-wrap: wrap;
  margin-top: 32px;
}

.btn {
  padding: 13px 22px;
  border: 1px solid #45454b;
  font-size: 13px;
  font-weight: bold;
  transition: .25s;
}

.btn.primary {
  background: var(--orange);
  color: #111;
  border-color: var(--orange);
}

.btn:hover {
  transform: translateY(-4px);
  border-color: var(--orange);
}

section {
  max-width: 1150px;
  padding: 90px 24px;
  margin: auto;
}

.section-label {
  color: var(--orange);
  letter-spacing: 4px;
  font-size: 11px;
  font-weight: bold;
}

h2 {
  font-size: clamp(32px, 5vw, 53px);
  line-height: 1.1;
  margin: 12px 0 20px;
  letter-spacing: -1px;
}

.intro {
  color: var(--gray);
  max-width: 650px;
  margin-bottom: 35px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 20px;
}

.card {
  background: linear-gradient(145deg, #19191d, #101012);
  border: 1px solid #29292e;
  padding: 30px;
  min-height: 250px;
  position: relative;
  overflow: hidden;
  transition: .3s;
}

.card:hover {
  transform: translateY(-6px);
  border-color: var(--orange);
}

.card .number {
  color: var(--orange);
  font-size: 12px;
  letter-spacing: 3px;
}

.card h3 {
  font-size: 29px;
  margin: 30px 0 12px;
}

.card p {
  color: var(--gray);
  font-size: 14px;
}

.card .symbol {
  position: absolute;
  right: 15px;
  bottom: -40px;
  font-size: 130px;
  opacity: .08;
}

.highlight {
  background: var(--orange);
  color: #101010;
  max-width: none;
  padding: 65px 24px;
}

.highlight-inner {
  max-width: 1100px;
  margin: auto;
}

.highlight .section-label {
  color: #321300;
}

.highlight p {
  max-width: 700px;
}

.highlight h2 {
  max-width: 750px;
}

.contact-box {
  padding: 35px;
  border: 1px solid #303035;
  background: var(--panel);
}

.contact-box p {
  color: var(--gray);
  margin-bottom: 22px;
}

footer {
  border-top: 1px solid #29292d;
  padding: 25px 20px;
  text-align: center;
  color: #888;
  font-size: 12px;
}

footer span {
  color: var(--orange);
}

@keyframes enter {
  from {
    opacity: 0;
    transform: translateY(25px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 650px) {
  nav {
    padding: 15px;
    flex-wrap: wrap;
  }

  .nav-links {
    width: 100%;
    gap: 16px;
    flex-wrap: wrap;
    font-size: 12px;
  }

  .hero {
    min-height: 75vh;
  }

  h1 {
    letter-spacing: -2px;
  }

  .cards {
    grid-template-columns: 1fr;
  }

  section {
    padding: 65px 20px;
  }
}

@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    scroll-behavior: auto !important;
    animation: none !important;
    transition: none !important;
  }
}
</style>
</head>

<body>

<header>
  <nav>
    <a class="logo" href="#home">SAM <span>SEPEHRIAN</span

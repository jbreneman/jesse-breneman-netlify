<template>
  <div class="page-background">
    <nuxt/>
  </div>
</template>

<style>
html {
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Work Sans', sans-serif;
}

*, *:before, *:after{
  box-sizing: border-box;
  margin: 0;
}

.page-background {
	padding: 2rem;
	min-width: 100%;
	min-height: 100vh;
	display: flex;
	flex-direction: column;
	justify-content: center;
	background-image: radial-gradient(ellipse at 100% 100%, rgba(38, 13, 119, 0.89) 0%, transparent 50%), radial-gradient(ellipse at 70% 0, rgba(76, 162, 113, 0.52) 0%, transparent 50%), radial-gradient(ellipse at 30% 100%, rgba(102, 13, 119, 0.81) 0%, transparent 50%), radial-gradient(ellipse at 10% 0, rgba(38, 45, 119, 0.94) 0%, transparent 50%), linear-gradient(#26788D, #26788D);
}
</style>

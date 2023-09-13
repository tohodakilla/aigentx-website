<script>
	export let feats = []
</script>

<div class="container">
	{#each feats as f}
		<div class="box">
			<!-- <span></span> -->
			<div class="content text-center">
				<p class="text-5xl mb-3">{f.emo}</p>
				<p class="text-3xl font-bold mb-3">{f.head}</p>
				<p class="text-2xl">{f.text}</p>
			</div>
		</div>
	{/each}
</div>

<style>
	.box p {
		position: relative;
		z-index: 100;
	}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  padding: 40px 0;
}

.container .box
{
  position: relative;
  width: 320px;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 40px 30px;
  transition: 0.5s;
}

.container .box::before
{
  content:' ';
  position: absolute;
  top: 0;
  left: 50px;
  width: 50%;
  height: 100%;
  text-decoration: none;
  background: #fff;
  border-radius: 8px;
  transform: skewX(15deg);
  transition: 0.5s;
}

.container .box::after
{
  content:'';
  position: absolute;
  top: 0;
  left: 50;
  width: 50%;
  height: 100%;
  background: #fff;
  border-radius: 8px;
  transform: skewX(15deg);
  transition: 0.5s;
  filter: blur(30px);
}

.container .box:hover:before,
.container .box:hover:after
{
  transform: skewX(0deg);
  left: 42px;
  width: calc(100% - 90px);
  
}
/* .container .box:before,
.container .box:after {
  background: linear-gradient(315deg, #3e7dffb0, #1d227d);
} */
/* Gradients for the 1 column layout */
.container .box:nth-child(1):before,
.container .box:nth-child(1):after {
  background: linear-gradient(315deg, #3e7dffb0, #1d227d);
}

.container .box:nth-child(2):before,
.container .box:nth-child(2):after {
  background: linear-gradient(315deg, #7fcce4b0, #4583ad);
}

.container .box:nth-child(3):before,
.container .box:nth-child(3):after {
  background: linear-gradient(315deg, #ffcb64b0, #ad8e49);
}

.container .box:nth-child(4):before,
.container .box:nth-child(4):after {
  background: linear-gradient(315deg,#cb50dc,#290028);
}

.container .box:nth-child(5):before,
.container .box:nth-child(5):after {
  background: linear-gradient(315deg, #00cc8fb0, #006d4c);
}

.container .box:nth-child(6):before,
.container .box:nth-child(6):after {
  background: linear-gradient(315deg, #ff3d00b0, #9f2000);
}

.container .box:nth-child(7):before,
.container .box:nth-child(7):after {
  background: linear-gradient(315deg, #ffbb00b0, #ad8e49);
}

.container .box:nth-child(8):before,
.container .box:nth-child(8):after {
  background: linear-gradient(315deg, #5a00a0b0, #2b004d);
}

.container .box:nth-child(9):before,
.container .box:nth-child(9):after {
  background: linear-gradient(315deg, #1d227db0, #3e7dff);
}

.container .box:nth-child(10):before,
.container .box:nth-child(10):after {
  background: linear-gradient(315deg,#6d0000,#cc3b00)
}

/* Gradients for the 2 columns layout */
/* Shuffle the order to avoid same colors beside each other */

/* Gradients for the 3 columns layout */
/* Shuffle the order to avoid same colors beside each other */



.container .box span
{
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 5;
  pointer-events: none;
}

.container .box span::before
{
  content:'';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 0;
  border-radius: 8px;
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  opacity: 0;
  transition: 0.1s;  
  animation: animate 2s ease-in-out infinite;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08)
}

.container .box:hover span::before
{
  top: -50px;
  left: 50px;
  width: 100px;
  height: 100px;
  opacity: 1;
}

.container .box span::after
{
  content:'';
  position: absolute;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
  border-radius: 8px;
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  opacity: 0;
  transition: 0.5s;
  animation: animate 2s ease-in-out infinite;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  animation-delay: -1s;
}

.container .box:hover span:after
{
  bottom: -50px;
  right: 50px;
  width: 100px;
  height: 100px;
  opacity: 1;
}

@keyframes animate
{
  0%, 100%
  {
    transform: translateY(10px);
  }
  
  50%
  {
    transform: translate(-10px);
  }
}

.container .box .content
{
  position: relative;
  left: 0;
  padding: 20px 40px;
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  z-index: 1;
  transform: 0.5s;
  color: #fff;
}
</style>
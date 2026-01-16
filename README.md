<svg fill="none" viewBox="0 0 800 400" width="800" height="400" xmlns="http://www.w3.org/2000/svg">
	<foreignObject width="100%" height="100%">
		<div xmlns="http://www.w3.org/1999/xhtml">
			<style>
				@keyframes glitch {
					0% { transform: translate(0) }
					20% { transform: translate(-2px, 2px) }
					40% { transform: translate(-2px, -2px) }
					60% { transform: translate(2px, 2px) }
					80% { transform: translate(2px, -2px) }
					to { transform: translate(0) }
				}
				@keyframes scanline {
					0% { transform: translateY(-100%) }
					to { transform: translateY(100%) }
				}
				@keyframes flicker {
					0% { opacity: 1 }
					50% { opacity: .8 }
					to { opacity: 1 }
				}
				.container {
					font-family: 'Courier New', monospace;
					text-align: center;
					background: #0a0a0a;
					color: #fff;
					padding: 50px 20px;
					border-radius: 10px;
					position: relative;
					overflow: hidden;
					height: 300px;
					display: flex;
					flex-direction: column;
					justify-content: center;
					align-items: center;
					border: 2px solid #0ff;
					box-shadow: 0 0 20px #0ff, inset 0 0 20px #0ff;
				}
				.container::before {
					content: "";
					position: absolute;
					top: 0;
					left: 0;
					width: 100%;
					height: 100%;
					background: repeating-linear-gradient(0deg, rgba(0, 255, 255, 0.1) 0px, rgba(0, 255, 255, 0.1) 1px, transparent 1px, transparent 2px);
					pointer-events: none;
				}
				.container::after {
					content: "";
					position: absolute;
					top: 0;
					left: 0;
					width: 100%;
					height: 100%;
					background: rgba(0, 255, 255, 0.05);
					animation: scanline 6s linear infinite;
					pointer-events: none;
				}
				.glitch {
					font-size: 4em;
					font-weight: bold;
					text-transform: uppercase;
					position: relative;
					text-shadow: 0.05em 0 0 #00fffc, -0.03em -0.04em 0 #fc00ff, 0.025em 0.04em 0 #fffc00;
					animation: glitch 725ms infinite;
				}
				.glitch::before, .glitch::after {
					content: attr(data-text);
					position: absolute;
					top: 0;
					left: 0;
					opacity: 0.8;
				}
				.glitch::before {
					animation: glitch 500ms infinite;
					clip-path: polygon(0 0, 100% 0, 100% 35%, 0 35%);
					transform: translate(-0.04em, -0.03em);
					color: #00fffc;
				}
				.glitch::after {
					animation: glitch 375ms infinite;
					clip-path: polygon(0 65%, 100% 65%, 100% 100%, 0 100%);
					transform: translate(0.04em, 0.03em);
					color: #fc00ff;
				}
				.subtitle {
					font-size: 1.5em;
					color: #0ff;
					margin-top: 10px;
					letter-spacing: 2px;
					animation: flicker 2s infinite;
				}
				.description {
					font-size: 1em;
					margin-top: 20px;
					color: #aaa;
					max-width: 80%;
				}
				.highlight {
					color: #0ff;
					font-weight: bold;
				}
			</style>
			<div class="container">
				<div class="glitch" data-text="MyStIc-mY">MyStIc-mY</div>
				
				<div class="subtitle">AMIT KUMAR</div>
				
				<div class="description">
					<span class="highlight">PYTHON</span> | AI & FUTURE TECH | SKILLING YOUTH
				</div>
			</div>
		</div>
	</foreignObject>
</svg>

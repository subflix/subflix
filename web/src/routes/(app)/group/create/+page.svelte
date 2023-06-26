<div class="border-b">
	<h1 class="h3">สร้างกลุ่มใหม่</h1>
</div>

<div class="container mx-auto">
	<div class="card max-w-lg mx-auto">
		<div class="p-4">
			<form action="" method="POST" class="space-y-4">
				<label class="label">
					<span>ชื่อกลุ่มหาร</span>
					<input class="input" type="text" placeholder="หาร netflix" />
				</label>
				<label class="label">
					<span>จำนวนเงินที่ต้องจ่ายต่อเดือน</span>
					<input class="input" type="number" step="0.01" placeholder="500.00" />
				</label>

				<div class="grid gap-4 col-span-4 grid-flow-col">
					<label class="flex items-center space-x-2">
						<input class="radio" name="platform" type="radio" value="Netflix" />
						<p>Netflix</p>
					</label>
					<label class="flex items-center space-x-2">
						<input class="radio" name="platform" type="radio" value="VIU" />
						<p>VIU</p>
					</label>
					<label class="flex items-center space-x-2">
						<input class="radio" name="platform" type="radio" value="Disney+" />
						<p>Disney+</p>
					</label>
					<label class="flex items-center space-x-2">
						<input class="radio" name="platform" type="radio" value="Disney+" />
						<p>Spotify</p>
					</label>
				</div>

				<button class="btn variant-filled-primary w-full mt-10"> Create </button>
			</form>
		</div>
	</div>
</div>

<script>
	function closeMenu() {
		this.hide();
	}
</script>

<ion-menu side="start">
	<ion-header>
		<ion-toolbar translucent>
			<ion-title>Menu</ion-title>
		</ion-toolbar>
	</ion-header>
	<ion-content>
		<ion-list>
			<ion-item on:click={closeMenu}>
				<ion-icon name="home" slot="start" />
				<ion-label>Home</ion-label>
			</ion-item>
			<ion-item on:click={closeMenu}>
				<ion-icon name="person" slot="start" />
				<ion-label>Profile</ion-label>
			</ion-item>
			<ion-item on:click={closeMenu}>
				<ion-icon name="chatbubbles" slot="start" />
				<ion-label>Messages</ion-label>
			</ion-item>
			<ion-item on:click={closeMenu}>
				<ion-icon name="settings" slot="start" />
				<ion-label>Settings</ion-label>
			</ion-item>
		</ion-list>
	</ion-content>
</ion-menu>

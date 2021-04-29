<script lang="ts" href="https://unpkg.com/mdbsvelte@latest/dist/mdbsvelte.js">
	 import Nav from './pages/Nav.svelte';
	 import {MDBContainer, MDBRow, MDBCol} from "mdbsvelte";
	 import SystemStatus from './pages/SystemStatus2.svelte';
</script>

<index>
	<MDBContainer fluid>
		<MDBRow>
			<MDBCol md='3'>
				<Nav/>
			</MDBCol>
			<MDBCol md='9 pl-0'>
				<SystemStatus/>
			</MDBCol>
		</MDBRow>
	</MDBContainer>
</index>

<style>
	index {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		index {
			max-width: none;
		}
	}
</style>

<script>
  import Header from '../components/Header.svelte';
  import Main from '../components/Main.svelte';
  import SideBar from '../components/SideBar.svelte';
  import TimeLine from '../components/TimeLine.svelte';


</script>

<style>
  :global(body){
    background: #676778;
    color:white;
  }

</style>

<Header/>
<Main>
  <TimeLine/>
  <SideBar/>
</Main>
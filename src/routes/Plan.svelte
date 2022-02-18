<script>
import TaskList from '../components/Tasklist.svelte'
</script>

<h2>Planning Organizer</h2>
<div class="view">Facilitator View</div>
<TaskList/>

<style lang="scss">
  h2 {
    @extend %route-title;
  }
</style>
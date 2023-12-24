<script lang="tsx">
import { defineComponent, ref } from 'vue'


export default defineComponent({
  // props: {

  // },
  setup() {
    const content = ref('关于页面的内容')
    function add() {
      content.value += 1
    }

    return () => <>
      <h3>这是关于页面的标题</h3>
      <main>
        {content.value}
      </main>
      <button onClick={add}>添加内容</button>
    </>
  }
})
</script>

<style scoped>
h3 {
  color: aqua;
}
</style>
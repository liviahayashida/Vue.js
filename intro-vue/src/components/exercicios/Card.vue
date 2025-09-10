    <template>
      <div>
        <header>
          <slot name="header"></slot> 
        </header>
        <main>
          <slot>Bem-vindo (default)</slot> 
        </main>
        <footer>
          <slot name="footer"></slot> 
        </footer>
      </div>
    </template>

<script>
export default {
  name: 'Cards'
}
</script>

<style scoped>
*{
    background-color: #ab39e4;
    color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
}
</style>
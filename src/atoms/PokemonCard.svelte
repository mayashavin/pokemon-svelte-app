<script>
  export let card;
</script>
<style>
  .item {
    border: 1px solid lightgray;
    display: flex;
    justify-content: center;
    flex-direction: column;
    padding: 5px;
    margin-right:10px;
    margin-bottom: 10px;
    width: 220px;
    box-shadow: 0 1px 2px rgba(0,0,0,.2);
  }

  .item:hover {
    background-color: #d3d3d363;
    cursor: pointer;
  }

  h3 {
    margin: 0;
    padding: 0.8rem 0;
    border-top: 1px solid lightgray;
    text-align: center;
  }

  img {
    width: 200px;
    height: auto;
  }

</style>
<div class="item">
  <img src={card.url} alt={card.title}/>
  <h3>{card.title}</h3>
</div>
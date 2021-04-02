<template>
  <div class="main-container">

	  <div class="filter-cart-container">
        
		  <div class="filter-container">
              <ng-filter />
          </div>

		  <div class="cart-container">cart</div>

	  </div>

	  <div class="search-result-container">

		  <div>search bar</div>

		  <div>results</div>

	  </div>

    
  </div>
</template>

<script>
    import ngFilter from '@/components/filter/ng-filter'

    export default {

        head() {
            return {
                title: 'My Next Guitar !'
            }
        },

        components: {
            ngFilter,
        }
    }
</script>

<style scoped>
    * {
        margin: 0
    }
    
    .main-container {
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        height: auto;
        border: 1px solid red;
        padding: 0 10px 0 10px;
    }
    
    .filter-cart-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        height: 350px;
    }
    
    .search-result-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        border: 1px solid green;
    }
</style>
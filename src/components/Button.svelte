<script>

    import { goto } from '$app/navigation';

    /**
	 * @type {string | URL}
	 */
     export let ep; 

    function onClick(){
        goto(ep)
    }

</script>

<div class="row d-flex justify-content-center">
    <div class="col-md-9 text-center justify-content-center">
          <button on:click="{onClick}" type="button" class="btn btn-lg btn-secondary" >
              Dál
          </button>
      </div>
  </div>
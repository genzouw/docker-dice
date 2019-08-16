<template>
  <div>
    <div class="row justify-content-center">
      <div class="col-auto">
        <h1>It's "Dice" web api.</h1>
      </div>
    </div>

    <hr />

    <div class="row justify-content-center">
      <div class="col-auto">
        <h2>What is "Dice"?</h2>
      </div>
    </div>

    <div class="row">
      <div class="col-sm-10 offset-sm-1">
        <p>
        This is a web API that randomly generates dice eyes.
        </p>

        <ul>
          <li>Returns a value between 1 and 6 at random.</li>
          <li>The response is output in JSON format.</li>
          <li>Anyone can use it for free.</li>
        </ul>
      </div>
    </div>

    <hr />

    <div class="row justify-content-center">
      <div class="col-auto">
        <h2>How to use</h2>
      </div>
    </div>

    <div class="row">
      <div class="col-sm-10 offset-sm-1">
        <p>
        Please access the following URL.
        </p>

        <ul>
          <li><a href="http://dice.spinosaurus.work/v1/dice">http://dice.spinosaurus.work/v1/dice</a></li>
        </ul>

        <p>
        The following JSON response is returned.
        The value of the dice roll changes randomly.
        </p>

        <prism language="javascript">
        {"dice":5}
        </prism>

        <p>If you use "curl" command, execute the following command. </p>

        <prism language="bash">
        curl -I \
          --request GET \
          --url http://dice.spinosaurus.work/v1/dice
        </prism>

      </div>
    </div>

  </div>
</template>

<script>
  import Prism from 'vue-prismjs'
  import 'prismjs/themes/prism.css'

  export default {
    components: {
      Prism
    }
  }
</script>

<style>
</style>

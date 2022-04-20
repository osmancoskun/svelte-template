<script>
  import { onMount } from "svelte";
  export let id;
  export let type = "primary";
  export let inverse = false;
  export let flat = false;
  export let disabled;
</script>

<button on:click {disabled} {id} class={type} class:inverse class:flat>
  <slot />
</button>

<style>
  .primary {
    background-color: #7957d5;
    color: white;
  }
  .primary.outlined {
    border-color: #7957d5;
    background-color: white;
    color: #7957d5;
  }
  .primary.light {
    background-color: #f2effb;
    color: #552fbc;
  }
  .success {
    background-color: #48c78e;
    color: white;
  }

  .success.outlined {
    border-color: #48c78e;
    background-color: white;

    color: #48c78e;
  }
  .success.light {
    background-color: #effaf5;
    color: #257953;
  }
  .danger {
    background-color: #f14668;
    color: white;
  }
  .danger.outlined {
    background-color: white;

    border-color: #f14668;
    color: #f14668;
  }
  .danger.light {
    background-color: #feecf0;
    color: #cc0f35;
  }
  .warning {
    background-color: #ffe08a;
    color: rgba(0, 0, 0, 0.7);
  }
  .warning.outlined {
    background-color: white;
    border-color: #ffe08a;
    color: rgba(0, 0, 0, 0.7);
  }
  .warning.light {
    background-color: #fffaeb;
    color: #946c00;
  }
  .info {
    background-color: #3e8ed0;
    color: white;
  }
  .info.outlined {
    background-color: white;
    border-color: #3e8ed0;
    color: #3e8ed0;
  }
  .info.light {
    background-color: #eff5fb;
    color: #296fa8;
  }
  .link {
    background-color: #485fc7;
    border-color: transparent;
    color: #fff;
  }
  .link.light {
    background-color: #eff1fa;
    color: #3850b7;
  }
  .light {
    background-color: #f5f5f5;
    border-color: transparent;
    color: rgba(0, 0, 0, 0.7);
  }
  .dark {
    background-color: #363636;
    border-color: transparent;
    color: #fff;
  }
  .text {
    background-color: transparent;
    border-color: transparent;
    color: #4a4a4a;
    text-decoration: underline;
  }
  .ghost {
    background: none;
    border-color: transparent;
    color: #7957d5;
    text-decoration: none;
  }
  .rounded {
    border-radius: 9999px;
    padding-left: 1.25em;
    padding-right: 1.25em;
  }
  button {
    background-color: #fff;
    border-color: #dbdbdb;
    border-width: 1px;
    border-radius: 5px;
    color: #363636;
    cursor: pointer;
    justify-content: center;
    padding: calc(0.5em - 1px) 1em;
    text-align: center;
    white-space: nowrap;
  }
  button::hover {
    box-shadow: 1px 2px 3px rgba(0, 0, 0, 0.2px);
  }
  button:active {
    color: white;
    background-color: lightgray;
    border: 1px solid gray;
  }
  button[disabled] {
    background-color: #fff;
    border-color: #dbdbdb;
    box-shadow: none;
    opacity: 0.5;
  }
</style>

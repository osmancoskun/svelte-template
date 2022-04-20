<script>
  import { metatags } from "@roxi/routify";
  import Button from "../components/m-button.svelte";

  metatags.title = "Svelte Template";
  metatags.description = "Svelte Template with Beautiful Components";
  let types = ["primary", "success", "danger", "warning", "info"];
</script>

<h1>Svelte Template With Components</h1>

<table>
  <tr>
    <th>NORMAL</th>
    <th>OUTLINED</th>
    <th>LIGHT</th>
  </tr>

  <tr>
    <td>
      <Button type="primary">primary</Button>
    </td>
    <td>
      <Button type="primary outlined">primary outlined</Button>
    </td>
    <td>
      <Button type="primary light">primary light</Button>
    </td>
  </tr>

  <tr>
    <td> <Button type="success">success</Button></td>
    <td> <Button type="success outlined">success outlined</Button></td>
    <td> <Button type="success light">success light</Button></td>
  </tr>
  <tr>
    <td> <Button type="danger">danger</Button></td>
    <td> <Button type="danger outlined">danger outlined</Button></td>
    <td> <Button type="danger light">danger light</Button></td>
  </tr>
  <tr>
    <td> <Button type="warning">warning</Button></td>
    <td> <Button type="warning outlined">warning outlined</Button></td>
    <td> <Button type="warning light">warning light</Button></td>
  </tr>
  <tr>
    <td> <Button type="info">info</Button></td>
    <td> <Button type="info outlined">info outlined</Button></td>
    <td> <Button type="info light">info light</Button></td>
  </tr>
  <tr>
    <td> <Button type="link">link</Button></td>
    <td> <Button type="link light">link light</Button></td>
  </tr>
  <tr>
    <td> <Button type="light">light</Button></td>
    <td> <Button type="dark">dark</Button></td>
  </tr>
  <tr>
    <td> <Button type="ghost">ghost</Button></td>
    <td> <Button type="text">text</Button></td>
  </tr>
</table>

<style>
  .maman {
    display: flex;
    flex-flow: row wrap;
  }
</style>

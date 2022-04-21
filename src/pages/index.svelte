<script>
  import { metatags } from "@roxi/routify";
  import Button from "../components/m-button.svelte";
  import Icon from "../components/m-icon.svelte";
  import Col from "../components/layout/Col.svelte";
  import Row from "../components/layout/Row.svelte";

  import AlignCenter from "../components/layout/AlignCenter.svelte";

  metatags.title = "Svelte Template";
  metatags.description = "Svelte Template with Beautiful Components";
  let types = ["primary", "success", "danger", "warning", "info"];
</script>

<h1>Svelte Template With Components</h1>
<h3>Buefy Inspired Buttons</h3>
<Col>
  <Row>
    <Button type="primary">primary</Button>
    <Button type="primary outlined">primary outlined</Button>
    <Button type="primary light">primary light</Button>
  </Row>
  <Row>
    <Button type="success">success</Button>
    <Button type="success outlined">success outlined</Button>
    <Button type="success light">success light</Button>
  </Row>
  <Row>
    <Button type="danger">danger</Button>
    <Button type="danger outlined">danger outlined</Button>
    <Button type="danger light">danger light</Button>
  </Row>
  <Row>
    <Button type="warning">warning</Button>
    <Button type="warning outlined">warning outlined</Button>
    <Button type="warning light">warning light</Button>
  </Row>
  <Row>
    <Button type="info">info</Button>
    <Button type="info outlined">info outlined</Button>
    <Button type="info light">info light</Button>
  </Row>
  <Row>
    <Button type="link">link</Button>
    <Button type="link light">link light</Button>
    <Button type="light">light</Button>
  </Row>
  <Row>
    <Button type="dark">dark</Button>
    <Button type="ghost">ghost</Button>
    <Button type="text">text</Button>
  </Row>
  <Row>
    <div class="container">
      <Col>
        <Button type="expanded primary ">
          This is a long button that extends to the limit of the container
        </Button>
        <Button type="expanded success outlined">
          This is a long button that extends to the limit of the container
        </Button>
        <Button type="expanded warning ">
          This is a long button that extends to the limit of the container
        </Button>
        <Button type="expanded danger outlined">
          This is a long button that extends to the limit of the container
        </Button>
      </Col>
    </div>
  </Row>
</Col>
<h3><a href="https://fonts.google.com/icons">Google Material Icons</a></h3>
<Icon icon="done" color="red" size={48} />
<Icon icon="person" color="blue" size={48} />
<Icon icon="home" color="green" size={48} />
<Icon icon="settings" color="yellow" size={48} />

<h3>Basic Flex Based Layout Component</h3>
<h4>Rows</h4>
<Row>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
</Row>
<h4>Columns</h4>
<Col>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
  <div
    style="height:50px;width:100px;border:1px solid gray;margin:10px;display:flex;justify-content:center;align-items:center"
  >
    Row Box
  </div>
</Col>

<style>
  .maman {
    display: flex;
    flex-flow: row wrap;
  }
  .container {
    width: 50%;
  }
</style>

<template>
    <div >
        <!-- <b-container fluid> -->
            <!-- <b-row > -->
            <b-navbar toggleable="md" type="dark" variant="dark">

            <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

            <b-navbar-brand href="#">Tessaract OCR</b-navbar-brand>

                        <b-collapse is-nav id="nav_collapse">

                            <!-- Right aligned nav items -->
                            <b-navbar-nav class="ml-auto">

                            <b-nav-item-dropdown right>
                                <!-- Using button-content slot -->
                                <template slot="button-content">
                                <em>User</em>
                                </template>
                                <b-dropdown-item href="#">Profile</b-dropdown-item>
                                <b-dropdown-item href="#">Signout</b-dropdown-item>
                            </b-nav-item-dropdown>
                            </b-navbar-nav>

                        </b-collapse>
        </b-navbar>
        <!-- <b-row> -->
    <!-- </b-container> -->
            <b-container class="bv-example-row" fluid>
                <b-row>
                    <b-col cols="2">
                        <b-nav toggleable="md" type="dark" variant="dark" vertical class="w-25">
                            <b-nav-item active>Active</b-nav-item>
                            <b-nav-item>Link</b-nav-item>
                            <b-nav-item>Another Link</b-nav-item>
                        </b-nav>
                    </b-col>
                    <b-col cols="1o">Welcome to TESSERACT OCR</b-col>
                </b-row>
            </b-container>
    </div>
        
</template>

<script>
export default {
  name: "Dashboard",
  data() {
    return {
      data: "dashboard data"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
a {
  color: #42b983;
}
</style>

<script>
import Layout from "../../../layouts/main.vue";
import PageHeader from "@/components/page-header";
import appConfig from "../../../../app.config";

export default {
  page: {
    title: "Product",
    meta: [{ name: "description", content: appConfig.description }],
  },
  data() {
    return {
      title: "Product",
      items: [
        {
          text: "Dashboards",
          href: "/",
        },
        {
          text: "Product",
          active: true,
        },
      ],
    }
  },
  components: {
    Layout,
    PageHeader,
  },
}
</script>

<template>
    <Layout>
        <PageHeader :title="title" :items="items" />

        <div class="row project-wrapper">
            <div class="col-xxl-8">
                <div class="row">
                    <div class="col-xl-4">
                        
                    </div>
                    <div class="col-xl-4">
                        
                    </div>
                </div>
                <div class="row">
                    <div class="col-xl-12">
                    </div>
                </div>
            </div>

            <div class="col-xxl-4">
                <Schedules />
            </div>
        </div>


        <div class="row">
            <div class="col-xxl-4">

            </div>  
            <div class="col-xxl-4 col-lg-6">

            </div>
            <div class="col-xxl-4 col-lg-6">

            </div>
        </div>

    </Layout>
</template>
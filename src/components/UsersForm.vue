<template>
  <template>
    <!-- Card -->
    <mdb-card>
      <mdb-card-body>
        <form>
          <p class="h4 text-center py-4">Step 1 - User Information</p>
          <div class="grey-text">
            <p class="h4 text-center py-4">User</p>

            <mdb-input label="First name" icon="user" group type="text" validate error="wrong" success="right"/>
            <mdb-input label="Last name" icon="user" group type="text" validate error="wrong" success="right"/>
            <mdb-input label="Preferred Language" icon="user" group type="text" validate error="wrong" success="right"/>
            <mdb-input label="User Type" icon="user" group type="text" validate error="wrong" success="right"/>


            <p class="h4 text-center py-4">Contact Information</p>

            <mdb-input label="Email"  group type="email" validate error="wrong" success="right"/>
            <mdb-input label="Phone Number"  group type="phone" validate error="wrong" success="right"/>
            <mdb-input label="Phone Extension"  group type="phone" validate error="wrong" success="right"/>
            <mdb-input label="Mobile Number"  group type="phone" validate error="wrong" success="right"/>

            <p class="h4 text-center py-4">Address</p>

            <mdb-input label="Street Number"  group type="number" validate error="wrong" success="right"/>
            <mdb-input label="Street Name"  group type="text" validate error="wrong" success="right"/>
            <mdb-input label="City"  group type="text" validate error="wrong" success="right"/>
            <mdb-input label="Province"  group type="text" validate error="wrong" success="right"/>
            <mdb-input label="Country"  group type="text" validate error="wrong" success="right"/>
            <mdb-input label="Postal Code"  group type="text" validate error="wrong" success="right"/>

          </div>
          <div class="text-center py-4 mt-3">
            <mdb-btn color="cyan" type="submit">Submit</mdb-btn>
          </div>
        </form>
      </mdb-card-body>
    </mdb-card>
    <!-- Card -->
  </template></template>
<script>
import { ref } from 'vue';

export default {
  name: 'App',
  setup() {
    // make users variable reactive with the ref() function
    const users = ref([

    ]);

    return {
      users
    };
  }
}
</script>
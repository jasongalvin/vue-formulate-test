<template>
  <formulate-form>
    <h2>Register</h2>
    <fieldset>
      <legend>Personal Details</legend>
 
      <formulate-input
        name="first"
        label="First name"
        help="What is your name?"
        validation="required"
        validation_name="First name"
      ></formulate-input>
      <formulate-input
        name="name"
        label="Last name"
        help="What is your name?"
        validation="required"
        validation_name="Last name"
      ></formulate-input>
    </fieldset>
    <fieldset>
      <legend>Account details</legend>
      <formulate-input
        name="username"
        label="Username"
        help="Select a username."
        validation="required"
      ></formulate-input>
      <formulate-input
        name="password"
        label="Password"
        help="Pick a password."
        validation="required|min:10,length"
      ></formulate-input>
      <formulate-input
        name="password_confirm"
        label="Password confirm"
        help="Re-type your password."
        validation="required|confirm"
        validation-name="Password confirmation"
      ></formulate-input>
    </fieldset>

    <formulate-input
      type="submit"
      label="Submit"
    ></formulate-input>
  </formulate-form>
</template>

<script>
export default {
  name: "RegisterTest",
  data () {
    return {
    }
  },
}
</script>

<style scoped>
fieldset {
  border: 0;
  margin-bottom: 2em;
  border-radius: .25em;
  border: 1px solid #e4e4e4;
}

legend {
  display: block;
}

.formulate-form {
  max-width: 500px;
  margin: 0 auto;
  padding: 1em;
  border-radius: .5em;
}
</style>


<template>
    

<div>test</div>


</template>
<script setup>
import { MailIcon, PhoneIcon, LocationMarkerIcon } from "@heroicons/vue/solid";
import { useForm } from "vee-validate";
const { handleSubmit } = useForm();
const send = handleSubmit((formValues) => {
    console.log(formValues);
});

</script>
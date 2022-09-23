<template>
    <div>
        <label
          :for="props.name"
          class="block mb-2 text-sm font-medium text-gray-900"
          >{{props.label}}</label
        >
        <input
          :type="props.type"
          :name="props.name"
          v-model="value"
          class="
            border border-gray-300
            text-gray-900
            sm:text-sm
            rounded-lg
            focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
            block
            w-full
            p-2.5
          "
          :placeholder="props.placeholder"
          
        />
        <div class="text-red-500 text-sm">
          
            {{errorMessage}}
          </div>
      </div>
      
</template>

<script setup>
import { useField } from 'vee-validate';

const props = defineProps({
    label: {
        type: String,
        required: true
    },
    type: {
        type: String,
        required: true
    },
    name: {
        type: String,
        required: true
    },
    rule: {
        type: String,
        required: true
    },
    placeholder: {
        type: String,
        required: true
    }
})


const { value, errorMessage } = useField(props.name, props.rule);
</script>


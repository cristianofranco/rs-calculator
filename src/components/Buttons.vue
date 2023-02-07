<template>
  <div class="grid grid-cols-4 gap-4 mt-6">
    <Button label="CE" isCE=true />
    <Button label="C" />
    <Button label="%" />
    <Button label="divide" isOperator=true iconPath="/divide.svg" />
    <Button label="7" />
    <Button label="8" />
    <Button label="9" />
    <Button label="multiply" isOperator=true iconPath="/multiply.svg"  />
    <Button label="4" />
    <Button label="5" />
    <Button label="6" />
    <Button label="minus" isOperator=true iconPath="/minus.svg"  />
    <Button label="1" />
    <Button label="2" />
    <Button label="3" />
    <Button label="plus" isOperator=true iconPath="/plus.svg"  />
    <Button label="plus-minus" iconPath="/plus-minus.svg"  />
    <Button label="0" />
    <Button label="," />
    <Button label="equals" isEquals="true" iconPath="/big-equals.svg" />
  </div>
</template>

<script>
import Button from './Button.vue'

export default {
  components: {
    Button
  },
};
</script>
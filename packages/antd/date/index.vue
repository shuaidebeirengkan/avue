<template>
  <div :class="b()">
    <a-date-picker :defaultValue="moment(text, format)"
                   :placeholder="placeholder"
                   :readonly="readonly"
                   :disabled="disabled"
                   :format="format"
                   @click.native="handleClick"
                   @change="handleChange"></a-date-picker>
  </div>
</template>

<script>
import create from "core/create";
import props from "../../core/common/props.js";
import event from "../../core/common/event.js";
export default create({
  name: "date",
  mixins: [props(), event()],
  data () {
    return {
      name: 'date',
    };
  },
  props: {
    valueFormat: {},
    format: {}
  },
  watch: {},
  created () { },
  mounted () { },
  methods: {}
});
</script>


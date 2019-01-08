<template>
    <div class="transaction-item-area flex items-center justify-between p-4 border-b-2 ">
        <div class="transaction-item-info max-w-md">
            <h4 class="mb-2">
                    {{item.title}}
            </h4>
            <p class="text-xs text-grey-darker">
                summary info goes here Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ipsa iusto qui quos soluta neque voluptates, dolorum corrupti atque dolorem? Veritatis, praesentium fugit? Molestias, sint facere. Quos iusto voluptatibus eius.
            </p>
        </div>
        <div class="transaction-more-details">
            <button class="btn-tertiary">Details</button>
        </div>
    </div>
</template>

<script>
export default {
  props: {
    item: {
      type: Object,
      required: true
    }
  }
}
</script>



<template>
    <ul class="list-reset">
        <li>
            <div class="transaction-item-area flex items-center justify-between p-4 border-b-2 ">
            <div class="transaction-item-info max-w-md">
                <h4 class="mb-2 font-normal">
                    <slot name="transaction-title">Default Transaction item title</slot>
                </h4>
                <p class="text-xs text-grey-darker">
                    <slot name="transaction-info">
                    summary info goes here Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ipsa iusto qui quos soluta neque voluptates, dolorum corrupti atque dolorem? Veritatis, praesentium fugit? Molestias, sint facere. Quos iusto voluptatibus eius.
                    </slot>
                </p>
            </div>
            <div class="transaction-more-details">
                <button class="border-none bg-none">Details</button>
            </div>
        </div>
    </li>
    </ul>
</template>

<script>
export default {
    data: {
    items: [
      { message: 'Foo' },
      { message: 'Bar' }
    ]
  }
}
</script>


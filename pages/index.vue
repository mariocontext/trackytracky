<template>
  <div class="nuxt-holding-element">
    <header
      class="sticky flex justify-between items-center w-full pin-t bg-grey-light p-4"
    >
      <!--
        We may want the header to disappear when content is scrolled down and reappear when scrolled up
      -->
      <span> <i class="text-4xl material-icons">menu</i> </span>
      <span><h1 class="text-lg pl-2">title goes here</h1></span>
      <span><i class="material-icons">more_vert</i></span>
    </header>
    <main class="container mx-auto m-4 p-4">
      <h2 class="text-xl">Secondary title</h2>
      <p class="text-sm bg-grey-light">
        Lorem ipsum dolor s it amet consectetur adipisicing elit. Et eligendi
        molestiae numquam eveniet, animi libero sint necessitatibus nemo
        perferendis aspernatur? Expedita ducimus officia iure libero. Dicta
        officiis minus tenetur neque.
      </p>
      <button class="btn btn-primary">Hello World</button>
<!-- Learn about this code on MDN: https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Your_first_HTML_form -->

        <form action="/my-handling-form-page" method="post">
          <div>
            <label for="name">Name:</label>
            <input class="bg-grey-lighter border border-black border-b block leading-loose px-4 text-grey-darkest mb-4" type="text" id="name" name="user_name">
          </div>

          <div>
            <label for="mail">E-mail:</label>
            <input class="border border-grey" type="email" id="mail" name="user_email">
          </div>

          <div>
            <label for="msg">Message:</label>
            <textarea class="border border-grey" id="msg" name="user_message"></textarea>
          </div>
         
          <div class="button">
            <button class="btn btn-primary" type="submit">Send your message</button>
          </div>
        </form>
    </main>
    <footer class="fixed w-full pin-b bg-grey-light p-4">
      <p class="text-center">footer goes here</p>
    </footer>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.btn {
  @apply bg-secondary rounded p-4 text-green;
}

.btn:hover {
  @apply text-blue text-lg;
}

.btn-primary {
  @apply bg-primary;
}

@screen md {

  .btn-primary {
    @apply bg-purple text-white;
  }
  
}

.links {
  @apply text-center;
}

</style>

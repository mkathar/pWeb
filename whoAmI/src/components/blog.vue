<template>
  <div class="blog">
    <span class="blog__ques">Recent Posts?</span>
    <h1 class="blog__title">Blog</h1>
    <div class="blog__content">
      <img
        class="blog__content__img"
        src="https://picsum.photos/id/237/350/350"
        alt=""
      />

      <div class="blog__content__group">
        <h4 class="blog__content__group__title">
          Consectetur adipisicing elit
        </h4>
        <div class="blog__content__group__response">
          <span class="blog__content__group__by">By:</span>
          <span class="blog__content__group__user">Admin</span>
          <div class="blog__content__group__response__like">
            <span><Icon name="heart" :size="16" /></span>
            <span class="blog__content__group__response__like__number"
              >989</span
            >
          </div>
          <div class="blog__content__group__response__commit">
            <span><Icon name="comment" :size="16" /></span>
            <span class="blog__content__group__response__commit__number"
              >154</span
            >
          </div>
        </div>
        <div class="blog__content__paragraph__group">
          <p class="blog__content__paragraph">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet
            nesciunt qui sit velit delectus voluptates, repellat ipsum culpa id
            deleniti. Rerum debitis facilis accusantium neque numquam mollitia
            modi quasi distinctio.
          </p>
          <p class="blog__content__emphasize">
            Necessitatibus nihil impedit! Ex nisi eveniet, dolor aliquid
            consequuntur repudiandae.
          </p>
          <p class="blog__content__paragraph">
            Magnam in repellat enim harum omnis aperiam! Explicabo illo,
            commodi, dolor blanditiis cupiditate harum nisi vero accusamus
            laudantium voluptatibus dolores quae obcaecati.
          </p>
          <a class="blog__content__link" href=""
            >Read more <span><Icon name="next" :size="12" /></span
          ></a>
        </div>
      </div>
    </div>
    <div class="blog__content">
      <img
        class="blog__content__img"
        src="https://picsum.photos/id/237/350/350"
        alt=""
      />

      <div class="blog__content__group">
        <h4 class="blog__content__group__title">
          Consectetur adipisicing elit
        </h4>
        <div class="blog__content__group__response">
          <span class="blog__content__group__by">By:</span>
          <span class="blog__content__group__user">Admin</span>
          <div class="blog__content__group__response__like">
            <span><Icon name="heart" :size="16" /></span>
            <span class="blog__content__group__response__like__number"
              >989</span
            >
          </div>
          <div class="blog__content__group__response__commit">
            <span><Icon name="comment" :size="16" /></span>
            <span class="blog__content__group__response__commit__number"
              >154</span
            >
          </div>
        </div>
        <div class="blog__content__paragraph__group">
          <p class="blog__content__paragraph">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet
            nesciunt qui sit velit delectus voluptates, repellat ipsum culpa id
            deleniti. Rerum debitis facilis accusantium neque numquam mollitia
            modi quasi distinctio.
          </p>
          <p class="blog__content__emphasize">
            Necessitatibus nihil impedit! Ex nisi eveniet, dolor aliquid
            consequuntur repudiandae.
          </p>
          <p class="blog__content__paragraph">
            Magnam in repellat enim harum omnis aperiam! Explicabo illo,
            commodi, dolor blanditiis cupiditate harum nisi vero accusamus
            laudantium voluptatibus dolores quae obcaecati.
          </p>
          <a class="blog__content__link" href=""
            >Read more <span><Icon name="next" :size="12" /></span
          ></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Icon } from "../icons.jsx";
export default {
  data() {
    return {};
  },
  components: { Icon },
};
</script>

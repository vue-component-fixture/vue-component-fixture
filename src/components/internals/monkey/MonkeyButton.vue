<template>
  <button class="monkey-button" :class="{ 'monkey-activated': activated }">
    <div class="monkey-root">
      <svg
        version="1.1"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        x="0px"
        y="0px"
        viewBox="0 -5 100 100"
        xml:space="preserve"
        transform="scale(0.8)"
        class="ready"
      >
        <g>
          <circle cx="40.374" cy="37.662" r="5.885" />
          <circle cx="59.628" cy="37.662" r="5.885" />
          <g>
            <path
              d="M86.31,25.354c-0.984,0-1.941,0.108-2.867,0.306C76.075,15.105,63.849,8.195,50,8.195
			c-13.847,0-26.075,6.912-33.441,17.466c-0.925-0.198-1.883-0.306-2.866-0.306c-7.562,0-13.691,6.129-13.691,13.689
			c0,6.046,3.924,11.167,9.361,12.981C10.93,73.105,28.519,89.725,50,89.725c21.482,0,39.071-16.619,40.641-37.7
			c5.437-1.814,9.361-6.935,9.361-12.981C100,31.483,93.87,25.354,86.31,25.354z M10.042,45.449c-3.332,0-6.033-2.701-6.033-6.034
			c0-3.332,2.701-6.033,6.033-6.033c3.333,0,6.034,2.702,6.034,6.033C16.076,42.749,13.375,45.449,10.042,45.449z M50,83.465
			c-14.44,0-26.544-7.747-29.805-18.175c6.848,3.496,17.722,5.651,29.804,5.651c12.083,0,22.958-2.155,29.806-5.651
			C76.544,75.718,64.441,83.465,50,83.465z M80.664,60.055c-4.868,3.614-16.003,6.84-30.665,6.84
			c-14.659,0-25.796-3.226-30.663-6.839c-0.002-0.132-0.013-0.263-0.013-0.396c0-5.861,2.734-11.225,7.261-15.373
			c-1.683-2.343-2.683-5.21-2.683-8.315c0-7.893,6.397-14.291,14.29-14.291c4.907,0,9.235,2.476,11.808,6.244
			c2.573-3.768,6.899-6.244,11.808-6.244c7.894,0,14.291,6.398,14.291,14.291c0,3.105-1.001,5.972-2.683,8.315
			c4.526,4.148,7.261,9.511,7.261,15.373C80.676,59.792,80.666,59.924,80.664,60.055z M89.958,45.449
			c-3.334,0-6.033-2.701-6.033-6.034c0-3.332,2.699-6.033,6.033-6.033c3.331,0,6.033,2.702,6.033,6.033
			C95.991,42.749,93.289,45.449,89.958,45.449z"
            />
          </g>
        </g>
      </svg>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        version="1.1"
        x="0px"
        y="0px"
        viewBox="0 0 100 100"
        enable-background="new 0 0 100 100"
        xml:space="preserve"
        class="on-fire"
      >
        <g>
          <g>
            <circle fill="none" cx="39.514" cy="59.696" r="2.978" />
            <path
              fill="none"
              d="M49.607,91.029c6.17,0,11.199-4.92,11.401-11.042H38.206C38.408,86.108,43.438,91.029,49.607,91.029z"
            />
            <path
              fill="none"
              d="M59.535,48.166c-3.205,0-6.288,1.373-8.456,3.767l-1.472,1.625l-1.472-1.625    c-2.169-2.394-5.251-3.767-8.456-3.767c-6.297,0-11.42,5.123-11.42,11.42c0,5.751,4.302,10.619,10.008,11.323l2.987,0.368    l-1.514,2.601c-0.417,0.716-0.731,1.478-0.982,2.258h21.699c-0.252-0.78-0.566-1.542-0.982-2.258l-1.514-2.601l2.987-0.368    c5.706-0.704,10.008-5.571,10.008-11.323C70.956,53.289,65.833,48.166,59.535,48.166z M39.514,66.645    c-3.832,0-6.95-3.118-6.95-6.95c0-3.832,3.118-6.949,6.95-6.949c3.832,0,6.949,3.117,6.949,6.949    C46.464,63.527,43.346,66.645,39.514,66.645z M46.257,70.285c-0.912,0-1.655-0.743-1.655-1.655c0-0.912,0.743-1.655,1.655-1.655    c0.912,0,1.654,0.743,1.654,1.655C47.911,69.543,47.169,70.285,46.257,70.285z M52.958,70.285c-0.912,0-1.655-0.743-1.655-1.655    c0-0.912,0.743-1.655,1.655-1.655c0.912,0,1.655,0.743,1.655,1.655C54.613,69.543,53.87,70.285,52.958,70.285z M59.701,66.314    c-3.832,0-6.95-3.118-6.95-6.95c0-3.832,3.118-6.949,6.95-6.949c3.832,0,6.95,3.117,6.95,6.949    C66.65,63.196,63.532,66.314,59.701,66.314z"
            />
            <circle fill="none" cx="59.701" cy="59.365" r="2.978" />
            <path
              d="M84.766,37.437c-0.448,0.588-0.933,1.138-1.451,1.645l-3.09,3.019l-0.346-4.307c-0.781-9.713-5.156-19.06-11.599-25.035    c-1.397,2.954-2.994,5.781-4.767,8.433l-2.348,3.513l-1.27-4.031C57.973,14.571,54.646,9.095,50.411,5    c-2.594,4.964-5.535,9.695-8.763,14.096l-3.079,4.198l-1.205-10.941c-7.172,6.453-12.88,15.279-16.255,25.223l-1.301,3.835    l-2.289-3.34c-0.897-1.308-1.561-2.821-1.974-4.423c-3.861,7.728-5.428,17.192-4.133,26.033    c1.122,7.663,5.209,13.749,12.147,18.091c3.275,2.049,6.992,3.59,10.931,4.683c0.304,1.619,0.855,3.15,1.625,4.548    C38.735,91.764,43.799,95,49.607,95c5.517,0,10.351-2.927,13.069-7.301c0.843-1.356,1.478-2.849,1.868-4.441    c1.917-0.391,3.751-0.858,5.461-1.4c12.318-3.907,23.061-16.495,17.543-34.9C86.773,44.374,85.65,40.5,84.766,37.437z     M49.607,91.029c-6.17,0-11.199-4.92-11.401-11.042h22.803C60.806,86.108,55.777,91.029,49.607,91.029z M60.947,70.909    l-2.987,0.368l1.514,2.601c0.417,0.716,0.731,1.478,0.982,2.258H38.758c0.252-0.78,0.566-1.542,0.982-2.258l1.514-2.601    l-2.987-0.368c-5.706-0.704-10.008-5.571-10.008-11.323c0-6.297,5.123-11.42,11.42-11.42c3.205,0,6.288,1.373,8.456,3.767    l1.472,1.625l1.472-1.625c2.169-2.394,5.251-3.767,8.456-3.767c6.297,0,11.42,5.123,11.42,11.42    C70.956,65.338,66.653,70.205,60.947,70.909z"
            />
            <circle cx="46.257" cy="68.63" r="1.655" />
            <circle cx="52.958" cy="68.63" r="1.655" />
            <path
              d="M39.514,52.746c-3.832,0-6.95,3.117-6.95,6.949c0,3.832,3.118,6.95,6.95,6.95c3.832,0,6.949-3.118,6.949-6.95    C46.464,55.863,43.346,52.746,39.514,52.746z M39.514,62.674c-1.642,0-2.978-1.336-2.978-2.978c0-1.642,1.336-2.978,2.978-2.978    s2.978,1.336,2.978,2.978C42.492,61.337,41.156,62.674,39.514,62.674z"
            />
            <path
              d="M59.701,52.415c-3.832,0-6.95,3.117-6.95,6.949c0,3.832,3.118,6.95,6.95,6.95c3.832,0,6.95-3.118,6.95-6.95    C66.65,55.533,63.532,52.415,59.701,52.415z M59.701,62.343c-1.642,0-2.978-1.336-2.978-2.978c0-1.642,1.336-2.978,2.978-2.978    s2.978,1.336,2.978,2.978C62.679,61.007,61.343,62.343,59.701,62.343z"
            />
          </g>
        </g>
      </svg>
      <div>
        Run
      </div>
    </div>
  </button>
</template>
<script>
export default {
  name: "monkey-button",
  props: {
    activated: {
      type: Boolean,
      default: false
    }
  }
};
</script>
<style lang="less" scoped>
@button-color: black;
@button-color-hover: red;
@button-size: 44px;
@button-svg-size: 40px;

button.monkey-button {
  padding: 0;
  border: 0;
  border-radius: 40px;
  box-shadow: 0;
  background: lightgreen;

  .monkey-root {
    display: flex;
    align-items: center;
    text-transform: uppercase;
    font-size: 16px;
    font-weight: bold;
    padding: 2px 10px 2px 2px;
  }

  &:focus {
    outline: 0;
  }
  svg {
    fill: @button-color;
    width: @button-svg-size;
    height: @button-svg-size;

    &.on-fire {
      display: none;
    }
    &.ready {
      display: inline;
    }

    &:hover {
      fill: @button-color-hover;
    }
  }
  &:hover {
    color: @button-color-hover;
    svg {
      fill: @button-color-hover;
      &.on-fire {
        display: inline;
      }
      &.ready {
        display: none;
      }
    }
  }

  &:active {
    svg {
      fill: red;
      &.on-fire {
        display: inline;
      }
      &.ready {
        display: none;
      }
    }
  }

  &.monkey-activated {
    svg {
      fill: @button-color-hover;
      &.on-fire {
        display: inline;
      }
      &.ready {
        display: none;
      }
    }
  }
}
</style>

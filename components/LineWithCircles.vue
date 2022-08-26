<template>
  <div>
    <div class="circle bg-text-button" />
    <div class="circle bg-text-button" />
    <div class="circle bg-text-button" />
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.circle {
  position: relative;
  border-radius: 100%;
  width: 2.4em;
  padding: 1.3em 0;
  line-height: 50px;
  text-align: center;
  margin-top: 12.5rem;
  background-color: #fff;
  z-index: 2;

  &::before{
    position: absolute;
    width: .1px;
    background-color: var(--text-color-primary);
    height: 12.5em;
    display: block;
    content: '';
    left: 50%;
    z-index: 1;
    top: -12.5em;
    margin-left: -1px;
  }
  &:first-child{
    margin-top: 0 !important;
  }
  &:first-child::before{
    height: 2.8125rem;
    top: -2.8125rem;
  }
  &:last-child::after{
    position: absolute;
    width: .1px;
    background-color: var(--text-color-primary);
    height: 2.8125rem;
    display: block;
    content: '';
    left: 50%;
    z-index: 1;
    bottom: -2.8125rem;
    margin-left: -1px;
  }
}

@media only screen and (max-width: 1400px) {
  .circle{
    margin-top: 14rem !important;

    &::before{
      height: 14em !important;
      top: -14em !important;
    }
    &:first-child::before{
      height: 2.8125rem !important;
      top: -2.8125rem !important;
    }
  }
}
@media only screen and (max-width: 1285px) {
  .circle{
    margin-top: 12.5rem !important;

    &::before{
      height: 12.5em !important;
      top: -12.5em !important;
    }
    &:first-child::before{
      height: 2.8125rem !important;
      top: -2.8125rem !important;
    }
  }
}
@media only screen and (max-width: 1210px) {
  .circle{
    margin-top: 14.5rem !important;

    &::before{
      height: 14.5em !important;
      top: -14.5em !important;
    }
    &:first-child::before{
      height: 2.8125rem !important;
      top: -2.8125rem !important;
    }
  }
}
@media only screen and (max-width: 1028px) {
  .circle{
    margin-top: 16rem !important;

    &::before{
      height: 16em !important;
      top: -16em !important;
    }
  }
}
@media only screen and (max-width: 875px) {
  .circle{
    margin-top: 18rem !important;

    &::before{
      height: 18em !important;
      top: -18em !important;
    }
  }
}
@media only screen and (max-width: 830px) {
  .circle{
    margin-top: 20rem !important;

    &::before{
      height: 20em !important;
      top: -20em !important;
    }
  }
}
@media only screen and (max-width: 800px) {
  .circle{
    margin-top: 12em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 12em !important;
      top: -12em !important;
    }
  }
}
@media only screen and (max-width: 646px) {
  .circle{
    margin-top: 14em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 14em !important;
      top: -14em !important;
    }
  }
}
@media only screen and (max-width: 592px) {
  .circle{
    margin-top: 16em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 16em !important;
      top: -16em !important;
    }
  }
}
@media only screen and (max-width: 517px) {
  .circle{
    margin-top: 17em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 17em !important;
      top: -17em !important;
    }
  }
}
@media only screen and (max-width: 463px) {
  .circle{
    margin-top: 18em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 18em !important;
      top: -18em !important;
    }
  }
}
@media only screen and (max-width: 440px) {
  .circle{
    margin-top: 22em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 22em !important;
      top: -22em !important;
    }
  }
}
@media only screen and (max-width: 370px) {
  .circle{
    margin-top: 25em !important;

    &:first-child {
      background: url('/skills-images/backend.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:nth-child(2) {
      background: url('/skills-images/databases.svg') center no-repeat;
      background-size: 25px 25px;
    }
    &:last-child {
      background: url('/skills-images/frontend.svg') center no-repeat;
      background-size: 25px 25px;
    }

    &::before{
      height: 25em !important;
      top: -25em !important;
    }
  }
}
</style>

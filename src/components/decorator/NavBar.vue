<template lang="pug">
  nav#navbar-main.navbar.navbar-top.navbar-expand-md.navbar-dark
    .container-fluid
      // Brand
      a.h4.mb-0.text-white.text-uppercase.d-none.d-lg-inline-block(href='./index.html') Dashboard
      // Form
      form.navbar-search.navbar-search-dark.form-inline.mr-3.d-none.d-md-flex.ml-lg-auto
        .form-group.mb-0
          .input-group.input-group-alternative
            .input-group-prepend
              span.input-group-text
                i.fas.fa-search
            input.form-control(placeholder='Search', type='text')
      // User
      ul.navbar-nav.align-items-center.d-none.d-md-flex
        li.nav-item.dropdown
          a.nav-link.pr-0(href='#', role='button', data-toggle='dropdown', aria-haspopup='true', aria-expanded='false')
            .media.align-items-center
              span.avatar.avatar-sm.rounded-circle
                img(alt='Image placeholder', src='/img/theme/team-4-800x800.jpg')
              .media-body.ml-2.d-none.d-lg-block
                span.mb-0.text-sm.font-weight-bold Jessica Jones
          .dropdown-menu.dropdown-menu-arrow.dropdown-menu-right
            .dropdown-header.noti-title
              h6.text-overflow.m-0 Welcome!
            a.dropdown-item(href='./examples/profile.html')
              i.ni.ni-single-02
              span My profile
            a.dropdown-item(href='./examples/profile.html')
              i.ni.ni-settings-gear-65
              span Settings
            a.dropdown-item(href='./examples/profile.html')
              i.ni.ni-calendar-grid-58
              span Activity
            a.dropdown-item(href='./examples/profile.html')
              i.ni.ni-support-16
              span Support
            .dropdown-divider
            a.dropdown-item(href='#!')
              i.ni.ni-user-run
              span Logout
</template>

<script>
export default {
  name: "f-nav-bar",
  data() {
    return {
      msg: "teste"
    };
  }
};
</script>

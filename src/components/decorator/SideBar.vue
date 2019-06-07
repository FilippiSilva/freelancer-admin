<template lang="pug">
  nav#sidenav-main.navbar.navbar-vertical.fixed-left.navbar-expand-md.navbar-light.bg-white
    .container-fluid
      // Toggler
      button.navbar-toggler(type='button', data-toggle='collapse', data-target='#sidenav-collapse-main', aria-controls='sidenav-main', aria-expanded='false', aria-label='Toggle navigation')
        span.navbar-toggler-icon
      // Brand
      a.navbar-brand.pt-0(href='./index.html')
        img.navbar-brand-img(src='/img/brand/blue.png', alt='...')
      // User
      ul.nav.align-items-center.d-md-none
        li.nav-item.dropdown
          a.nav-link.nav-link-icon(href='#', role='button', data-toggle='dropdown', aria-haspopup='true', aria-expanded='false')
            i.ni.ni-bell-55
          .dropdown-menu.dropdown-menu-arrow.dropdown-menu-right(aria-labelledby='navbar-default_dropdown_1')
            a.dropdown-item(href='#') Action
            a.dropdown-item(href='#') Another action
            .dropdown-divider
            a.dropdown-item(href='#') Something else here
        li.nav-item.dropdown
          a.nav-link(href='#', role='button', data-toggle='dropdown', aria-haspopup='true', aria-expanded='false')
            .media.align-items-center
              span.avatar.avatar-sm.rounded-circle
                img(alt='Image placeholder', src='/img/theme/team-1-800x800.jpg')
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
      // Collapse
      #sidenav-collapse-main.collapse.navbar-collapse
        // Collapse header
        .navbar-collapse-header.d-md-none
          .row
            .col-6.collapse-brand
              a(href='./index.html')
                img(src='/img/brand/blue.png')
            .col-6.collapse-close
              button.navbar-toggler(type='button', data-toggle='collapse', data-target='#sidenav-collapse-main', aria-controls='sidenav-main', aria-expanded='false', aria-label='Toggle sidenav')
                span
                span
        // Form
        form.mt-4.mb-3.d-md-none
          .input-group.input-group-rounded.input-group-merge
            input.form-control.form-control-rounded.form-control-prepended(type='search', placeholder='Search', aria-label='Search')
            .input-group-prepend
              .input-group-text
                span.fa.fa-search
        // Navigation
        ul.navbar-nav
          li.nav-item
            router-link.nav-link(to='/' active-class='active')
              i.fas.fa-tachometer-alt
              //- i.ni.ni-tv-2.text-primary
              |  Dashboard
</template>

<script>
export default {
  name: "f-sidebar",
  data() {
    return {
      msg: "f-sidebar"
    };
  }
};
</script>

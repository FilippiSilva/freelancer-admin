<template lang="pug">
  div
    // Sidenav
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
              a.nav-link(href='./index.html')
                i.fas.fa-tachometer-alt
                //- i.ni.ni-tv-2.text-primary
                |  Dashboard
    // Main content
    .main-content
      // Top navbar
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
      // Header
      .header.bg-gradient-primary.pb-8.pt-5.pt-md-8
        .container-fluid
          .header-body
            // Card stats
            .row
              .col-xl-3.col-lg-6
                .card.card-stats.mb-4.mb-xl-0
                  .card-body
                    .row
                      .col
                        h5.card-title.text-uppercase.text-muted.mb-0 Traffic
                        span.h2.font-weight-bold.mb-0 350,897
                      .col-auto
                        .icon.icon-shape.bg-danger.text-white.rounded-circle.shadow
                          i.fas.fa-chart-bar
                    p.mt-3.mb-0.text-muted.text-sm
                      span.text-success.mr-2
                        i.fa.fa-arrow-up
                        |  3.48%
                      span.text-nowrap Since last month
              .col-xl-3.col-lg-6
                .card.card-stats.mb-4.mb-xl-0
                  .card-body
                    .row
                      .col
                        h5.card-title.text-uppercase.text-muted.mb-0 New users
                        span.h2.font-weight-bold.mb-0 2,356
                      .col-auto
                        .icon.icon-shape.bg-warning.text-white.rounded-circle.shadow
                          i.fas.fa-chart-pie
                    p.mt-3.mb-0.text-muted.text-sm
                      span.text-danger.mr-2
                        i.fas.fa-arrow-down
                        |  3.48%
                      span.text-nowrap Since last week
              .col-xl-3.col-lg-6
                .card.card-stats.mb-4.mb-xl-0
                  .card-body
                    .row
                      .col
                        h5.card-title.text-uppercase.text-muted.mb-0 Sales
                        span.h2.font-weight-bold.mb-0 924
                      .col-auto
                        .icon.icon-shape.bg-yellow.text-white.rounded-circle.shadow
                          i.fas.fa-users
                    p.mt-3.mb-0.text-muted.text-sm
                      span.text-warning.mr-2
                        i.fas.fa-arrow-down
                        |  1.10%
                      span.text-nowrap Since yesterday
              .col-xl-3.col-lg-6
                .card.card-stats.mb-4.mb-xl-0
                  .card-body
                    .row
                      .col
                        h5.card-title.text-uppercase.text-muted.mb-0 Performance
                        span.h2.font-weight-bold.mb-0 49,65%
                      .col-auto
                        .icon.icon-shape.bg-info.text-white.rounded-circle.shadow
                          i.fas.fa-percent
                    p.mt-3.mb-0.text-muted.text-sm
                      span.text-success.mr-2
                        i.fas.fa-arrow-up
                        |  12%
                      span.text-nowrap Since last month
      // Page content
      .container-fluid.mt--7
        .row
          .col-xl-8.mb-5.mb-xl-0
            .card.bg-gradient-default.shadow
              .card-header.bg-transparent
                .row.align-items-center
                  .col
                    h6.text-uppercase.text-light.ls-1.mb-1 Overview
                    h2.text-white.mb-0 Sales value
                  .col
                    ul.nav.nav-pills.justify-content-end
                      li.nav-item.mr-2.mr-md-0(data-toggle='chart', data-target='#chart-sales', data-update='{"data":{"datasets":[{"data":[0, 20, 10, 30, 15, 40, 20, 60, 60]}]}}', data-prefix='$', data-suffix='k')
                        a.nav-link.py-2.px-3.active(href='#', data-toggle='tab')
                          span.d-none.d-md-block Month
                          span.d-md-none M
                      li.nav-item(data-toggle='chart', data-target='#chart-sales', data-update='{"data":{"datasets":[{"data":[0, 20, 5, 25, 10, 30, 15, 40, 40]}]}}', data-prefix='$', data-suffix='k')
                        a.nav-link.py-2.px-3(href='#', data-toggle='tab')
                          span.d-none.d-md-block Week
                          span.d-md-none W
              .card-body
                // Chart
                .chart
                  // Chart wrapper
                  canvas#chart-sales.chart-canvas
          .col-xl-4
            .card.shadow
              .card-header.bg-transparent
                .row.align-items-center
                  .col
                    h6.text-uppercase.text-muted.ls-1.mb-1 Performance
                    h2.mb-0 Total orders
              .card-body
                // Chart
                .chart
                  canvas#chart-orders.chart-canvas
        .row.mt-5
          .col-xl-8.mb-5.mb-xl-0
            .card.shadow
              .card-header.border-0
                .row.align-items-center
                  .col
                    h3.mb-0 Page visits
                  .col.text-right
                    a.btn.btn-sm.btn-primary(href='#!') See all
              .table-responsive
                // Projects table
                table.table.align-items-center.table-flush
                  thead.thead-light
                    tr
                      th(scope='col') Page name
                      th(scope='col') Visitors
                      th(scope='col') Unique users
                      th(scope='col') Bounce rate
                  tbody
                    tr
                      th(scope='row')
                        | /argon/
                      td
                        | 4,569
                      td
                        | 340
                      td
                        i.fas.fa-arrow-up.text-success.mr-3
                        |  46,53%
                    tr
                      th(scope='row')
                        | /argon/index.html
                      td
                        | 3,985
                      td
                        | 319
                      td
                        i.fas.fa-arrow-down.text-warning.mr-3
                        |  46,53%
                    tr
                      th(scope='row')
                        | /argon/charts.html
                      td
                        | 3,513
                      td
                        | 294
                      td
                        i.fas.fa-arrow-down.text-warning.mr-3
                        |  36,49%
                    tr
                      th(scope='row')
                        | /argon/tables.html
                      td
                        | 2,050
                      td
                        | 147
                      td
                        i.fas.fa-arrow-up.text-success.mr-3
                        |  50,87%
                    tr
                      th(scope='row')
                        | /argon/profile.html
                      td
                        | 1,795
                      td
                        | 190
                      td
                        i.fas.fa-arrow-down.text-danger.mr-3
                        |  46,53%
          .col-xl-4
            .card.shadow
              .card-header.border-0
                .row.align-items-center
                  .col
                    h3.mb-0 Social traffic
                  .col.text-right
                    a.btn.btn-sm.btn-primary(href='#!') See all
              .table-responsive
                // Projects table
                table.table.align-items-center.table-flush
                  thead.thead-light
                    tr
                      th(scope='col') Referral
                      th(scope='col') Visitors
                      th(scope='col')
                  tbody
                    tr
                      th(scope='row')
                        | Facebook
                      td
                        | 1,480
                      td
                        .d-flex.align-items-center
                          span.mr-2 60%
                          div
                            .progress
                              .progress-bar.bg-gradient-danger(role='progressbar', aria-valuenow='60', aria-valuemin='0', aria-valuemax='100', style='width: 60%;')
                    tr
                      th(scope='row')
                        | Facebook
                      td
                        | 5,480
                      td
                        .d-flex.align-items-center
                          span.mr-2 70%
                          div
                            .progress
                              .progress-bar.bg-gradient-success(role='progressbar', aria-valuenow='70', aria-valuemin='0', aria-valuemax='100', style='width: 70%;')
                    tr
                      th(scope='row')
                        | Google
                      td
                        | 4,807
                      td
                        .d-flex.align-items-center
                          span.mr-2 80%
                          div
                            .progress
                              .progress-bar.bg-gradient-primary(role='progressbar', aria-valuenow='80', aria-valuemin='0', aria-valuemax='100', style='width: 80%;')
                    tr
                      th(scope='row')
                        | Instagram
                      td
                        | 3,678
                      td
                        .d-flex.align-items-center
                          span.mr-2 75%
                          div
                            .progress
                              .progress-bar.bg-gradient-info(role='progressbar', aria-valuenow='75', aria-valuemin='0', aria-valuemax='100', style='width: 75%;')
                    tr
                      th(scope='row')
                        | twitter
                      td
                        | 2,645
                      td
                        .d-flex.align-items-center
                          span.mr-2 30%
                          div
                            .progress
                              .progress-bar.bg-gradient-warning(role='progressbar', aria-valuenow='30', aria-valuemin='0', aria-valuemax='100', style='width: 30%;')
        // Footer
        footer.footer
          .row.align-items-center.justify-content-xl-between
            .col-xl-6
              .copyright.text-center.text-xl-left.text-muted
                | © 2018 
                a.font-weight-bold.ml-1(href='https://www.creative-tim.com', target='_blank') Creative Tim
            .col-xl-6
              ul.nav.nav-footer.justify-content-center.justify-content-xl-end
                li.nav-item
                  a.nav-link(href='https://www.creative-tim.com', target='_blank') Creative Tim
                li.nav-item
                  a.nav-link(href='https://www.creative-tim.com/presentation', target='_blank') About Us
                li.nav-item
                  a.nav-link(href='http://blog.creative-tim.com', target='_blank') Blog
                li.nav-item
                  a.nav-link(href='https://github.com/creativetimofficial/argon-dashboard/blob/master/LICENSE.md', target='_blank') MIT License
</template>

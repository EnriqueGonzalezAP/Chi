<template lang="pug">
  div
    h2 chi-date-picker
    <PropertiesGenerator tag="chi-date-picker" />
    h2 chi-date
    <PropertiesGenerator tag="chi-date" />
    h2 JavaScript
    p.-text This component accepts options to configure its behavior.

    section.chi-table.chi-table__options.-bordered.-my--3
      div
        table.-text(cellpadding='0', cellspacing='0')
          thead
            tr
              th
                div Option
              th
                div Default
              th
                div Description
          tbody
            tr
              td
                div
                  code= 'date'
              td
                div
                  code= 'null'
              td
                div
                  | Sets the initial date into the date picker. Overrides the value of the input.
            tr
              td
                div
                  code= 'locale'
              td
                div
                  code 'en'
              td
                div
                  | Sets the locale for names of months and days of the week. The locales supported are the ones supported
                  | by Day.js. <strong>Locales must be imported before using them</strong>.
                  | <a href="https://github.com/iamkun/dayjs/tree/dev/src/locale">List of supported locales</a>.
            tr
              td
                div
                  code= 'min'
              td
                div
                  code '01/01/1900'
              td
                div
                  | Prevent user pick a date before the configured.
            tr
              td
                div
                  code= 'max'
              td
                div
                  code '12/31/2100'
              td
                div
                  | Prevent user pick a date after the configured.
            tr
              td
                div
                  code= 'format'
              td
                div
                  code 'MM/DD/YYYY'
              td
                div
                  | Format of the date used in the input.
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({})
export default class Properties extends Vue {}
</script>

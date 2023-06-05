# Comparing `tmp/ovos_skill_weather-0.0.1a8-py3-none-any.whl.zip` & `tmp/ovos_skill_weather-0.0.1a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,1179 +1,3027 @@
-Zip file size: 1319915 bytes, number of entries: 1177
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 15:04 skill_ovos_weather/LICENSE
--rw-r--r--  2.0 unx      152 b- defN 23-May-22 15:04 skill_ovos_weather/MANIFEST.in
--rw-r--r--  2.0 unx     1588 b- defN 23-May-22 15:04 skill_ovos_weather/README.md
--rw-r--r--  2.0 unx    40406 b- defN 23-May-22 15:04 skill_ovos_weather/__init__.py
--rwxr-xr-x  2.0 unx      920 b- defN 23-May-22 15:04 skill_ovos_weather/settingsmeta.json
--rw-r--r--  2.0 unx      177 b- defN 23-May-22 15:04 skill_ovos_weather/version.py
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/and.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       76 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      179 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx       99 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      207 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       65 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      187 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      241 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx       94 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      138 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       21 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/regex/location.rx
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      201 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/location.voc
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       36 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/weather.voc
--rw-r--r--  2.0 unx      185 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      169 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      118 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      107 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx      106 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       70 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      125 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       81 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx       78 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx       79 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       54 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/how.voc
--rw-r--r--  2.0 unx      161 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       41 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       42 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/and.dialog
--rw-r--r--  2.0 unx       39 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx      131 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      296 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/east.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      371 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx      150 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      318 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      391 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx      152 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       39 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx      189 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx      126 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/regex/location.rx
--rw-r--r--  2.0 unx       24 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      468 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/location.voc
--rw-r--r--  2.0 unx      111 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       69 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/weather.voc
--rw-r--r--  2.0 unx      159 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      170 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      241 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       66 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx      151 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      175 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      138 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx      138 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       27 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      206 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       34 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx      273 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx      123 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       33 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx      232 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx      168 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/how.voc
--rw-r--r--  2.0 unx      153 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/query.voc
--rw-r--r--  2.0 unx      124 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       70 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       68 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/da-dk/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/and.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       88 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      173 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-humidity-local.dialog
--rw-r--r--  2.0 unx      102 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-humidity-location.dialog
--rw-r--r--  2.0 unx       70 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--  2.0 unx      100 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--  2.0 unx       69 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--  2.0 unx       74 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-future-local.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-future-location.dialog
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-local.dialog
--rw-r--r--  2.0 unx       95 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-location.dialog
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-local.dialog
--rw-r--r--  2.0 unx      218 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-location.dialog
--rw-r--r--  2.0 unx      124 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-low.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-local.dialog
--rw-r--r--  2.0 unx      172 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-location.dialog
--rw-r--r--  2.0 unx      170 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-low-local.dialog
--rw-r--r--  2.0 unx      180 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-low-location.dialog
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-weather-local.dialog
--rw-r--r--  2.0 unx      228 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-weather-location.dialog
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-light-local.dialog
--rw-r--r--  2.0 unx      183 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-light-location.dialog
--rw-r--r--  2.0 unx      131 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      166 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      213 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-strong-local.dialog
--rw-r--r--  2.0 unx      253 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/current-wind-strong-location.dialog
--rw-r--r--  2.0 unx      173 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/current/currrent-clouds-alternative-local.dialog
--rw-r--r--  2.0 unx      147 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--  2.0 unx      177 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      173 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       93 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-humidity-local.dialog
--rw-r--r--  2.0 unx      118 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-humidity-location.dialog
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      176 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--  2.0 unx       94 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--  2.0 unx      108 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--  2.0 unx       69 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--  2.0 unx       97 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunset-local.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunset-location.dialog
--rw-r--r--  2.0 unx      115 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--  2.0 unx      146 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--  2.0 unx       97 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-local.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-location.dialog
--rw-r--r--  2.0 unx       66 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--  2.0 unx      136 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--  2.0 unx      340 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-weather-local.dialog
--rw-r--r--  2.0 unx      396 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-weather-location.dialog
--rw-r--r--  2.0 unx      165 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--  2.0 unx      264 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--  2.0 unx      147 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      260 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      162 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      189 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/error/location-not-found.dialog
--rw-r--r--  2.0 unx       95 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      110 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/error/seven-days-available.dialog
--rw-r--r--  2.0 unx      201 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      286 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       76 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      144 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx      154 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      177 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--  2.0 unx       88 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--  2.0 unx      118 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--  2.0 unx      174 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--  2.0 unx      247 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/weekly/weekly-condition.dialog
--rw-r--r--  2.0 unx       96 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/regex/location.rx
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      204 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/location.voc
--rw-r--r--  2.0 unx       67 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/sunset.voc
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/weather.voc
--rw-r--r--  2.0 unx      141 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      224 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       32 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      141 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      132 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       86 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      119 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx      237 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       67 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/how.voc
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       28 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       38 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       39 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/de-de/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/and.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/clear-sky.dialog
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/depositing-rime-fog.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-dense-intensity.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-light-intensity.dialog
--rw-r--r--  2.0 unx       28 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-moderate-intensity.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/fog.dialog
--rw-r--r--  2.0 unx       34 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/freezing-drizzle-dense-intensity.dialog
--rw-r--r--  2.0 unx       34 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/freezing-drizzle-light-intensity.dialog
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/freezing-rain-dense-intensity.dialog
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/freezing-rain-light-intensity.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/heavy-rain.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/heavy-snow-fall.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/heavy-snow-showers.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/humidity.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/mainly-clear.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/moderate-rain-showers.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/moderate-rain.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/moderate-snow-fall.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/overcast.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/partly-cloudy.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/slight-rain-showers.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/slight-rain.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/slight-snow-fall.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/slight-snow-showers.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/snow-grains.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       29 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm-with-heavy-hail.dialog
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm-with-slight-hail.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/condition/violent-rain-showers.dialog
--rw-r--r--  2.0 unx      128 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx      145 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      146 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      174 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-humidity-local.dialog
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-humidity-location.dialog
--rw-r--r--  2.0 unx       66 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-future-local.dialog
--rw-r--r--  2.0 unx      143 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-future-location.dialog
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-local.dialog
--rw-r--r--  2.0 unx      131 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-location.dialog
--rw-r--r--  2.0 unx      170 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-local.dialog
--rw-r--r--  2.0 unx      214 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-location.dialog
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-low.dialog
--rw-r--r--  2.0 unx      135 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-local.dialog
--rw-r--r--  2.0 unx      177 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-location.dialog
--rw-r--r--  2.0 unx      162 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-low-local.dialog
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-low-location.dialog
--rw-r--r--  2.0 unx      182 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-weather-local.dialog
--rw-r--r--  2.0 unx      223 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-weather-location.dialog
--rw-r--r--  2.0 unx      134 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-light-local.dialog
--rw-r--r--  2.0 unx      162 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-light-location.dialog
--rw-r--r--  2.0 unx      130 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      158 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      221 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-strong-local.dialog
--rw-r--r--  2.0 unx      258 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/current-wind-strong-location.dialog
--rw-r--r--  2.0 unx      237 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
--rw-r--r--  2.0 unx      148 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--  2.0 unx      185 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx      146 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      174 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       90 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-humidity-local.dialog
--rw-r--r--  2.0 unx      118 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-humidity-location.dialog
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      148 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--  2.0 unx       95 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--  2.0 unx      107 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--  2.0 unx      100 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--  2.0 unx      142 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--  2.0 unx      134 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunset-local.dialog
--rw-r--r--  2.0 unx      139 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunset-location.dialog
--rw-r--r--  2.0 unx      106 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--  2.0 unx      123 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--  2.0 unx       84 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-local.dialog
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-location.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--  2.0 unx      121 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--  2.0 unx      465 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-weather-local.dialog
--rw-r--r--  2.0 unx      313 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-weather-location.dialog
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--  2.0 unx      145 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--  2.0 unx      238 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      275 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      134 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--  2.0 unx      164 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      173 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       52 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/error/location-not-found.dialog
--rw-r--r--  2.0 unx       68 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/error/seven-days-available.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      128 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      156 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--  2.0 unx      224 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--  2.0 unx      291 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/inch.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/unit/millimeter.dialog
--rw-r--r--  2.0 unx       74 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/weekly/weekly-condition.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/regex/location.rx
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/forecast.voc
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/like.voc
--rw-r--r--  2.0 unx      185 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/location.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/outside.voc
--rw-r--r--  2.0 unx       42 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       21 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/sunset.voc
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/weather.voc
--rw-r--r--  2.0 unx      114 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      119 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx     1139 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--  2.0 unx       21 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      108 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/few.voc
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx      272 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/number-days.voc
--rw-r--r--  2.0 unx      182 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx       50 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx      108 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       72 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/how.voc
--rw-r--r--  2.0 unx       64 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       40 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/en-us/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       40 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/and.dialog
--rw-r--r--  2.0 unx       58 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx       45 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/humidity.dialog
--rw-r--r--  2.0 unx       45 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx       45 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      113 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      136 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       75 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-humidity-local.dialog
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-humidity-location.dialog
--rw-r--r--  2.0 unx      105 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--  2.0 unx      130 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--  2.0 unx      111 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--  2.0 unx      130 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--  2.0 unx      151 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-future-local.dialog
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-future-location.dialog
--rw-r--r--  2.0 unx      145 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-local.dialog
--rw-r--r--  2.0 unx      179 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-location.dialog
--rw-r--r--  2.0 unx      207 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--  2.0 unx      249 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--  2.0 unx      137 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--  2.0 unx      172 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-local.dialog
--rw-r--r--  2.0 unx      214 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-location.dialog
--rw-r--r--  2.0 unx      191 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--  2.0 unx      211 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--  2.0 unx      214 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-weather-local.dialog
--rw-r--r--  2.0 unx      263 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-weather-location.dialog
--rw-r--r--  2.0 unx      157 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--  2.0 unx      185 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--  2.0 unx      170 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      198 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      273 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--  2.0 unx      309 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/current-wind-strong-location.dialog
--rw-r--r--  2.0 unx      197 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/current/currrent-clouds-alternative-local.dialog
--rw-r--r--  2.0 unx      123 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--  2.0 unx      148 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx      112 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      140 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-humidity-local.dialog
--rw-r--r--  2.0 unx      150 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-humidity-location.dialog
--rw-r--r--  2.0 unx      166 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      191 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--  2.0 unx      142 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--  2.0 unx      148 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--  2.0 unx      185 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--  2.0 unx      154 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunset-local.dialog
--rw-r--r--  2.0 unx      196 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunset-location.dialog
--rw-r--r--  2.0 unx      141 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--  2.0 unx      160 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--  2.0 unx      152 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--  2.0 unx      141 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--  2.0 unx      158 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--  2.0 unx      528 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--  2.0 unx      366 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--  2.0 unx      175 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--  2.0 unx      284 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      322 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      164 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--  2.0 unx      195 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-strong-location.dialog
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/east.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx       42 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/direction/west.dialog
--rw-r--r--  2.0 unx     2430 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--  2.0 unx      200 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/error/location-not-found.dialog
--rw-r--r--  2.0 unx      121 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      153 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/error/seven-days-available.dialog
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       78 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      180 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--  2.0 unx      187 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--  2.0 unx      126 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--  2.0 unx      154 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--  2.0 unx      269 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--  2.0 unx      350 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       49 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       54 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx      112 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/weekly/weekly-condition.dialog
--rw-r--r--  2.0 unx      134 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       58 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/regex/location.rx
--rw-r--r--  2.0 unx       49 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/forecast.voc
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/like.voc
--rw-r--r--  2.0 unx      225 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/location.voc
--rw-r--r--  2.0 unx       53 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/outside.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       64 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       45 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/weather.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx       80 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      146 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--  2.0 unx       53 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx      110 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       58 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx      100 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       42 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx       46 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/few.voc
--rw-r--r--  2.0 unx      152 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx      400 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/number-days.voc
--rw-r--r--  2.0 unx      207 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx      112 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       49 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       53 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       52 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       48 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx      114 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx       44 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/how.voc
--rw-r--r--  2.0 unx      107 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       76 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       64 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       65 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       65 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       55 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       49 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 15:04 skill_ovos_weather/locale/es-es/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/direction/west.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/regex/location.rx
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/location.voc
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       48 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       83 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/weather.voc
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx       38 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx      131 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       36 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       27 b- defN 23-May-22 15:04 skill_ovos_weather/locale/fr-fr/vocabulary/query/query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/and.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        3 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       72 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       80 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-humidity-location.dialog
--rw-r--r--  2.0 unx      171 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--  2.0 unx      203 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--  2.0 unx       78 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--  2.0 unx       96 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-local.dialog
--rw-r--r--  2.0 unx      133 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-location.dialog
--rw-r--r--  2.0 unx      149 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--  2.0 unx      155 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--  2.0 unx      164 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-weather-local.dialog
--rw-r--r--  2.0 unx      392 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-weather-location.dialog
--rw-r--r--  2.0 unx       59 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--  2.0 unx       69 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--  2.0 unx      119 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      171 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      159 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--  2.0 unx      193 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-strong-location.dialog
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--  2.0 unx      168 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx       99 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--  2.0 unx       68 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--  2.0 unx      107 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--  2.0 unx      109 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--  2.0 unx      395 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--  2.0 unx      292 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--  2.0 unx       56 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--  2.0 unx      191 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      241 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--  2.0 unx       93 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      159 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/error/location-not-found.dialog
--rw-r--r--  2.0 unx       84 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      176 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      248 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx       98 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       89 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
--rw-r--r--  2.0 unx      136 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      124 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--  2.0 unx      210 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--  2.0 unx      271 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       93 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/regex/location.rx
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      201 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/location.voc
--rw-r--r--  2.0 unx       39 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/weather.voc
--rw-r--r--  2.0 unx      115 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx       98 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--  2.0 unx       33 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      131 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      116 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx      106 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      113 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx       86 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx       55 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx       81 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       59 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/how.voc
--rw-r--r--  2.0 unx       59 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       29 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/direction/west.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/regex/location.rx
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/location.voc
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       29 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/sunset.voc
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/weather.voc
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--  2.0 unx       32 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       21 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       68 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      110 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      113 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       41 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx      104 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       27 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       31 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       45 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 15:04 skill_ovos_weather/locale/it-it/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        3 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/regex/location.rx
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/location.voc
--rw-r--r--  2.0 unx       75 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       36 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/weather.voc
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx       41 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       39 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/nl-nl/vocabulary/query/query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/and.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       83 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-humidity-location.dialog
--rw-r--r--  2.0 unx      169 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-local.dialog
--rw-r--r--  2.0 unx      201 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-location.dialog
--rw-r--r--  2.0 unx       72 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-low.dialog
--rw-r--r--  2.0 unx       90 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-local.dialog
--rw-r--r--  2.0 unx      138 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-location.dialog
--rw-r--r--  2.0 unx      147 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-low-local.dialog
--rw-r--r--  2.0 unx      152 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-low-location.dialog
--rw-r--r--  2.0 unx      157 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-weather-local.dialog
--rw-r--r--  2.0 unx      384 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-weather-location.dialog
--rw-r--r--  2.0 unx       90 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-light-local.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-light-location.dialog
--rw-r--r--  2.0 unx      120 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      155 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      151 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-strong-local.dialog
--rw-r--r--  2.0 unx      198 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-strong-location.dialog
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--  2.0 unx      167 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx       99 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-high.dialog
--rw-r--r--  2.0 unx       66 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-local.dialog
--rw-r--r--  2.0 unx       95 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-location.dialog
--rw-r--r--  2.0 unx       99 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--  2.0 unx      108 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--  2.0 unx      405 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-weather-local.dialog
--rw-r--r--  2.0 unx      278 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-weather-location.dialog
--rw-r--r--  2.0 unx       78 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--  2.0 unx      101 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--  2.0 unx      200 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--  2.0 unx      244 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--  2.0 unx      100 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--  2.0 unx      124 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      225 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       96 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/error/location-not-found.dialog
--rw-r--r--  2.0 unx      179 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      245 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx       93 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      139 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      130 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--  2.0 unx      193 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--  2.0 unx      278 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       90 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/regex/location.rx
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      250 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/location.voc
--rw-r--r--  2.0 unx       66 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/sunset.voc
--rw-r--r--  2.0 unx       14 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/weather.voc
--rw-r--r--  2.0 unx      129 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      119 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      113 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/fog.voc
--rw-r--r--  2.0 unx       24 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       75 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      127 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       99 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       74 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      112 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx       94 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx       59 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       30 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx       83 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       60 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/how.voc
--rw-r--r--  2.0 unx       63 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       65 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       29 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       33 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       40 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx       28 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx      436 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/east.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/north.dialog
--rw-r--r--  2.0 unx       26 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       24 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/south.dialog
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/direction/west.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       32 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/regex/location.rx
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      378 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/location.voc
--rw-r--r--  2.0 unx       91 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       50 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/sunset.voc
--rw-r--r--  2.0 unx      166 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/weather.voc
--rw-r--r--  2.0 unx       47 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx      203 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       73 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       37 b- defN 23-May-22 15:04 skill_ovos_weather/locale/ru-ru/vocabulary/query/query.voc
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/and.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/percentage-number.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/ash.dialog
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/clear.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/clouds.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/drizzle.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/dust.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/haze.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/mist.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/rain.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/smoke.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/snow.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/squall.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/condition/tornado.dialog
--rw-r--r--  2.0 unx       96 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-local.dialog
--rw-r--r--  2.0 unx       83 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-location.dialog
--rw-r--r--  2.0 unx      188 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/east.dialog
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/north.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/northeast.dialog
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/northwest.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/south.dialog
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/southeast.dialog
--rw-r--r--  2.0 unx        9 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/southwest.dialog
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/direction/west.dialog
--rw-r--r--  2.0 unx      234 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/error/cant-get-forecast.dialog
--rw-r--r--  2.0 unx       84 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/error/no-forecast.dialog
--rw-r--r--  2.0 unx      213 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--  2.0 unx      268 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--  2.0 unx      106 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--  2.0 unx       80 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--  2.0 unx      119 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--  2.0 unx      117 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/unit/celsius.dialog
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/unit/fahrenheit.dialog
--rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/unit/meters per second.dialog
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/unit/miles per hour.dialog
--rw-r--r--  2.0 unx       94 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/dialog/weekly/weekly-temperature.dialog
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/regex/location.rx
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/forecast.voc
--rw-r--r--  2.0 unx      201 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/location.voc
--rw-r--r--  2.0 unx       54 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/sunrise.voc
--rw-r--r--  2.0 unx       33 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/sunset.voc
--rw-r--r--  2.0 unx        7 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/weather.voc
--rw-r--r--  2.0 unx      122 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/clear.voc
--rw-r--r--  2.0 unx      113 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/clouds.voc
--rw-r--r--  2.0 unx      105 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--  2.0 unx       29 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/humidity.voc
--rw-r--r--  2.0 unx       58 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/precipitation.voc
--rw-r--r--  2.0 unx      116 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/rain.voc
--rw-r--r--  2.0 unx       97 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/snow.voc
--rw-r--r--  2.0 unx       85 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/thunderstorm.voc
--rw-r--r--  2.0 unx       61 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/condition/windy.voc
--rw-r--r--  2.0 unx        8 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/couple.voc
--rw-r--r--  2.0 unx      103 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/later.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/next.voc
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/now.voc
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-day.voc
--rw-r--r--  2.0 unx       51 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-time.voc
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/today.voc
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/week.voc
--rw-r--r--  2.0 unx       36 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/date-time/weekend.voc
--rw-r--r--  2.0 unx       16 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query-current.voc
--rw-r--r--  2.0 unx      141 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query-future.voc
--rw-r--r--  2.0 unx       88 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query.voc
--rw-r--r--  2.0 unx        4 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/how.voc
--rw-r--r--  2.0 unx       74 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/query.voc
--rw-r--r--  2.0 unx       50 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/query/when.voc
--rw-r--r--  2.0 unx       27 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/cold.voc
--rw-r--r--  2.0 unx       28 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/fog.voc
--rw-r--r--  2.0 unx       43 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/high.voc
--rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/hot.voc
--rw-r--r--  2.0 unx       25 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/low.voc
--rw-r--r--  2.0 unx       48 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/temperature/temperature.voc
--rw-r--r--  2.0 unx       11 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/unit/fahrenheit.voc
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.entity
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.voc
--rw-r--r--  2.0 unx     2327 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/PKG-INFO
--rw-r--r--  2.0 unx    56732 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       84 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/entry_points.txt
--rw-r--r--  2.0 unx      186 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/requires.txt
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 skill_ovos_weather/ovos_skill_weather.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1606 b- defN 23-May-22 15:04 skill_ovos_weather/res/desktop/skill.json
--rw-r--r--  2.0 unx     8974 b- defN 23-May-22 15:04 skill_ovos_weather/ui/CurrentWeather.qml
--rw-r--r--  2.0 unx     2309 b- defN 23-May-22 15:04 skill_ovos_weather/ui/DailyForecast.qml
--rw-r--r--  2.0 unx     1751 b- defN 23-May-22 15:04 skill_ovos_weather/ui/DailyForecastColumnDelegate.qml
--rw-r--r--  2.0 unx     2355 b- defN 23-May-22 15:04 skill_ovos_weather/ui/HourlyForecast.qml
--rw-r--r--  2.0 unx     1745 b- defN 23-May-22 15:04 skill_ovos_weather/ui/HourlyForecastColumnDelegate.qml
--rw-r--r--  2.0 unx     5832 b- defN 23-May-22 15:04 skill_ovos_weather/ui/SingleDay.qml
--rw-r--r--  2.0 unx     2913 b- defN 23-May-22 15:04 skill_ovos_weather/ui/SunriseSunset.qml
--rw-r--r--  2.0 unx     8388 b- defN 23-May-22 15:04 skill_ovos_weather/ui/WeatherDelegate.qml
--rw-r--r--  2.0 unx      346 b- defN 23-May-22 15:04 skill_ovos_weather/ui/qmldir
--rwxr-xr-x  2.0 unx     4829 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/clouds.json
--rwxr-xr-x  2.0 unx     5635 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/fog.json
--rw-r--r--  2.0 unx     8384 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/night.json
--rwxr-xr-x  2.0 unx     8559 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/partial_clouds.json
--rwxr-xr-x  2.0 unx    64205 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/rain.json
--rwxr-xr-x  2.0 unx    30103 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/sleet.json
--rwxr-xr-x  2.0 unx    46868 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/snow.json
--rwxr-xr-x  2.0 unx     4248 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/storm.json
--rwxr-xr-x  2.0 unx     4811 b- defN 23-May-22 15:04 skill_ovos_weather/ui/animations/sun.json
--rw-r--r--  2.0 unx      313 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/Rainy.qml
--rw-r--r--  2.0 unx      235 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/Simple.qml
--rw-r--r--  2.0 unx      314 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/Snowy.qml
--rw-r--r--  2.0 unx       62 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/qmldir
--rw-r--r--  2.0 unx     1725 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/components/Rain.qml
--rw-r--r--  2.0 unx     1822 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/components/Snow.qml
--rw-r--r--  2.0 unx       36 b- defN 23-May-22 15:04 skill_ovos_weather/ui/backgrounds/components/qmldir
--rw-r--r--  2.0 unx      936 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/clouds.svg
--rw-r--r--  2.0 unx   451965 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/day.jpg
--rw-r--r--  2.0 unx      994 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/fog.svg
--rw-r--r--  2.0 unx      605 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/high_temperature.svg
--rw-r--r--  2.0 unx     2175 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/humidity.svg
--rw-r--r--  2.0 unx      595 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/low_temperature.svg
--rw-r--r--  2.0 unx      496 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/moon.svg
--rw-r--r--  2.0 unx   379434 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/night.jpg
--rw-r--r--  2.0 unx   177391 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/night.svg
--rw-r--r--  2.0 unx     4471 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/partial_clouds_day.svg
--rw-r--r--  2.0 unx     1025 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/partial_clouds_night.svg
--rw-r--r--  2.0 unx     5481 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/rain.svg
--rw-r--r--  2.0 unx     4208 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/snow.svg
--rw-r--r--  2.0 unx      753 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/storm.svg
--rw-r--r--  2.0 unx     3502 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/sun.svg
--rw-r--r--  2.0 unx     1253 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/sunrise.svg
--rw-r--r--  2.0 unx      834 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/sunset.svg
--rw-r--r--  2.0 unx     3129 b- defN 23-May-22 15:04 skill_ovos_weather/ui/images/wind.svg
--rw-r--r--  2.0 unx      345 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_de.ts
--rw-r--r--  2.0 unx      348 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_es.ts
--rw-r--r--  2.0 unx      349 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_fr.ts
--rw-r--r--  2.0 unx      347 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_it.ts
--rw-r--r--  2.0 unx      346 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_nl.ts
--rw-r--r--  2.0 unx      344 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/DailyForecast_pt.ts
--rw-r--r--  2.0 unx      350 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_de.ts
--rw-r--r--  2.0 unx      349 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_es.ts
--rw-r--r--  2.0 unx      347 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_fr.ts
--rw-r--r--  2.0 unx      348 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_it.ts
--rw-r--r--  2.0 unx      343 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_nl.ts
--rw-r--r--  2.0 unx      346 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/HourlyForecast_pt.ts
--rw-r--r--  2.0 unx      171 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_de.qm
--rw-r--r--  2.0 unx      179 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_es.qm
--rw-r--r--  2.0 unx      177 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_fr.qm
--rw-r--r--  2.0 unx      175 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_it.qm
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_nl.qm
--rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:04 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_pt.qm
--rw-r--r--  2.0 unx     1048 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/__init__.py
--rw-r--r--  2.0 unx     3646 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/config.py
--rw-r--r--  2.0 unx    16926 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/dialog.py
--rw-r--r--  2.0 unx     4942 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/intent.py
--rw-r--r--  2.0 unx     4385 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/openmeteo.py
--rw-r--r--  2.0 unx     4983 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/util.py
--rw-r--r--  2.0 unx    19610 b- defN 23-May-22 15:04 skill_ovos_weather/weather_helpers/weather.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2327 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       84 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx   143256 b- defN 23-May-22 15:04 ovos_skill_weather-0.0.1a8.dist-info/RECORD
-1177 files, 1677031 bytes uncompressed, 1073875 bytes compressed:  36.0%
+Zip file size: 1980340 bytes, number of entries: 3025
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-05 15:25 skill_ovos_weather/LICENSE
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/MANIFEST.in
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jun-05 15:25 skill_ovos_weather/README.md
+-rw-r--r--  2.0 unx    42055 b- defN 23-Jun-05 15:25 skill_ovos_weather/__init__.py
+-rwxr-xr-x  2.0 unx      920 b- defN 23-Jun-05 15:25 skill_ovos_weather/settingsmeta.json
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/version.py
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/and.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      262 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      273 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      309 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      524 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      329 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      266 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/regex/location.rx
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/location.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      386 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/and.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      248 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      295 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      133 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      494 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      270 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      302 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2329 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      315 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/regex/location.rx
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/location.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/cs-cz/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/and.dialog
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      262 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      564 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx      318 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      391 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      328 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/regex/location.rx
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      468 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/location.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/outside.voc
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
+-rw-r--r--  2.0 unx     1211 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      206 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      273 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       33 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/da-dk/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/and.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      253 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-low-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-low-location.dialog
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      351 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      396 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/date-time/afternoon.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/date-time/early morning.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/date-time/evening.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/date-time/morning.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/date-time/overnight.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      286 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/regex/location.rx
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/location.voc
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx      502 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/de-de/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/and.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      221 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-low-local.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-low-location.dialog
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      465 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      313 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/date-time/afternoon.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/date-time/early morning.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/date-time/evening.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/date-time/morning.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/date-time/overnight.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      291 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/kilometer per hour.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/regex/location.rx
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/location.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/en-us/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/and.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      273 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      309 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-low-local.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-low-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      528 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      322 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2430 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/regex/location.rx
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/location.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      400 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/es-es/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/and.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      222 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      287 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      309 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      540 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      374 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      282 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     3323 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      266 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      344 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/regex/location.rx
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/location.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      397 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/fr-fr/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/and.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        3 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      203 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      133 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      392 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      395 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      248 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      210 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/regex/location.rx
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/location.voc
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--  2.0 unx       33 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/and.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      261 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      291 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      227 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      307 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2590 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      256 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      359 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/regex/location.rx
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/location.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      389 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/hu-hu/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/and.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      133 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      209 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      265 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      528 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      359 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      266 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      313 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2386 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      206 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      256 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      327 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/regex/location.rx
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/location.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--  2.0 unx       32 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      421 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/it-it/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/and.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        3 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      264 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      543 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      378 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      314 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/regex/location.rx
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/location.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1253 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       39 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      373 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      199 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/nl-nl/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/and.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      206 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      209 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      248 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      261 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      294 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      337 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      281 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      321 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     1674 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      133 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/regex/location.rx
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/location.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1474 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      340 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pl-pl/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/and.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      384 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-high.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      405 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      278 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      244 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      278 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/regex/location.rx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/location.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       33 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/and.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      222 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      265 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      290 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      152 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      362 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      270 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      302 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2075 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      209 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/regex/location.rx
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/location.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1271 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/pt-pt/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/and.dialog
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      229 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      314 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      329 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      207 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      239 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      268 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      399 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      314 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      222 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      436 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
+-rw-r--r--  2.0 unx      614 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      432 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      211 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      363 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      396 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      240 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     2407 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      295 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      212 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      442 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       32 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/regex/location.rx
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      378 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/location.voc
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     2191 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      203 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      711 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      368 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/ru-ru/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/and.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      231 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      286 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      501 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      351 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     1505 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      154 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      259 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/regex/location.rx
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/location.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1339 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      511 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      227 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-fi/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/and.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      206 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      276 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      306 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      221 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      617 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      197 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      306 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      331 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--  2.0 unx      268 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      173 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/regex/location.rx
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/location.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       33 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/weather.voc
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1310 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      419 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       27 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/fog.voc
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/and.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/percentage-number.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/ash.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/clear-sky.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/clear.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/clouds.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/depositing-rime-fog.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-moderate-intensity.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/dust.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/fog.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-drizzle-light-intensity.dialog
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-rain-dense-intensity.dialog
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-rain-light-intensity.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/haze.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-rain.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-snow-fall.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-snow-showers.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/humidity.dialog
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/mainly-clear.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/mist.dialog
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-rain-showers.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-rain.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-snow-fall.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/overcast.dialog
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/partly-cloudy.dialog
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/rain.dialog
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/slight-rain-showers.dialog
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/slight-rain.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/slight-snow-fall.dialog
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/slight-snow-showers.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/smoke.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/snow-grains.dialog
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/snow.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/squall.dialog
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm-with-slight-hail.dialog
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm.dialog
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/tornado.dialog
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/condition/violent-rain-showers.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-humidity-local.dialog
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-humidity-location.dialog
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-temperature-local.dialog
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-temperature-location.dialog
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-weather-local.dialog
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-weather-location.dialog
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-light-local.dialog
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-light-location.dialog
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      217 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      291 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--  2.0 unx      218 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/current/currrent-clouds-alternative-local.dialog
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--  2.0 unx      158 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-weather-local.dialog
+-rw-r--r--  2.0 unx      358 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-weather-location.dialog
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--  2.0 unx      345 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--  2.0 unx      367 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-strong-location.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/east.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/north.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/northeast.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/northwest.dialog
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/south.dialog
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/southeast.dialog
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/southwest.dialog
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/direction/west.dialog
+-rw-r--r--  2.0 unx     1538 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/error/cant-get-forecast.dialog
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/error/location-not-found.dialog
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/error/no-forecast.dialog
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/error/seven-days-available.dialog
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--  2.0 unx      169 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/celsius.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/fahrenheit.dialog
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/inch.dialog
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/meter per second.dialog
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/miles per hour.dialog
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/unit/millimeter.dialog
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/weekly/weekly-condition.dialog
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/dialog/weekly/weekly-temperature.dialog
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/regex/location.rx
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/forecast.voc
+-rw-r--r--  2.0 unx      229 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/location.voc
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/outside.voc
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/sunrise.voc
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/sunset.voc
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/weather.voc
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/clear.voc
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/clouds.voc
+-rw-r--r--  2.0 unx     1329 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/fog.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/humidity.voc
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/precipitation.voc
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/rain.voc
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/snow.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/thunderstorm.voc
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/condition/windy.voc
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/couple.voc
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/few.voc
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/later.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/next.voc
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/now.voc
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/number-days.voc
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/relative-day.voc
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/relative-time.voc
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/today.voc
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/week.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/date-time/weekend.voc
+-rw-r--r--  2.0 unx       56 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query-current.voc
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query-future.voc
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/how.voc
+-rw-r--r--  2.0 unx      123 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/query.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/query/when.voc
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/temperature/cold.voc
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/temperature/high.voc
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/temperature/hot.voc
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/temperature/low.voc
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/temperature/temperature.voc
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/unit/fahrenheit.voc
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/unit/unit.entity
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-05 15:25 skill_ovos_weather/locale/tr-tr/vocabulary/unit/unit.voc
+-rw-r--r--  2.0 unx     2327 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx   158058 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/requires.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 skill_ovos_weather/ovos_skill_weather.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1606 b- defN 23-Jun-05 15:25 skill_ovos_weather/res/desktop/skill.json
+-rw-r--r--  2.0 unx    10559 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/CurrentWeather.qml
+-rw-r--r--  2.0 unx     2309 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/DailyForecast.qml
+-rw-r--r--  2.0 unx     1751 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/DailyForecastColumnDelegate.qml
+-rw-r--r--  2.0 unx     2355 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/HourlyForecast.qml
+-rw-r--r--  2.0 unx     1745 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/HourlyForecastColumnDelegate.qml
+-rw-r--r--  2.0 unx    10263 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/SingleDay.qml
+-rw-r--r--  2.0 unx     2514 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/SunriseSunset.qml
+-rw-r--r--  2.0 unx     8388 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/WeatherDelegate.qml
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/qmldir
+-rwxr-xr-x  2.0 unx     4829 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/clouds.json
+-rwxr-xr-x  2.0 unx     5635 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/fog.json
+-rw-r--r--  2.0 unx     8384 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/night.json
+-rwxr-xr-x  2.0 unx     8559 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/partial_clouds.json
+-rwxr-xr-x  2.0 unx    64205 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/rain.json
+-rwxr-xr-x  2.0 unx    30103 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/sleet.json
+-rwxr-xr-x  2.0 unx    46868 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/snow.json
+-rwxr-xr-x  2.0 unx     4248 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/storm.json
+-rwxr-xr-x  2.0 unx     4811 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/animations/sun.json
+-rw-r--r--  2.0 unx      313 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/Rainy.qml
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/Simple.qml
+-rw-r--r--  2.0 unx      314 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/Snowy.qml
+-rw-r--r--  2.0 unx       62 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/qmldir
+-rw-r--r--  2.0 unx     1725 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/components/Rain.qml
+-rw-r--r--  2.0 unx     1822 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/components/Snow.qml
+-rw-r--r--  2.0 unx       36 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/backgrounds/components/qmldir
+-rw-r--r--  2.0 unx     6134 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/chanceprecipitation.svg
+-rw-r--r--  2.0 unx      936 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/clouds.svg
+-rw-r--r--  2.0 unx   451965 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/day.jpg
+-rw-r--r--  2.0 unx      994 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/fog.svg
+-rw-r--r--  2.0 unx      605 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/high_temperature.svg
+-rw-r--r--  2.0 unx     2175 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/humidity.svg
+-rw-r--r--  2.0 unx      595 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/low_temperature.svg
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/moon.svg
+-rw-r--r--  2.0 unx   379434 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/night.jpg
+-rw-r--r--  2.0 unx   177391 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/night.svg
+-rw-r--r--  2.0 unx     4471 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/partial_clouds_day.svg
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/partial_clouds_night.svg
+-rw-r--r--  2.0 unx     5481 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/rain.svg
+-rw-r--r--  2.0 unx     4208 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/snow.svg
+-rw-r--r--  2.0 unx      753 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/storm.svg
+-rw-r--r--  2.0 unx     3502 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/sun.svg
+-rw-r--r--  2.0 unx     1253 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/sunrise.svg
+-rw-r--r--  2.0 unx      834 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/sunset.svg
+-rw-r--r--  2.0 unx     3129 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/images/wind.svg
+-rw-r--r--  2.0 unx      345 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_de.ts
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_es.ts
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_fr.ts
+-rw-r--r--  2.0 unx      347 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_it.ts
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_nl.ts
+-rw-r--r--  2.0 unx      344 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/DailyForecast_pt.ts
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_de.ts
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_es.ts
+-rw-r--r--  2.0 unx      347 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_fr.ts
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_it.ts
+-rw-r--r--  2.0 unx      343 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_nl.ts
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/HourlyForecast_pt.ts
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_de.qm
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_es.qm
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_fr.qm
+-rw-r--r--  2.0 unx      175 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_it.qm
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_nl.qm
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-05 15:25 skill_ovos_weather/ui/translations/skill-ovos-weather.openvoiceos_pt.qm
+-rw-r--r--  2.0 unx     1048 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/__init__.py
+-rw-r--r--  2.0 unx     3638 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/config.py
+-rw-r--r--  2.0 unx    17783 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/dialog.py
+-rw-r--r--  2.0 unx     5081 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/intent.py
+-rw-r--r--  2.0 unx     5196 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/openmeteo.py
+-rw-r--r--  2.0 unx     5389 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/util.py
+-rw-r--r--  2.0 unx    19977 b- defN 23-Jun-05 15:25 skill_ovos_weather/weather_helpers/weather.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2338 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx   380382 b- defN 23-Jun-05 15:25 ovos_skill_weather-0.0.1a9.dist-info/RECORD
+3025 files, 2285273 bytes uncompressed, 1324672 bytes compressed:  42.0%
```

## zipnote {}

```diff
@@ -21,62 +21,299 @@
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-high-low.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/direction/northeast.dialog
@@ -96,17 +333,26 @@
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/direction/west.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/error/cant-get-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/error/location-not-found.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/error/no-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/error/seven-days-available.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
@@ -117,38 +363,68 @@
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/ca-es/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/ca-es/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ca-es/dialog/weekly/weekly-condition.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/dialog/weekly/weekly-temperature.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/weather.voc
@@ -156,14 +432,17 @@
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/clear.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/clouds.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/fog.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/humidity.voc
@@ -183,23 +462,29 @@
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/condition/windy.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/couple.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/next.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/now.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/number-days.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-day.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/relative-time.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/date-time/today.voc
@@ -249,68 +534,803 @@
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/ca-es/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/cs-cz/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/cs-cz/vocabulary/unit/unit.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/and.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/direction/northeast.dialog
@@ -330,17 +1350,26 @@
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/direction/west.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/error/cant-get-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/error/location-not-found.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/error/no-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/error/seven-days-available.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
@@ -351,38 +1380,68 @@
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/da-dk/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/da-dk/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/da-dk/dialog/weekly/weekly-condition.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/dialog/weekly/weekly-temperature.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/weather.voc
@@ -393,14 +1452,17 @@
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/clouds.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/fog.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/humidity.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/precipitation.voc
@@ -417,23 +1479,29 @@
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/condition/windy.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/couple.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/next.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/now.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/number-days.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-day.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/relative-time.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/da-dk/vocabulary/date-time/today.voc
@@ -492,50 +1560,134 @@
 
 Filename: skill_ovos_weather/locale/de-de/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
@@ -570,35 +1722,20 @@
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-sunset-past-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-location.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-high-low.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-low-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/de-de/dialog/current/current-temperature-low-location.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-weather-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-weather-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/current/current-wind-light-local.dialog
@@ -666,14 +1803,20 @@
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-high-low-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
@@ -702,14 +1845,29 @@
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/date-time/afternoon.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/date-time/early morning.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/date-time/evening.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/date-time/morning.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/date-time/overnight.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/direction/northeast.dialog
@@ -783,20 +1941,26 @@
 
 Filename: skill_ovos_weather/locale/de-de/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/de-de/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/de-de/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/de-de/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/dialog/unit/millimeter.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/dialog/weekly/weekly-condition.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/dialog/weekly/weekly-temperature.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/regex/location.rx
@@ -804,14 +1968,17 @@
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/weather.voc
@@ -846,23 +2013,29 @@
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/condition/windy.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/couple.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/next.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/now.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/number-days.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-day.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-time.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/de-de/vocabulary/date-time/today.voc
@@ -1083,35 +2256,20 @@
 
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-sunset-past-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-location.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-high-low.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-low-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/en-us/dialog/current/current-temperature-low-location.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-weather-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-weather-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/current/current-wind-light-local.dialog
@@ -1179,14 +2337,20 @@
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-high-low-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
@@ -1215,14 +2379,29 @@
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/en-us/dialog/date-time/afternoon.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/date-time/early morning.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/date-time/evening.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/date-time/morning.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/date-time/overnight.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/en-us/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/direction/northeast.dialog
@@ -1287,15 +2466,18 @@
 
 Filename: skill_ovos_weather/locale/en-us/dialog/unit/fahrenheit.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/unit/inch.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/en-us/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/en-us/dialog/unit/kilometer per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/en-us/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/unit/miles per hour.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/dialog/unit/millimeter.dialog
 Comment: 
@@ -1308,17 +2490,14 @@
 
 Filename: skill_ovos_weather/locale/en-us/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/vocabulary/forecast.voc
 Comment: 
 
-Filename: skill_ovos_weather/locale/en-us/vocabulary/like.voc
-Comment: 
-
 Filename: skill_ovos_weather/locale/en-us/vocabulary/location.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/vocabulary/outside.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/en-us/vocabulary/sunrise.voc
@@ -1440,53 +2619,134 @@
 
 Filename: skill_ovos_weather/locale/es-es/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/humidity.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-condition-not-expected-local.dialog
@@ -1521,35 +2781,20 @@
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-sunset-past-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-location.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-high-low.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-location.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-low-local.dialog
-Comment: 
-
-Filename: skill_ovos_weather/locale/es-es/dialog/current/current-temperature-low-location.dialog
-Comment: 
-
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-weather-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-weather-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/current/current-wind-light-local.dialog
@@ -1617,14 +2862,20 @@
 
 Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-high-low-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/daily/daily-temperature-low-local.dialog
@@ -1722,35 +2973,38 @@
 
 Filename: skill_ovos_weather/locale/es-es/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/es-es/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/es-es/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/es-es/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/es-es/dialog/unit/millimeter.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/es-es/dialog/weekly/weekly-condition.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/dialog/weekly/weekly-temperature.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/vocabulary/forecast.voc
 Comment: 
 
-Filename: skill_ovos_weather/locale/es-es/vocabulary/like.voc
-Comment: 
-
 Filename: skill_ovos_weather/locale/es-es/vocabulary/location.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/vocabulary/outside.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/vocabulary/sunrise.voc
@@ -1863,56 +3117,302 @@
 
 Filename: skill_ovos_weather/locale/es-es/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/es-es/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/and.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/direction/northeast.dialog
@@ -1929,62 +3429,203 @@
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/direction/southwest.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/direction/west.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/weather.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/fog.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/humidity.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/precipitation.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/thunderstorm.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/condition/windy.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/next.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/how.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/query.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/fr-fr/vocabulary/unit/unit.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/gl-es/dialog/and.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/condition/ash.dialog
@@ -2190,15 +3831,15 @@
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/gl-es/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/gl-es/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/unit/miles per hour.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/dialog/weekly/weekly-temperature.dialog
 Comment: 
@@ -2316,62 +3957,803 @@
 
 Filename: skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/gl-es/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/hu-hu/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/hu-hu/vocabulary/unit/unit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/and.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/direction/northeast.dialog
@@ -2388,35 +4770,89 @@
 
 Filename: skill_ovos_weather/locale/it-it/dialog/direction/southwest.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/direction/west.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/it-it/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/it-it/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/weather.voc
@@ -2424,14 +4860,17 @@
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/clear.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/clouds.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/fog.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/humidity.voc
@@ -2442,32 +4881,71 @@
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/rain.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/snow.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/thunderstorm.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/condition/windy.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/next.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/week.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/date-time/weekend.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query-future.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/query/confirm-query.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/query/how.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/query/query.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/it-it/vocabulary/query/when.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/it-it/vocabulary/temperature/cold.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/temperature/high.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/temperature/hot.voc
@@ -2484,56 +4962,302 @@
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/it-it/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/and.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/northeast.dialog
@@ -2547,62 +5271,707 @@
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/southeast.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/southwest.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/weather.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/fog.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/humidity.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/precipitation.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/thunderstorm.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/condition/windy.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/next.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/how.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/query.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/nl-nl/vocabulary/unit/unit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/pl-pl/vocabulary/unit/unit.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/pt-br/dialog/and.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/condition/ash.dialog
@@ -2805,15 +6174,15 @@
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/pt-br/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/pt-br/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/unit/miles per hour.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/dialog/weekly/weekly-temperature.dialog
 Comment: 
@@ -2931,59 +6300,806 @@
 
 Filename: skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/pt-br/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/pt-pt/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/pt-pt/vocabulary/unit/unit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/and.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/direction/northeast.dialog
@@ -3000,116 +7116,992 @@
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/direction/southwest.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/direction/west.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/weather.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/fog.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/humidity.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/precipitation.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/thunderstorm.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/condition/windy.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/next.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/how.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/query.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/ru-ru/vocabulary/unit/unit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-fi/vocabulary/unit/unit.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/and.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/percentage-number.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/ash.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/clear-sky.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/clear.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/clouds.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/drizzle.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/dust.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/haze.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/mainly-clear.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/mist.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/partly-cloudy.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/rain.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/smoke.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/snow-grains.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/snow.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/squall.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/thunderstorm.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/condition/tornado.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/direction/east.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/direction/north.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/direction/northeast.dialog
@@ -3129,17 +8121,26 @@
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/direction/west.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/error/cant-get-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/error/location-not-found.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/error/no-forecast.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/error/seven-days-available.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
@@ -3150,38 +8151,68 @@
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/unit/celsius.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/unit/fahrenheit.dialog
 Comment: 
 
-Filename: skill_ovos_weather/locale/sv-se/dialog/unit/meters per second.dialog
+Filename: skill_ovos_weather/locale/sv-se/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/unit/meter per second.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/dialog/unit/miles per hour.dialog
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/sv-se/dialog/weekly/weekly-condition.dialog
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/dialog/weekly/weekly-temperature.dialog
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/regex/location.rx
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/forecast.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/location.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/vocabulary/outside.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/sunrise.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/sunset.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/weather.voc
@@ -3189,14 +8220,17 @@
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/clear.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/clouds.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/humidity.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/precipitation.voc
@@ -3213,23 +8247,29 @@
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/condition/windy.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/couple.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/few.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/later.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/next.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/now.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/number-days.voc
+Comment: 
+
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-day.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/relative-time.voc
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/date-time/today.voc
@@ -3282,14 +8322,515 @@
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.entity
 Comment: 
 
 Filename: skill_ovos_weather/locale/sv-se/vocabulary/unit/unit.voc
 Comment: 
 
+Filename: skill_ovos_weather/locale/tr-tr/dialog/and.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/percentage-number.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/ash.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/clear-sky.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/clouds.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/depositing-rime-fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle-moderate-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/drizzle.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/dust.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/fog.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-drizzle-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-rain-dense-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/freezing-rain-light-intensity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/haze.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/heavy-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/humidity.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/mainly-clear.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/mist.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/moderate-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/overcast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/partly-cloudy.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/slight-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/slight-rain.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/slight-snow-fall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/slight-snow-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/smoke.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/snow-grains.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/snow.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/squall.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm-with-slight-hail.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/thunderstorm.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/tornado.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/condition/violent-rain-showers.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunrise-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-future-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-future-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-past-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-sunset-past-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/current-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/current/currrent-clouds-alternative-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-not-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-condition-not-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-humidity-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-humidity-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-none-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-precipitation-next-none-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunrise-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunrise-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunset-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-sunset-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-high-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-high-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-low-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-temperature-low-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-light-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-light-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-moderate-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-moderate-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-strong-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/daily/daily-wind-strong-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/east.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/north.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/northeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/northwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/south.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/southeast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/southwest.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/direction/west.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/error/cant-get-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/error/forty-eight-hours-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/error/location-not-found.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/error/no-forecast.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/error/seven-days-available.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-condition-expected-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-condition-expected-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-precipitation-next-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-precipitation-next-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-temperature-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-temperature-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-weather-local.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/hourly/hourly-weather-location.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/celsius.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/fahrenheit.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/inch.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/meter per second.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/miles per hour.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/unit/millimeter.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/weekly/weekly-condition.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/dialog/weekly/weekly-temperature.dialog
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/regex/location.rx
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/forecast.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/location.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/outside.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/sunrise.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/sunset.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/weather.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/clear.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/clouds.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/do-i-need-an-umbrella.intent
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/fog.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/humidity.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/precipitation.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/rain.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/snow.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/thunderstorm.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/condition/windy.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/couple.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/few.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/later.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/next.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/now.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/number-days.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/relative-day.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/relative-time.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/today.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/week.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/date-time/weekend.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query-current.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query-future.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/confirm-query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/how.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/query.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/query/when.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/temperature/cold.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/temperature/high.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/temperature/hot.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/temperature/low.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/temperature/temperature.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/unit/fahrenheit.voc
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/unit/unit.entity
+Comment: 
+
+Filename: skill_ovos_weather/locale/tr-tr/vocabulary/unit/unit.voc
+Comment: 
+
 Filename: skill_ovos_weather/ovos_skill_weather.egg-info/PKG-INFO
 Comment: 
 
 Filename: skill_ovos_weather/ovos_skill_weather.egg-info/SOURCES.txt
 Comment: 
 
 Filename: skill_ovos_weather/ovos_skill_weather.egg-info/dependency_links.txt
@@ -3378,14 +8919,17 @@
 
 Filename: skill_ovos_weather/ui/backgrounds/components/Snow.qml
 Comment: 
 
 Filename: skill_ovos_weather/ui/backgrounds/components/qmldir
 Comment: 
 
+Filename: skill_ovos_weather/ui/images/chanceprecipitation.svg
+Comment: 
+
 Filename: skill_ovos_weather/ui/images/clouds.svg
 Comment: 
 
 Filename: skill_ovos_weather/ui/images/day.jpg
 Comment: 
 
 Filename: skill_ovos_weather/ui/images/fog.svg
@@ -3507,26 +9051,26 @@
 
 Filename: skill_ovos_weather/weather_helpers/util.py
 Comment: 
 
 Filename: skill_ovos_weather/weather_helpers/weather.py
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/LICENSE
+Filename: ovos_skill_weather-0.0.1a9.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/METADATA
+Filename: ovos_skill_weather-0.0.1a9.dist-info/METADATA
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/WHEEL
+Filename: ovos_skill_weather-0.0.1a9.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/entry_points.txt
+Filename: ovos_skill_weather-0.0.1a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/top_level.txt
+Filename: ovos_skill_weather-0.0.1a9.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_skill_weather-0.0.1a8.dist-info/RECORD
+Filename: ovos_skill_weather-0.0.1a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skill_ovos_weather/__init__.py

```diff
@@ -20,29 +20,37 @@
 city name provided in the request.
 """
 from datetime import datetime
 from time import sleep
 from typing import List
 
 from lingua_franca.parse import extract_number
+from lingua_franca.format import (
+    nice_time,
+    nice_weekday,
+    get_date_strings
+)
 from ovos_bus_client.message import Message
 from ovos_utils import classproperty
 from ovos_utils.intents import IntentBuilder
+from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_workshop.decorators import intent_handler, skill_api_method
 from ovos_workshop.skills import OVOSSkill
 from requests import HTTPError
 
 from .weather_helpers import (
-    CurrentDialog,
+    CURRENT,
     DAILY,
-    DailyDialog,
-    Weather,
     HOURLY,
+    WeatherDialog,
+    CurrentDialog,
+    DailyDialog,
     HourlyDialog,
+    Weather,
     get_dialog_for_timeframe,
     LocationNotFoundError,
     WeatherConfig,
     WeatherIntent,
     WeatherReport,
     WeeklyDialog,
     get_report
@@ -66,40 +74,46 @@
                                    no_network_fallback=False,
                                    no_gui_fallback=True)
 
     def initialize(self):
         # TODO - skill api
         self.bus.on("skill-ovos-weather.openvoiceos.weather.request",
                     self.get_current_weather_homescreen)
+    
+    @property
+    def date_format(self) -> str:
+        return self.config_core.get("date_format", "MDY")
+    
+    @property
+    def use_24h(self) -> bool:
+        return self.config_core.get("time_format", "full") == "full"
 
     @intent_handler(
         IntentBuilder("current_weather")
         .optionally("query")
         .one_of("weather", "forecast")
         .optionally("location")
-        .optionally("today")
         .optionally("unit")
     )
     def handle_current_weather(self, message: Message):
         """Handle current weather requests such as: what is the weather like?
 
         Args:
             message: Message Bus event information from the intent parser
         """
         self._report_current_weather(message)
 
     @intent_handler(
-        IntentBuilder("like_outside")
+        IntentBuilder("outside")
         .require("query")
-        .require("like")
         .require("outside")
         .optionally("location")
         .optionally("unit")
     )
-    def handle_like_outside(self, message: Message):
+    def handle_outside(self, message: Message):
         """Handle current weather requests such as: what's it like outside?
 
         Args:
             message: Message Bus event information from the intent parser
         """
         self._report_current_weather(message)
 
@@ -129,15 +143,15 @@
             days = int(extract_number(message.data["utterance"], lang=self.lang))
         self._report_multi_day_forecast(message, days)
 
     @intent_handler(
         IntentBuilder("one_day_forecast")
         .optionally("query")
         .one_of("weather", "forecast")
-        .require("relative-day")
+        .one_of("relative-day", "today")
         .optionally("location")
         .optionally("unit")
     )
     def handle_one_day_forecast(self, message):
         """Handle forecast for a single day.
 
         Examples:
@@ -167,14 +181,15 @@
 
     @intent_handler(
         IntentBuilder("weather_at_time")
         .optionally("query")
         .one_of("weather", "forecast")
         .require("relative-time")
         .optionally("relative-day")
+        .optionally("today")
         .optionally("location")
         .optionally("unit")
     )
     def handle_weather_at_time(self, message: Message):
         """Handle future weather requests such as: what's the weather tonight?
 
         Args:
@@ -247,15 +262,15 @@
         """Handle simple requests for current temperature.
 
         Examples: "What is the temperature?"
 
         Args:
             message: Message Bus event information from the intent parser
         """
-        self._report_temperature(message, temperature_type="current")
+        self._report_temperature(message)
 
     @intent_handler(
         IntentBuilder("hourly_temperature")
         .optionally("query")
         .require("temperature")
         .require("relative-time")
         .optionally("relative-day")
@@ -270,19 +285,20 @@
             "What is the temperature tomorrow morning?"
 
         Args:
             message: Message Bus event information from the intent parser
         """
         self._report_temperature(message)
 
+    # TODO high low teperatures really only make sense if tied to a daytime
     @intent_handler(
         IntentBuilder("high_temperature")
         .optionally("query")
         .require("high")
-        .optionally("temperature")
+        .require("temperature")
         .optionally("location")
         .optionally("unit")
         .optionally("relative-day")
         .optionally("now")
         .optionally("today")
     )
     def handle_high_temperature(self, message: Message):
@@ -297,15 +313,15 @@
         """
         self._report_temperature(message, temperature_type="high")
 
     @intent_handler(
         IntentBuilder("low_temperature")
         .optionally("query")
         .require("low")
-        .optionally("temperature")
+        .require("temperature")
         .optionally("location")
         .optionally("unit")
         .optionally("relative-day")
         .optionally("now")
         .optionally("today")
     )
     def handle_low_temperature(self, message: Message):
@@ -317,27 +333,29 @@
 
         Args:
             message: Message Bus event information from the intent parser
         """
         self._report_temperature(message, temperature_type="low")
 
     @intent_handler(
-        IntentBuilder("is_hot")
+        IntentBuilder("is_hot_cold")
         .require("confirm-query-current")
         .one_of("hot", "cold")
         .optionally("location")
         .optionally("today")
     )
-    def handle_is_it_hot(self, message: Message):
+    def handle_is_it_hot_or_cold(self, message: Message):
         """Handler for temperature requests such as: is it going to be hot today?
 
         Args:
             message: Message Bus event information from the intent parser
         """
-        self._report_temperature(message, "current")
+        utterance = message.data["utterance"]
+        temperature_type = "high" if self.voc_match(utterance, "hot") else "low"
+        self._report_temperature(message, temperature_type)
 
     @intent_handler(
         IntentBuilder("how_hot_or_cold")
         .optionally("query")
         .one_of("hot", "cold")
         .require("confirm-query")
         .optionally("location")
@@ -479,15 +497,15 @@
         """
         self._report_weather_condition(message, "thunderstorm")
 
     @intent_handler(
         IntentBuilder("next_rain")
         .require("when")
         .optionally("next")
-        .require("precipitation")
+        .one_of("rain", "precipitation")
         .optionally("location")
     )
     def handle_next_precipitation(self, message: Message):
         """Handler for weather requests such as: when will it rain next?
 
         Args:
             message: Message Bus event information from the intent parser
@@ -495,18 +513,14 @@
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         if weather is not None:
             forecast, timeframe = weather.get_next_precipitation(intent_data)
             intent_data.timeframe = timeframe
             dialog = get_dialog_for_timeframe(intent_data, forecast)
             dialog.build_next_precipitation_dialog()
-            spoken_percentage = self.translate(
-                "percentage-number", data=dict(number=dialog.data["percent"])
-            )
-            dialog.data.update(percent=spoken_percentage)
             self._speak_weather(dialog)
 
     @intent_handler(
         IntentBuilder("humidity")
         .require("query")
         .require("humidity")
         .optionally("relative-day")
@@ -524,50 +538,52 @@
             intent_weather = weather.get_weather_for_intent(intent_data)
             dialog = get_dialog_for_timeframe(intent_data, intent_weather)
             dialog.build_humidity_dialog()
             self._speak_weather(dialog)
 
     @intent_handler(
         IntentBuilder("sunrise")  # TODO - this should be in other skill
-        .one_of("query", "when")
+        .require("when")
         .optionally("location")
         .require("sunrise")
         .optionally("today")
         .optionally("relative-day")
     )
     def handle_sunrise(self, message: Message):
         """Handler for weather requests such as: when is the sunrise?
 
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
+        intent_data.timeframe = DAILY
         weather = self._get_weather(intent_data)
         if weather is not None:
             intent_weather = weather.get_weather_for_intent(intent_data)
             dialog = get_dialog_for_timeframe(intent_data, intent_weather)
             dialog.build_sunrise_dialog()
             self._display_sunrise_sunset(intent_weather, intent_data.display_location)
             self._speak_weather(dialog)
 
     @intent_handler(
         IntentBuilder("sunset")  # TODO - this should be in other skill
-        .one_of("query", "when")
+        .require("when")
         .require("sunset")
         .optionally("location")
         .optionally("today")
         .optionally("relative-day")
     )
     def handle_sunset(self, message: Message):
         """Handler for weather requests such as: when is the sunset?
 
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
+        intent_data.timeframe = DAILY
         weather = self._get_weather(intent_data)
         if weather is not None:
             intent_weather = weather.get_weather_for_intent(intent_data)
             dialog = get_dialog_for_timeframe(intent_data, intent_weather)
             dialog.build_sunset_dialog()
             self._display_sunrise_sunset(intent_weather, intent_data.display_location)
             self._speak_weather(dialog)
@@ -576,87 +592,65 @@
         """Display the sunrise and sunset.
 
         Args:
             forecast: daily forecasts to display
             weather_location: the geographical location of the weather
         """
         self.gui.clear()
-        self.gui["weatherDate"] = forecast.date_time.strftime("%A %b %d")
+        self.gui["currentTimezone"] = self._format_dt(forecast.date_time)
         self.gui["weatherLocation"] = weather_location
-        self.gui["sunrise"] = self._format_sunrise_sunset_time(forecast.sunrise)
-        self.gui["sunset"] = self._format_sunrise_sunset_time(forecast.sunset)
-        self.gui["ampm"] = self.config_core["time_format"] == TWELVE_HOUR
+        self.gui["sunrise"] = self._format_time(forecast.sunrise)
+        self.gui["sunset"] = self._format_time(forecast.sunset)
         self.gui.show_page("SunriseSunset.qml")
 
-    def _format_sunrise_sunset_time(self, date_time: datetime) -> str:
-        """Format the sunrise or sunset datetime into a string for GUI display.
-
-        The datetime builtin returns hour in two character format.  Remove the
-        leading zero when present.
-
-        Args:
-            date_time: the sunrise or sunset
-
-        Returns:
-            the value to display on the screen
-        """
-        if self.config_core["time_format"] == TWELVE_HOUR:
-            display_time = date_time.strftime("%I:%M")
-            if display_time.startswith("0"):
-                display_time = display_time[1:]
-        else:
-            display_time = date_time.strftime("%H:%M")
-
-        return display_time
-
     def _report_current_weather(self, message: Message):
         """Handles all requests for current weather conditions.
 
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         if weather is not None:
             self._display_current_conditions(weather, intent_data.display_location)
             dialog = CurrentDialog(intent_data,  weather.current)
             dialog.build_weather_dialog()
             self._speak_weather(dialog)
             dialog = CurrentDialog(intent_data, weather.current)
-            dialog.build_high_low_temperature_dialog()
+            dialog.build_humidity_dialog()
             self._speak_weather(dialog)
             if self.gui.connected:
-                sleep(5)
-                self._display_hourly_forecast(weather, intent_data.display_location)
-                sleep(5)
+                sleep(7)
+                self._display_hourly_forecast(weather.hourly, intent_data.display_location)
+                sleep(7)
                 four_day_forecast = weather.daily[1:5]
                 self._display_multi_day_forecast(four_day_forecast, intent_data)
 
     def _display_current_conditions(self, weather: WeatherReport, weather_location: str):
         """Display current weather conditions on a screen.
 
         This is the first screen that shows.  Others will follow.
 
         Args:
             weather: current weather conditions from Open Weather Maps
             weather_location: the geographical location of the reported weather
         """
         if self.gui.connected:
-            page_name = "CurrentWeather.qml"
-            self.log.info(weather.current.date_time.now().strftime("%a %B %d, %Y"))
             self.gui["weatherCode"] = weather.current.condition.animated_code
-            self.gui["currentTimezone"] = weather.current.date_time.now().strftime("%a %B %d, %Y")
+            self.gui["currentTimezone"] = self._format_dt(weather.current.date_time.now(),
+                                                          incl_time=True)
             self.gui["currentTemperature"] = weather.current.temperature
             self.gui["weatherCondition"] = weather.current.condition.image
             self.gui["weatherLocation"] = weather_location
-            self.gui["highTemperature"] = weather.current.temperature_high
-            self.gui["lowTemperature"] = weather.current.temperature_low
+            self.gui["highTemperature"] = weather.daily[0].temperature_high
+            self.gui["lowTemperature"] = weather.daily[0].temperature_low
+            self.gui["chanceOfPrecipitation"] = weather.current.chance_of_precipitation
             self.gui["windSpeed"] = weather.current.wind_speed
             self.gui["humidity"] = weather.current.humidity
-            self.gui.show_page(page_name)
+            self.gui.show_page("CurrentWeather.qml", override_idle=20)
         else:
             self.enclosure.deactivate_mouth_events()
             self.enclosure.weather_display(
                 weather.current.condition.code, weather.current.temperature
             )
 
     def _report_one_hour_weather(self, message: Message):
@@ -665,53 +659,55 @@
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         if weather is not None:
             try:
-                forecast = weather.get_forecast_for_hour(intent_data)
+                forecast = weather.get_forecast_for_multiple_hours(intent_data)
             except IndexError:
                 self.speak_dialog("forty-eight-hours-available")
             else:
-                dialog = HourlyDialog(intent_data, forecast)
+                dialog = HourlyDialog(intent_data, forecast[0])
                 dialog.build_weather_dialog()
+                self._display_hourly_forecast(forecast, intent_data.display_location)
                 self._speak_weather(dialog)
 
-    def _display_hourly_forecast(self, weather: WeatherReport, weather_location: str):
+    def _display_hourly_forecast(self, weather: List[Weather], weather_location: str):
         """Display hourly forecast on a device that supports the GUI.
 
         On the Mark II this screen is the final for current weather.  It can
         also be shown when the hourly forecast is requested.
 
         :param weather: hourly weather conditions from Open Weather Maps
         """
         hourly_forecast = []
-        for hour_count, hourly in enumerate(weather.hourly):
+        for hour_count, hourly in enumerate(weather):
             if not hour_count:
                 continue
             if hour_count > 4:
                 break
             if self.config_core["time_format"] == TWELVE_HOUR:
                 # The datetime builtin returns hour in two character format.  Convert
                 # to a integer and back again to remove the leading zero when present.
                 hour = int(hourly.date_time.strftime("%I"))
                 am_pm = hourly.date_time.strftime(" %p")
                 formatted_time = str(hour) + am_pm
             else:
                 formatted_time = hourly.date_time.strftime("%H:00")
             hourly_forecast.append(
                 dict(
-                    time=hourly.date_time.strftime(formatted_time),
+                    time=formatted_time,
                     precipitation=hourly.chance_of_precipitation,
                     temperature=hourly.temperature,
                     weatherCondition=hourly.condition.animated_code,
                 )
             )
-        self.gui["weatherCode"] = weather.current.condition.animated_code
+        self.gui["currentTimezone"] = self._format_dt(weather[0].date_time)
+        self.gui["weatherCode"] = weather[0].condition.animated_code
         self.gui["weatherLocation"] = weather_location
         self.gui["hourlyForecast"] = dict(hours=hourly_forecast)
         self.gui.show_page("HourlyForecast.qml")
 
     def _report_one_day_forecast(self, message: Message):
         """Handles all requests for a single day forecast.
 
@@ -723,29 +719,38 @@
         weather = self._get_weather(intent_data)
         if weather is not None:
             forecast = weather.get_forecast_for_date(intent_data)
             dialogs = self._build_forecast_dialogs([forecast], intent_data)
             if self.gui.connected:
                 self._display_one_day(forecast, intent_data)
             for dialog in dialogs:
-                self._speak_weather(dialog)
+                self._speak_weather(dialog, wait=True)
 
     def _display_one_day(self, forecast: Weather, intent_data: WeatherIntent):
         """Display the forecast for a single day on a Mark II.
 
         :param forecast: daily forecasts to display
         """
-        self.gui.clear()
-        self.gui["weatherLocation"] = intent_data.display_location
-        self.gui["weatherCondition"] = forecast.condition.animated_code
-        self.gui["weatherDate"] = forecast.date_time.strftime("%a %B %d, %Y")
-        self.gui["highTemperature"] = forecast.temperature_high
-        self.gui["lowTemperature"] = forecast.temperature_low
-        self.gui["chanceOfPrecipitation"] = str(forecast.chance_of_precipitation)
-        self.gui.show_page("SingleDay.qml")
+        if self.gui.connected:
+            self.gui.clear()
+            self.gui["weatherLocation"] = intent_data.display_location
+            self.gui["weatherCode"] = forecast.condition.animated_code
+            self.gui["weatherDate"] = self._format_dt(forecast.date_time)
+            self.gui["highTemperature"] = forecast.temperature_high
+            self.gui["lowTemperature"] = forecast.temperature_low
+            self.gui["chanceOfPrecipitation"] = str(forecast.chance_of_precipitation)
+            self.gui["windSpeed"] = forecast.wind_speed_max
+            self.gui["humidity"] = forecast.humidity
+            self.gui.show_page("SingleDay.qml")
+        else:
+            self.enclosure.deactivate_mouth_events()
+            self.enclosure.weather_display(
+                forecast.condition.code,
+                (forecast.temperature_high + forecast.temperature_low) / 2
+            )
 
     def _report_multi_day_forecast(self, message: Message, days: int):
         """Handles all requests for multiple day forecasts.
 
         :param message: Message Bus event information from the intent parser
         """
         weather_config = self._get_weather_config(message)
@@ -756,30 +761,30 @@
                 forecast = weather.get_forecast_for_multiple_days(days)
             except IndexError:
                 self.speak_dialog("seven-days-available")
                 forecast = weather.get_forecast_for_multiple_days(7)
             dialogs = self._build_forecast_dialogs(forecast, intent_data)
             self._display_multi_day_forecast(forecast, intent_data)
             for dialog in dialogs:
-                self._speak_weather(dialog)
+                self._speak_weather(dialog, wait=True)
 
     def _report_weekend_forecast(self, message: Message):
         """Handles requests for a weekend forecast.
 
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         if weather is not None:
             forecast = weather.get_weekend_forecast()
             dialogs = self._build_forecast_dialogs(forecast, intent_data)
             self._display_multi_day_forecast(forecast, intent_data)
             for dialog in dialogs:
-                self._speak_weather(dialog)
+                self._speak_weather(dialog, wait=True)
 
     def _build_forecast_dialogs(self, forecast: List[Weather], intent_data: WeatherIntent) -> List[DailyDialog]:
         """
         Build the dialogs for each of the forecast days being reported to the user.
 
         :param forecast: daily forecasts to report
         :param intent_data: information about the intent that was triggered
@@ -869,28 +874,30 @@
             if day_number == 4:
                 break
             display_data.append(
                 dict(
                     weatherCondition=day.condition.animated_code,
                     highTemperature=day.temperature_high,
                     lowTemperature=day.temperature_low,
-                    date=day.date_time.strftime("%a"),
+                    date=nice_weekday(day.date_time, self.lang)[:3],
                 )
             )
         self.gui["forecast"] = dict(all=display_data)
         self.gui.show_page("DailyForecast.qml")
 
     def _report_temperature(self, message: Message, temperature_type: str = None):
         """Handles all requests for a temperature.
 
         Args:
             message: Message Bus event information from the intent parser
             temperature_type: current, high or low temperature
         """
         intent_data = self._get_intent_data(message)
+        if temperature_type in ("high","low",):
+            intent_data.timeframe = "daily"
         weather = self._get_weather(intent_data)
         if weather is not None:
             intent_weather = weather.get_weather_for_intent(intent_data)
             dialog = get_dialog_for_timeframe(intent_data, intent_weather)
             dialog.build_temperature_dialog(temperature_type)
             self._speak_weather(dialog)
 
@@ -917,30 +924,26 @@
             weather: Current, hourly or daily weather forecast
             intent_data: Parsed intent data
             condition: weather condition requested by the user
         """
         dialog = get_dialog_for_timeframe(intent_data, weather)
         intent_match = self.voc_match(weather.condition.category.lower(), condition)
         dialog.build_condition_dialog(intent_match)
-        dialog.data.update(condition=weather.condition.description)
         return dialog
 
     def _report_wind(self, message: Message):
         """Handles all requests for a wind conditions.
 
         Args:
             message: Message Bus event information from the intent parser
         """
         intent_data = self._get_intent_data(message)
         weather = self._get_weather(intent_data)
         if weather is not None:
             intent_weather = weather.get_weather_for_intent(intent_data)
-            intent_weather.wind_direction = self.translate(
-                intent_weather.wind_direction
-            )
             dialog = get_dialog_for_timeframe(intent_data, intent_weather)
             dialog.build_wind_dialog()
             self._speak_weather(dialog)
 
     def _get_intent_data(self, message: Message) -> WeatherIntent:
         """Parse the intent data from the message into data used in the skill.
 
@@ -954,21 +957,22 @@
         try:
             weather_config = self._get_weather_config(message)
             intent_data = WeatherIntent(message, weather_config)
         except ValueError:
             self.speak_dialog("cant-get-forecast")
         else:
             unit = message.data.get("unit")
+            if self.voc_match(intent_data.utterance, "relative-day") or \
+                    self.voc_match(intent_data.utterance, "today"):
+                intent_data.timeframe = DAILY
             if self.voc_match(intent_data.utterance, "relative-time"):
                 intent_data.timeframe = HOURLY
             elif self.voc_match(intent_data.utterance, "later"):
                 intent_data.timeframe = HOURLY
-            elif self.voc_match(intent_data.utterance, "relative-day"):
-                if not self.voc_match(intent_data.utterance, "today"):
-                    intent_data.timeframe = DAILY
+                    
             if unit and self.voc_match(unit, "fahrenheit"):
                 intent_data.config.settings["units"] = "imperial"
             elif unit and self.voc_match(unit, "celsius"):
                 intent_data.config.settings["units"] = "metric"
 
         return intent_data
 
@@ -999,23 +1003,23 @@
             An object representing the data returned by the API
         """
         weather = None
         if intent_data is not None:
             try:
                 weather = get_report(intent_data.config)
             except HTTPError as api_error:
-                self.log.exception("Weather API failure")
+                LOG.exception("Weather API failure")
                 self._handle_api_error(api_error)
             except LocationNotFoundError:
-                self.log.exception("City not found.")
+                LOG.exception("City not found.")
                 self.speak_dialog(
                     "location-not-found", data=dict(location=intent_data.location)
                 )
             except Exception:
-                self.log.exception("Unexpected error retrieving weather")
+                LOG.exception("Unexpected error retrieving weather")
                 self.speak_dialog("cant-get-forecast")
 
         return weather
 
     def _handle_api_error(self, exception: HTTPError):
         """Communicate an error condition to the user.
 
@@ -1023,21 +1027,64 @@
             exception: the HTTPError returned by the API call
         """
         if exception.response.status_code == 401:
             self.bus.emit(Message("mycroft.not.paired"))
         else:
             self.speak_dialog("cant-get-forecast")
 
-    def _speak_weather(self, dialog):
+    def _speak_weather(self, dialog: WeatherDialog, wait: bool = False):
         """Instruct device to speak the contents of the specified dialog.
 
         :param dialog: the dialog that will be spoken
         """
-        self.log.info("Speaking dialog: " + dialog.name)
-        self.speak_dialog(dialog.name, dialog.data, wait=True)
+        LOG.info(f"Speaking dialog: {dialog.name}")
+        self.speak_dialog(dialog.name, dialog.data, wait=wait)
+
+    def _format_dt(self, dt: datetime, incl_time: bool = False) -> str:
+        """Convert a datetime object to a localized string.
+
+        Args:
+            dt: datetime object
+            incl_time: whether to include the time in the output
+
+        Returns:
+            A localized string representing the datetime
+        """
+        dt_strings = get_date_strings(dt, lang=self.lang)
+        wd_abbr = dt_strings["weekday_string"][:3].capitalize()
+        month = dt_strings["month_string"].capitalize()
+        day = dt_strings["day_string"]
+        time = dt_strings["time_string"]
+
+        if self.date_format == "MDY":
+            dt_string = f"{wd_abbr}, {month} {day}"
+        else:
+            dt_string = f"{wd_abbr}, {day} {month}"
+        if incl_time:
+            return dt_string + f" {time}"
+        
+        return dt_string
+    
+    def _format_time(self, dt: datetime) -> str:
+        """Format the datetime into a string for GUI display.
+
+        The datetime builtin returns hour in two character format.  Remove the
+        leading zero when present.
+
+        Args:
+            date_time: the sunrise or sunset
+
+        Returns:
+            the value to display on the screen
+        """
+        return nice_time(dt,
+                         self.lang,
+                         speech=False,
+                         use_24hour = self.use_24h,
+                         use_ampm = not self.use_24h)
 
     @skill_api_method
     def get_current_weather_homescreen(self, message=None):
         """Get the current temperature and weather condition.
         Returns:
             Dict: {
                 weather_temp: current temperature
@@ -1052,23 +1099,25 @@
         """
         try:
             weather_config = self._get_weather_config(message=message)
             weather = get_report(weather_config)
 
             result = dict(
                 weather_temp=weather.current.temperature,
-                high_temperature=weather.current.temperature_high,
-                low_temperature=weather.current.temperature_low,
+                high_temperature=weather.daily[0].temperature_high,
+                low_temperature=weather.daily[0].temperature_low,
                 weather_code=weather.current.condition.code,
                 condition_category=weather.current.condition.category,
-                condition_description=weather.current.condition.description,
+                condition_description=self.translate(
+                    weather.current.condition.description
+                ),
                 system_unit=weather_config.scale
             )
 
             self.bus.emit(Message("skill-ovos-weather.openvoiceos.weather.response",
                                   {"report": result}))
             return result
         except Exception:
-            self.log.exception("Unexpected error getting weather for skill API.")
+            LOG.exception("Unexpected error getting weather for skill API.")
 
     def stop(self):
         self.gui.release()
```

## skill_ovos_weather/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 1
-VERSION_ALPHA = 8
+VERSION_ALPHA = 9
 # END_VERSION_BLOCK
```

## skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-local.dialog

```diff
@@ -1,3 +1,3 @@
 # Informing that an the requested condition is not in the forecast
-Es wird {condition} für heute vorhergesagt 
-Für heute wird {condition} erwartet
+Nein, es wird {condition} für heute vorhergesagt 
+Nein, für heute wird {condition} erwartet
```

## skill_ovos_weather/locale/de-de/dialog/current/current-condition-not-expected-location.dialog

```diff
@@ -1,3 +1,3 @@
 # Informing that an the requested condition is not in the forecast
-In {location} wird {condition} für heute vorhergesagt
-Für heute wird {condition} in {location} erwartet
+Nein, in {location} wird {condition} für heute vorhergesagt
+Nein, für heute wird {condition} in {location} erwartet
```

## skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog

```diff
@@ -1,3 +1,3 @@
 # Informing that an the requested condition is not in the forecast
-Es wird {condition} für {day} vorhergesagt 
-Für {day} wird {condition} erwartet
+Nein, es wird {condition} für {day} vorhergesagt 
+Nein, für {day} wird {condition} erwartet
```

## skill_ovos_weather/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog

```diff
@@ -1,3 +1,3 @@
 # Informing that an the requested condition is not in the forecast
-In {location} wird {condition} für {day} vorhergesagt
-Für {day} wird {condition} in {location} erwartet
+Nein, In {location} wird {condition} für {day} vorhergesagt
+Nein, für {day} wird {condition} in {location} erwartet
```

## skill_ovos_weather/locale/de-de/dialog/daily/daily-humidity-local.dialog

```diff
@@ -1,2 +1 @@
-The humidity {day} will be {percent}
 Für {day} ist mit Luftfeuchte von {percent} zu rechnen
```

## skill_ovos_weather/locale/de-de/dialog/daily/daily-weather-local.dialog

```diff
@@ -1,3 +1,3 @@
-{day} wird {condition} vorausgesagt, mit maximal {high_temperature} und minimal {low_temperature}
+{day} wird {condition} vorausgesagt, mit maximal {high_temperature} und minimal {low_temperature} grad.
 {day} werden wir maximal {high_temperature} und minimal {low_temperature} Grad haben, {condition} wird erwartet
-Die Vorhersage {day} sieht ein Maximum von {high_temperature} und ein Minimum von {low_temperature}, {condition} ist vorausgesagt
+Die Vorhersage {day} sieht ein Maximum von {high_temperature} und ein Minimum von {low_temperature} grad, {condition} ist vorausgesagt
```

## skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog

```diff
@@ -1,2 +1,2 @@
 # Wenn der Benutzer fragt, ob es regnet, aber keine Wolke oder Alternative vorhergesagt wird
-Nein, die {time} -Prognose schlägt dies nicht vor
+Nein, die {time} -Prognose geht nicht davon aus.
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## skill_ovos_weather/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog

```diff
@@ -1,2 +1,2 @@
 # Wenn der Benutzer fragt, ob es sich um eine Bedingung handelt, dies jedoch nicht
-Nein, die {time} Vorhersage in {location} schlägt dies nicht vor
+Nein, die {time} Vorhersage in {location} geht nicht davon aus.
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog

```diff
@@ -1,2 +1,2 @@
-es ist zu {percent} um {time} mit {precipitation} zu rechnen.
-es ist mit einer wahrscheinlichkeit von {percent} um {time} mit {precipitation} zu rechnen.
+es ist zu {percent} {time} mit {precipitation} zu rechnen.
+es ist mit einer wahrscheinlichkeit von {percent} {time} mit {precipitation} zu rechnen.
```

## skill_ovos_weather/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog

```diff
@@ -1,2 +1,2 @@
-in {location} ist zu {percent} mit {precipitation} um {time} zu rechnen
-es ist um {time} mit einer wahrscheinlichkeit von {percent} mit {precipitation} in {location} zu rechnen
+in {location} ist zu {percent} {time} mit {precipitation} zu rechnen
+es ist {time} mit einer wahrscheinlichkeit von {percent} mit {precipitation} in {location} zu rechnen
```

## skill_ovos_weather/locale/de-de/vocabulary/sunrise.voc

```diff
@@ -1,5 +1,6 @@
 Sonnenaufgang
+sonne auf
 Sonne aufgehen
 Dämmerung
 Tagesanbruch
 Tag anbrechen
```

## skill_ovos_weather/locale/de-de/vocabulary/sunset.voc

```diff
@@ -1,3 +1,4 @@
 Sonnenuntergang
+sonne unter
 Sonne untergehen
 Dämmerung
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/clouds.voc

```diff
@@ -1,2 +1,6 @@
 # Freimachen von Wettertypen, die verwendet werden in der Behandlungsroutine für "Wird es bewölkt sein"
-(bewölkt|Wolke|Wolken|wenige Wolken|vereinzelte Wolken)
+bewölkt
+bewölkung
+Wolke
+Wolken
+bedeckt
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/fog.voc

```diff
@@ -1,4 +1,2 @@
 Nebel
 neblig
-Nebel
-neblig
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/humidity.voc

```diff
@@ -1,3 +1,3 @@
 feucht
 Luftfeuchtigkeit
-dampfig
+luftfeuchte
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/precipitation.voc

```diff
@@ -1,5 +1 @@
-regnerisch
-verregnet
 Niederschlag
-regnen
-regnet es
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/rain.voc

```diff
@@ -1,2 +1,5 @@
 # Regen Bedingungen welche zum Beispiel in "wird es heute regnen" genutzt werden
-(leichter Regen|Regen|Nieselregen|Sprühregen|Niederschlag)
+regen
+regnen
+regnet
+regnerisch
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/snow.voc

```diff
@@ -1,2 +1,4 @@
 Schneeverhältnisse, wie sie z.B. im Umgang mit "Wird es morgen regnen" verwendet werden
-(schnee|schneien|schneeregen|schneeregnen)
+schnee
+schneien
+schneit
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/thunderstorm.voc

```diff
@@ -1,2 +1,4 @@
-# Klare Wettertypen im Handler für "Wird es stürmen?"
-(Sturm|stürmisch|stürmisch)
+gewitter
+gewittert
+donnert
+donner
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## skill_ovos_weather/locale/de-de/vocabulary/condition/windy.voc

```diff
@@ -1,7 +1,7 @@
 Wind
 windig
+windet
 Winde
-Windgeschwindigkeit
-windig
-stürmend
-wehend
+Sturm
+stürmt
+stürmen
```

## skill_ovos_weather/locale/de-de/vocabulary/date-time/now.voc

```diff
@@ -1,2 +1,5 @@
 Aktuell
 jetzt
+gerade
+momentan
+im moment
```

## skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-day.voc

```diff
@@ -1,9 +1,7 @@
-heute
-heutige
 morgen
 morgige
 montag
 montags
 am montag
 dienstag
 dienstags
```

## skill_ovos_weather/locale/de-de/vocabulary/date-time/relative-time.voc

```diff
@@ -6,7 +6,55 @@
 nachmittags
 abend
 abends
 nacht
 nachts
 mitternacht
 mitternachts
+01:00 uhr
+1 uhr
+02:00 uhr
+2 uhr
+03:00 uhr
+3 uhr
+04:00 uhr
+4 uhr
+05:00 uhr
+5 uhr
+06:00 uhr
+6 uhr
+07:00 uhr
+7 uhr
+08:00 uhr
+8 uhr
+09:00 uhr
+9 uhr
+10:00 uhr
+10 uhr
+11:00 uhr
+11 uhr
+12:00 uhr
+12 uhr
+13:00 uhr
+13 uhr
+14:00 uhr
+14 uhr
+15:00 uhr
+15 uhr
+16:00 uhr
+16 uhr
+17:00 uhr
+17 uhr
+18:00 uhr
+18 uhr
+19:00 uhr
+19 uhr
+20:00 uhr
+20 uhr
+21:00 uhr
+21 uhr
+22:00 uhr
+22 uhr
+23:00 uhr
+23 uhr
+24:00 uhr
+24 uhr
```

## skill_ovos_weather/locale/de-de/vocabulary/query/query.voc

```diff
@@ -1,6 +1,5 @@
 wie
 was ist
-was ist
 was wird
 erzähle (mir|uns) (etwas über|)
 gib mir
```

## skill_ovos_weather/locale/de-de/vocabulary/query/when.voc

```diff
@@ -1,5 +1,4 @@
 wann
-wenn es
-wann wird es
-wann ist es
-wann
+wann wird (es|)
+wann ist (es|)
+wann war (es|)
```

## skill_ovos_weather/locale/de-de/vocabulary/temperature/cold.voc

```diff
@@ -1,4 +1,2 @@
 kalt
 kühl
-gefrierend
-kühl
```

## skill_ovos_weather/locale/de-de/vocabulary/temperature/high.voc

```diff
@@ -1,4 +1,6 @@
 Höchstwert
+Höchsttemperatur
+hoch
 höchste(n|r|s)
 Maximum
 Maximum
```

## skill_ovos_weather/locale/de-de/vocabulary/temperature/low.voc

```diff
@@ -1,4 +1,6 @@
 Tiefstwert
+Tiefsttemperatur
 niedrigste
+tief
 Minimum
-Minimum
+minimale
```

## skill_ovos_weather/ovos_skill_weather.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-skill-weather
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: ovos skill plugin
 Home-page: https://github.com/OpenVoiceOS/skill-ovos-weather
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # <img src='https://rawgithub.com/FortAwesome/Font-Awesome/master/svgs/solid/sun.svg' card_color='#FEE255' width='50' height='50' style='vertical-align:bottom'/> Weather
         Weather conditions and forecasts
```

## skill_ovos_weather/ovos_skill_weather.egg-info/SOURCES.txt

```diff
@@ -3,71 +3,166 @@
 README.md
 __init__.py
 setup.py
 version.py
 locale/ca-es/dialog/and.dialog
 locale/ca-es/dialog/percentage-number.dialog
 locale/ca-es/dialog/condition/ash.dialog
+locale/ca-es/dialog/condition/clear-sky.dialog
 locale/ca-es/dialog/condition/clear.dialog
 locale/ca-es/dialog/condition/clouds.dialog
+locale/ca-es/dialog/condition/depositing-rime-fog.dialog
+locale/ca-es/dialog/condition/drizzle-dense-intensity.dialog
+locale/ca-es/dialog/condition/drizzle-light-intensity.dialog
+locale/ca-es/dialog/condition/drizzle-moderate-intensity.dialog
 locale/ca-es/dialog/condition/drizzle.dialog
 locale/ca-es/dialog/condition/dust.dialog
+locale/ca-es/dialog/condition/fog.dialog
+locale/ca-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/ca-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/ca-es/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/ca-es/dialog/condition/freezing-rain-light-intensity.dialog
 locale/ca-es/dialog/condition/haze.dialog
+locale/ca-es/dialog/condition/heavy-rain.dialog
+locale/ca-es/dialog/condition/heavy-snow-fall.dialog
+locale/ca-es/dialog/condition/heavy-snow-showers.dialog
+locale/ca-es/dialog/condition/humidity.dialog
+locale/ca-es/dialog/condition/mainly-clear.dialog
 locale/ca-es/dialog/condition/mist.dialog
+locale/ca-es/dialog/condition/moderate-rain-showers.dialog
+locale/ca-es/dialog/condition/moderate-rain.dialog
+locale/ca-es/dialog/condition/moderate-snow-fall.dialog
+locale/ca-es/dialog/condition/overcast.dialog
+locale/ca-es/dialog/condition/partly-cloudy.dialog
 locale/ca-es/dialog/condition/rain.dialog
+locale/ca-es/dialog/condition/slight-rain-showers.dialog
+locale/ca-es/dialog/condition/slight-rain.dialog
+locale/ca-es/dialog/condition/slight-snow-fall.dialog
+locale/ca-es/dialog/condition/slight-snow-showers.dialog
 locale/ca-es/dialog/condition/smoke.dialog
+locale/ca-es/dialog/condition/snow-grains.dialog
 locale/ca-es/dialog/condition/snow.dialog
 locale/ca-es/dialog/condition/squall.dialog
+locale/ca-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/ca-es/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/ca-es/dialog/condition/thunderstorm.dialog
 locale/ca-es/dialog/condition/tornado.dialog
+locale/ca-es/dialog/condition/violent-rain-showers.dialog
 locale/ca-es/dialog/current/current-condition-expected-local.dialog
 locale/ca-es/dialog/current/current-condition-expected-location.dialog
+locale/ca-es/dialog/current/current-condition-not-expected-local.dialog
+locale/ca-es/dialog/current/current-condition-not-expected-location.dialog
+locale/ca-es/dialog/current/current-humidity-local.dialog
+locale/ca-es/dialog/current/current-humidity-location.dialog
+locale/ca-es/dialog/current/current-sunrise-future-local.dialog
+locale/ca-es/dialog/current/current-sunrise-future-location.dialog
+locale/ca-es/dialog/current/current-sunrise-past-local.dialog
+locale/ca-es/dialog/current/current-sunrise-past-location.dialog
+locale/ca-es/dialog/current/current-sunset-future-local.dialog
+locale/ca-es/dialog/current/current-sunset-future-location.dialog
+locale/ca-es/dialog/current/current-sunset-past-local.dialog
+locale/ca-es/dialog/current/current-sunset-past-location.dialog
+locale/ca-es/dialog/current/current-temperature-high-low.dialog
+locale/ca-es/dialog/current/current-temperature-local.dialog
+locale/ca-es/dialog/current/current-temperature-location.dialog
+locale/ca-es/dialog/current/current-weather-local.dialog
+locale/ca-es/dialog/current/current-weather-location.dialog
+locale/ca-es/dialog/current/current-wind-light-local.dialog
+locale/ca-es/dialog/current/current-wind-light-location.dialog
+locale/ca-es/dialog/current/current-wind-moderate-local.dialog
+locale/ca-es/dialog/current/current-wind-moderate-location.dialog
+locale/ca-es/dialog/current/current-wind-strong-local.dialog
+locale/ca-es/dialog/current/current-wind-strong-location.dialog
+locale/ca-es/dialog/current/currrent-clouds-alternative-local.dialog
+locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
 locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
+locale/ca-es/dialog/daily/daily-condition-not-expected-local.dialog
+locale/ca-es/dialog/daily/daily-condition-not-expected-location.dialog
+locale/ca-es/dialog/daily/daily-humidity-local.dialog
+locale/ca-es/dialog/daily/daily-humidity-location.dialog
+locale/ca-es/dialog/daily/daily-precipitation-next-local.dialog
+locale/ca-es/dialog/daily/daily-precipitation-next-location.dialog
+locale/ca-es/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/ca-es/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/ca-es/dialog/daily/daily-sunrise-local.dialog
+locale/ca-es/dialog/daily/daily-sunrise-location.dialog
+locale/ca-es/dialog/daily/daily-sunset-local.dialog
+locale/ca-es/dialog/daily/daily-sunset-location.dialog
+locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
+locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
+locale/ca-es/dialog/daily/daily-temperature-local.dialog
+locale/ca-es/dialog/daily/daily-temperature-location.dialog
+locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
+locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
+locale/ca-es/dialog/daily/daily-weather-local.dialog
+locale/ca-es/dialog/daily/daily-weather-location.dialog
 locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
+locale/ca-es/dialog/daily/daily-wind-light-local.dialog
+locale/ca-es/dialog/daily/daily-wind-light-location.dialog
+locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
+locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
+locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
+locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
 locale/ca-es/dialog/direction/east.dialog
 locale/ca-es/dialog/direction/north.dialog
 locale/ca-es/dialog/direction/northeast.dialog
 locale/ca-es/dialog/direction/northwest.dialog
 locale/ca-es/dialog/direction/south.dialog
 locale/ca-es/dialog/direction/southeast.dialog
 locale/ca-es/dialog/direction/southwest.dialog
 locale/ca-es/dialog/direction/west.dialog
 locale/ca-es/dialog/error/cant-get-forecast.dialog
+locale/ca-es/dialog/error/forty-eight-hours-available.dialog
+locale/ca-es/dialog/error/location-not-found.dialog
 locale/ca-es/dialog/error/no-forecast.dialog
+locale/ca-es/dialog/error/seven-days-available.dialog
 locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
 locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
 locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
 locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
 locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
 locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+locale/ca-es/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/ca-es/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
+locale/ca-es/dialog/hourly/hourly-temperature-location.dialog
+locale/ca-es/dialog/hourly/hourly-weather-local.dialog
+locale/ca-es/dialog/hourly/hourly-weather-location.dialog
 locale/ca-es/dialog/unit/celsius.dialog
 locale/ca-es/dialog/unit/fahrenheit.dialog
-locale/ca-es/dialog/unit/meters per second.dialog
+locale/ca-es/dialog/unit/inch.dialog
+locale/ca-es/dialog/unit/meter per second.dialog
 locale/ca-es/dialog/unit/miles per hour.dialog
+locale/ca-es/dialog/unit/millimeter.dialog
+locale/ca-es/dialog/weekly/weekly-condition.dialog
 locale/ca-es/dialog/weekly/weekly-temperature.dialog
 locale/ca-es/regex/location.rx
 locale/ca-es/vocabulary/forecast.voc
 locale/ca-es/vocabulary/location.voc
+locale/ca-es/vocabulary/outside.voc
 locale/ca-es/vocabulary/sunrise.voc
 locale/ca-es/vocabulary/sunset.voc
 locale/ca-es/vocabulary/weather.voc
 locale/ca-es/vocabulary/condition/clear.voc
 locale/ca-es/vocabulary/condition/clouds.voc
+locale/ca-es/vocabulary/condition/do-i-need-an-umbrella.intent
 locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
 locale/ca-es/vocabulary/condition/fog.voc
 locale/ca-es/vocabulary/condition/humidity.voc
 locale/ca-es/vocabulary/condition/precipitation.voc
 locale/ca-es/vocabulary/condition/rain.voc
 locale/ca-es/vocabulary/condition/snow.voc
 locale/ca-es/vocabulary/condition/thunderstorm.voc
 locale/ca-es/vocabulary/condition/windy.voc
 locale/ca-es/vocabulary/date-time/couple.voc
+locale/ca-es/vocabulary/date-time/few.voc
 locale/ca-es/vocabulary/date-time/later.voc
 locale/ca-es/vocabulary/date-time/next.voc
 locale/ca-es/vocabulary/date-time/now.voc
+locale/ca-es/vocabulary/date-time/number-days.voc
 locale/ca-es/vocabulary/date-time/relative-day.voc
 locale/ca-es/vocabulary/date-time/relative-time.voc
 locale/ca-es/vocabulary/date-time/today.voc
 locale/ca-es/vocabulary/date-time/week.voc
 locale/ca-es/vocabulary/date-time/weekend.voc
 locale/ca-es/vocabulary/query/confirm-query-current.voc
 locale/ca-es/vocabulary/query/confirm-query-future.voc
@@ -79,73 +174,334 @@
 locale/ca-es/vocabulary/temperature/high.voc
 locale/ca-es/vocabulary/temperature/hot.voc
 locale/ca-es/vocabulary/temperature/low.voc
 locale/ca-es/vocabulary/temperature/temperature.voc
 locale/ca-es/vocabulary/unit/fahrenheit.voc
 locale/ca-es/vocabulary/unit/unit.entity
 locale/ca-es/vocabulary/unit/unit.voc
+locale/cs-cz/dialog/and.dialog
+locale/cs-cz/dialog/percentage-number.dialog
+locale/cs-cz/dialog/condition/ash.dialog
+locale/cs-cz/dialog/condition/clear-sky.dialog
+locale/cs-cz/dialog/condition/clear.dialog
+locale/cs-cz/dialog/condition/clouds.dialog
+locale/cs-cz/dialog/condition/depositing-rime-fog.dialog
+locale/cs-cz/dialog/condition/drizzle-dense-intensity.dialog
+locale/cs-cz/dialog/condition/drizzle-light-intensity.dialog
+locale/cs-cz/dialog/condition/drizzle-moderate-intensity.dialog
+locale/cs-cz/dialog/condition/drizzle.dialog
+locale/cs-cz/dialog/condition/dust.dialog
+locale/cs-cz/dialog/condition/fog.dialog
+locale/cs-cz/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/cs-cz/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/cs-cz/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/cs-cz/dialog/condition/freezing-rain-light-intensity.dialog
+locale/cs-cz/dialog/condition/haze.dialog
+locale/cs-cz/dialog/condition/heavy-rain.dialog
+locale/cs-cz/dialog/condition/heavy-snow-fall.dialog
+locale/cs-cz/dialog/condition/heavy-snow-showers.dialog
+locale/cs-cz/dialog/condition/humidity.dialog
+locale/cs-cz/dialog/condition/mainly-clear.dialog
+locale/cs-cz/dialog/condition/mist.dialog
+locale/cs-cz/dialog/condition/moderate-rain-showers.dialog
+locale/cs-cz/dialog/condition/moderate-rain.dialog
+locale/cs-cz/dialog/condition/moderate-snow-fall.dialog
+locale/cs-cz/dialog/condition/overcast.dialog
+locale/cs-cz/dialog/condition/partly-cloudy.dialog
+locale/cs-cz/dialog/condition/rain.dialog
+locale/cs-cz/dialog/condition/slight-rain-showers.dialog
+locale/cs-cz/dialog/condition/slight-rain.dialog
+locale/cs-cz/dialog/condition/slight-snow-fall.dialog
+locale/cs-cz/dialog/condition/slight-snow-showers.dialog
+locale/cs-cz/dialog/condition/smoke.dialog
+locale/cs-cz/dialog/condition/snow-grains.dialog
+locale/cs-cz/dialog/condition/snow.dialog
+locale/cs-cz/dialog/condition/squall.dialog
+locale/cs-cz/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/cs-cz/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/cs-cz/dialog/condition/thunderstorm.dialog
+locale/cs-cz/dialog/condition/tornado.dialog
+locale/cs-cz/dialog/condition/violent-rain-showers.dialog
+locale/cs-cz/dialog/current/current-condition-expected-local.dialog
+locale/cs-cz/dialog/current/current-condition-expected-location.dialog
+locale/cs-cz/dialog/current/current-condition-not-expected-local.dialog
+locale/cs-cz/dialog/current/current-condition-not-expected-location.dialog
+locale/cs-cz/dialog/current/current-humidity-local.dialog
+locale/cs-cz/dialog/current/current-humidity-location.dialog
+locale/cs-cz/dialog/current/current-sunrise-future-local.dialog
+locale/cs-cz/dialog/current/current-sunrise-future-location.dialog
+locale/cs-cz/dialog/current/current-sunrise-past-local.dialog
+locale/cs-cz/dialog/current/current-sunrise-past-location.dialog
+locale/cs-cz/dialog/current/current-sunset-future-local.dialog
+locale/cs-cz/dialog/current/current-sunset-future-location.dialog
+locale/cs-cz/dialog/current/current-sunset-past-local.dialog
+locale/cs-cz/dialog/current/current-sunset-past-location.dialog
+locale/cs-cz/dialog/current/current-temperature-local.dialog
+locale/cs-cz/dialog/current/current-temperature-location.dialog
+locale/cs-cz/dialog/current/current-weather-local.dialog
+locale/cs-cz/dialog/current/current-weather-location.dialog
+locale/cs-cz/dialog/current/current-wind-light-local.dialog
+locale/cs-cz/dialog/current/current-wind-light-location.dialog
+locale/cs-cz/dialog/current/current-wind-moderate-local.dialog
+locale/cs-cz/dialog/current/current-wind-moderate-location.dialog
+locale/cs-cz/dialog/current/current-wind-strong-local.dialog
+locale/cs-cz/dialog/current/current-wind-strong-location.dialog
+locale/cs-cz/dialog/current/currrent-clouds-alternative-local.dialog
+locale/cs-cz/dialog/daily/daily-condition-expected-local.dialog
+locale/cs-cz/dialog/daily/daily-condition-expected-location.dialog
+locale/cs-cz/dialog/daily/daily-condition-not-expected-local.dialog
+locale/cs-cz/dialog/daily/daily-condition-not-expected-location.dialog
+locale/cs-cz/dialog/daily/daily-humidity-local.dialog
+locale/cs-cz/dialog/daily/daily-humidity-location.dialog
+locale/cs-cz/dialog/daily/daily-precipitation-next-local.dialog
+locale/cs-cz/dialog/daily/daily-precipitation-next-location.dialog
+locale/cs-cz/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/cs-cz/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/cs-cz/dialog/daily/daily-sunrise-local.dialog
+locale/cs-cz/dialog/daily/daily-sunrise-location.dialog
+locale/cs-cz/dialog/daily/daily-sunset-local.dialog
+locale/cs-cz/dialog/daily/daily-sunset-location.dialog
+locale/cs-cz/dialog/daily/daily-temperature-high-local.dialog
+locale/cs-cz/dialog/daily/daily-temperature-high-location.dialog
+locale/cs-cz/dialog/daily/daily-temperature-local.dialog
+locale/cs-cz/dialog/daily/daily-temperature-location.dialog
+locale/cs-cz/dialog/daily/daily-temperature-low-local.dialog
+locale/cs-cz/dialog/daily/daily-temperature-low-location.dialog
+locale/cs-cz/dialog/daily/daily-weather-local.dialog
+locale/cs-cz/dialog/daily/daily-weather-location.dialog
+locale/cs-cz/dialog/daily/daily-wind-light-local.dialog
+locale/cs-cz/dialog/daily/daily-wind-light-location.dialog
+locale/cs-cz/dialog/daily/daily-wind-moderate-local.dialog
+locale/cs-cz/dialog/daily/daily-wind-moderate-location.dialog
+locale/cs-cz/dialog/daily/daily-wind-strong-local.dialog
+locale/cs-cz/dialog/daily/daily-wind-strong-location.dialog
+locale/cs-cz/dialog/direction/east.dialog
+locale/cs-cz/dialog/direction/north.dialog
+locale/cs-cz/dialog/direction/northeast.dialog
+locale/cs-cz/dialog/direction/northwest.dialog
+locale/cs-cz/dialog/direction/south.dialog
+locale/cs-cz/dialog/direction/southeast.dialog
+locale/cs-cz/dialog/direction/southwest.dialog
+locale/cs-cz/dialog/direction/west.dialog
+locale/cs-cz/dialog/error/cant-get-forecast.dialog
+locale/cs-cz/dialog/error/forty-eight-hours-available.dialog
+locale/cs-cz/dialog/error/location-not-found.dialog
+locale/cs-cz/dialog/error/no-forecast.dialog
+locale/cs-cz/dialog/error/seven-days-available.dialog
+locale/cs-cz/dialog/hourly/hourly-condition-expected-local.dialog
+locale/cs-cz/dialog/hourly/hourly-condition-expected-location.dialog
+locale/cs-cz/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/cs-cz/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/cs-cz/dialog/hourly/hourly-temperature-local.dialog
+locale/cs-cz/dialog/hourly/hourly-temperature-location.dialog
+locale/cs-cz/dialog/hourly/hourly-weather-local.dialog
+locale/cs-cz/dialog/hourly/hourly-weather-location.dialog
+locale/cs-cz/dialog/unit/celsius.dialog
+locale/cs-cz/dialog/unit/fahrenheit.dialog
+locale/cs-cz/dialog/unit/inch.dialog
+locale/cs-cz/dialog/unit/meter per second.dialog
+locale/cs-cz/dialog/unit/miles per hour.dialog
+locale/cs-cz/dialog/unit/millimeter.dialog
+locale/cs-cz/dialog/weekly/weekly-condition.dialog
+locale/cs-cz/dialog/weekly/weekly-temperature.dialog
+locale/cs-cz/regex/location.rx
+locale/cs-cz/vocabulary/forecast.voc
+locale/cs-cz/vocabulary/location.voc
+locale/cs-cz/vocabulary/outside.voc
+locale/cs-cz/vocabulary/sunrise.voc
+locale/cs-cz/vocabulary/sunset.voc
+locale/cs-cz/vocabulary/weather.voc
+locale/cs-cz/vocabulary/condition/clear.voc
+locale/cs-cz/vocabulary/condition/clouds.voc
+locale/cs-cz/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/cs-cz/vocabulary/condition/fog.voc
+locale/cs-cz/vocabulary/condition/humidity.voc
+locale/cs-cz/vocabulary/condition/precipitation.voc
+locale/cs-cz/vocabulary/condition/rain.voc
+locale/cs-cz/vocabulary/condition/snow.voc
+locale/cs-cz/vocabulary/condition/thunderstorm.voc
+locale/cs-cz/vocabulary/condition/windy.voc
+locale/cs-cz/vocabulary/date-time/couple.voc
+locale/cs-cz/vocabulary/date-time/few.voc
+locale/cs-cz/vocabulary/date-time/later.voc
+locale/cs-cz/vocabulary/date-time/next.voc
+locale/cs-cz/vocabulary/date-time/now.voc
+locale/cs-cz/vocabulary/date-time/number-days.voc
+locale/cs-cz/vocabulary/date-time/relative-day.voc
+locale/cs-cz/vocabulary/date-time/relative-time.voc
+locale/cs-cz/vocabulary/date-time/today.voc
+locale/cs-cz/vocabulary/date-time/week.voc
+locale/cs-cz/vocabulary/date-time/weekend.voc
+locale/cs-cz/vocabulary/query/confirm-query-current.voc
+locale/cs-cz/vocabulary/query/confirm-query-future.voc
+locale/cs-cz/vocabulary/query/confirm-query.voc
+locale/cs-cz/vocabulary/query/how.voc
+locale/cs-cz/vocabulary/query/query.voc
+locale/cs-cz/vocabulary/query/when.voc
+locale/cs-cz/vocabulary/temperature/cold.voc
+locale/cs-cz/vocabulary/temperature/high.voc
+locale/cs-cz/vocabulary/temperature/hot.voc
+locale/cs-cz/vocabulary/temperature/low.voc
+locale/cs-cz/vocabulary/temperature/temperature.voc
+locale/cs-cz/vocabulary/unit/fahrenheit.voc
+locale/cs-cz/vocabulary/unit/unit.entity
+locale/cs-cz/vocabulary/unit/unit.voc
 locale/da-dk/dialog/and.dialog
 locale/da-dk/dialog/percentage-number.dialog
 locale/da-dk/dialog/condition/ash.dialog
+locale/da-dk/dialog/condition/clear-sky.dialog
 locale/da-dk/dialog/condition/clear.dialog
 locale/da-dk/dialog/condition/clouds.dialog
+locale/da-dk/dialog/condition/depositing-rime-fog.dialog
+locale/da-dk/dialog/condition/drizzle-dense-intensity.dialog
+locale/da-dk/dialog/condition/drizzle-light-intensity.dialog
+locale/da-dk/dialog/condition/drizzle-moderate-intensity.dialog
 locale/da-dk/dialog/condition/drizzle.dialog
 locale/da-dk/dialog/condition/dust.dialog
+locale/da-dk/dialog/condition/fog.dialog
+locale/da-dk/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/da-dk/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/da-dk/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/da-dk/dialog/condition/freezing-rain-light-intensity.dialog
 locale/da-dk/dialog/condition/haze.dialog
+locale/da-dk/dialog/condition/heavy-rain.dialog
+locale/da-dk/dialog/condition/heavy-snow-fall.dialog
+locale/da-dk/dialog/condition/heavy-snow-showers.dialog
+locale/da-dk/dialog/condition/humidity.dialog
+locale/da-dk/dialog/condition/mainly-clear.dialog
 locale/da-dk/dialog/condition/mist.dialog
+locale/da-dk/dialog/condition/moderate-rain-showers.dialog
+locale/da-dk/dialog/condition/moderate-rain.dialog
+locale/da-dk/dialog/condition/moderate-snow-fall.dialog
+locale/da-dk/dialog/condition/overcast.dialog
+locale/da-dk/dialog/condition/partly-cloudy.dialog
 locale/da-dk/dialog/condition/rain.dialog
+locale/da-dk/dialog/condition/slight-rain-showers.dialog
+locale/da-dk/dialog/condition/slight-rain.dialog
+locale/da-dk/dialog/condition/slight-snow-fall.dialog
+locale/da-dk/dialog/condition/slight-snow-showers.dialog
 locale/da-dk/dialog/condition/smoke.dialog
+locale/da-dk/dialog/condition/snow-grains.dialog
 locale/da-dk/dialog/condition/snow.dialog
 locale/da-dk/dialog/condition/squall.dialog
+locale/da-dk/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/da-dk/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/da-dk/dialog/condition/thunderstorm.dialog
 locale/da-dk/dialog/condition/tornado.dialog
+locale/da-dk/dialog/condition/violent-rain-showers.dialog
 locale/da-dk/dialog/current/current-condition-expected-local.dialog
 locale/da-dk/dialog/current/current-condition-expected-location.dialog
+locale/da-dk/dialog/current/current-condition-not-expected-local.dialog
+locale/da-dk/dialog/current/current-condition-not-expected-location.dialog
+locale/da-dk/dialog/current/current-humidity-local.dialog
+locale/da-dk/dialog/current/current-humidity-location.dialog
+locale/da-dk/dialog/current/current-sunrise-future-local.dialog
+locale/da-dk/dialog/current/current-sunrise-future-location.dialog
+locale/da-dk/dialog/current/current-sunrise-past-local.dialog
+locale/da-dk/dialog/current/current-sunrise-past-location.dialog
+locale/da-dk/dialog/current/current-sunset-future-local.dialog
+locale/da-dk/dialog/current/current-sunset-future-location.dialog
+locale/da-dk/dialog/current/current-sunset-past-local.dialog
+locale/da-dk/dialog/current/current-sunset-past-location.dialog
+locale/da-dk/dialog/current/current-temperature-local.dialog
+locale/da-dk/dialog/current/current-temperature-location.dialog
+locale/da-dk/dialog/current/current-weather-local.dialog
+locale/da-dk/dialog/current/current-weather-location.dialog
+locale/da-dk/dialog/current/current-wind-light-local.dialog
+locale/da-dk/dialog/current/current-wind-light-location.dialog
+locale/da-dk/dialog/current/current-wind-moderate-local.dialog
+locale/da-dk/dialog/current/current-wind-moderate-location.dialog
+locale/da-dk/dialog/current/current-wind-strong-local.dialog
+locale/da-dk/dialog/current/current-wind-strong-location.dialog
+locale/da-dk/dialog/current/currrent-clouds-alternative-local.dialog
+locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
 locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
+locale/da-dk/dialog/daily/daily-condition-not-expected-local.dialog
+locale/da-dk/dialog/daily/daily-condition-not-expected-location.dialog
+locale/da-dk/dialog/daily/daily-humidity-local.dialog
+locale/da-dk/dialog/daily/daily-humidity-location.dialog
+locale/da-dk/dialog/daily/daily-precipitation-next-local.dialog
+locale/da-dk/dialog/daily/daily-precipitation-next-location.dialog
+locale/da-dk/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/da-dk/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/da-dk/dialog/daily/daily-sunrise-local.dialog
+locale/da-dk/dialog/daily/daily-sunrise-location.dialog
+locale/da-dk/dialog/daily/daily-sunset-local.dialog
+locale/da-dk/dialog/daily/daily-sunset-location.dialog
+locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
+locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
+locale/da-dk/dialog/daily/daily-temperature-local.dialog
+locale/da-dk/dialog/daily/daily-temperature-location.dialog
+locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
+locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
+locale/da-dk/dialog/daily/daily-weather-local.dialog
+locale/da-dk/dialog/daily/daily-weather-location.dialog
+locale/da-dk/dialog/daily/daily-wind-light-local.dialog
+locale/da-dk/dialog/daily/daily-wind-light-location.dialog
+locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
+locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
+locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
+locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
 locale/da-dk/dialog/direction/east.dialog
 locale/da-dk/dialog/direction/north.dialog
 locale/da-dk/dialog/direction/northeast.dialog
 locale/da-dk/dialog/direction/northwest.dialog
 locale/da-dk/dialog/direction/south.dialog
 locale/da-dk/dialog/direction/southeast.dialog
 locale/da-dk/dialog/direction/southwest.dialog
 locale/da-dk/dialog/direction/west.dialog
 locale/da-dk/dialog/error/cant-get-forecast.dialog
+locale/da-dk/dialog/error/forty-eight-hours-available.dialog
+locale/da-dk/dialog/error/location-not-found.dialog
 locale/da-dk/dialog/error/no-forecast.dialog
+locale/da-dk/dialog/error/seven-days-available.dialog
 locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
 locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
 locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
 locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
 locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
 locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
+locale/da-dk/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/da-dk/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
+locale/da-dk/dialog/hourly/hourly-temperature-location.dialog
+locale/da-dk/dialog/hourly/hourly-weather-local.dialog
+locale/da-dk/dialog/hourly/hourly-weather-location.dialog
 locale/da-dk/dialog/unit/celsius.dialog
 locale/da-dk/dialog/unit/fahrenheit.dialog
-locale/da-dk/dialog/unit/meters per second.dialog
+locale/da-dk/dialog/unit/inch.dialog
+locale/da-dk/dialog/unit/meter per second.dialog
 locale/da-dk/dialog/unit/miles per hour.dialog
+locale/da-dk/dialog/unit/millimeter.dialog
+locale/da-dk/dialog/weekly/weekly-condition.dialog
 locale/da-dk/dialog/weekly/weekly-temperature.dialog
 locale/da-dk/regex/location.rx
 locale/da-dk/vocabulary/forecast.voc
 locale/da-dk/vocabulary/location.voc
+locale/da-dk/vocabulary/outside.voc
 locale/da-dk/vocabulary/sunrise.voc
 locale/da-dk/vocabulary/sunset.voc
 locale/da-dk/vocabulary/weather.voc
 locale/da-dk/vocabulary/condition/clear.voc
 locale/da-dk/vocabulary/condition/clouds.voc
 locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
+locale/da-dk/vocabulary/condition/do-i-need-an-umbrella.intent
 locale/da-dk/vocabulary/condition/fog.voc
 locale/da-dk/vocabulary/condition/humidity.voc
 locale/da-dk/vocabulary/condition/precipitation.voc
 locale/da-dk/vocabulary/condition/rain.voc
 locale/da-dk/vocabulary/condition/snow.voc
 locale/da-dk/vocabulary/condition/thunderstorm.voc
 locale/da-dk/vocabulary/condition/windy.voc
 locale/da-dk/vocabulary/date-time/couple.voc
+locale/da-dk/vocabulary/date-time/few.voc
 locale/da-dk/vocabulary/date-time/later.voc
 locale/da-dk/vocabulary/date-time/next.voc
 locale/da-dk/vocabulary/date-time/now.voc
+locale/da-dk/vocabulary/date-time/number-days.voc
 locale/da-dk/vocabulary/date-time/relative-day.voc
 locale/da-dk/vocabulary/date-time/relative-time.voc
 locale/da-dk/vocabulary/date-time/today.voc
 locale/da-dk/vocabulary/date-time/week.voc
 locale/da-dk/vocabulary/date-time/weekend.voc
 locale/da-dk/vocabulary/query/confirm-query-current.voc
 locale/da-dk/vocabulary/query/confirm-query-future.voc
@@ -160,47 +516,70 @@
 locale/da-dk/vocabulary/temperature/temperature.voc
 locale/da-dk/vocabulary/unit/fahrenheit.voc
 locale/da-dk/vocabulary/unit/unit.entity
 locale/da-dk/vocabulary/unit/unit.voc
 locale/de-de/dialog/and.dialog
 locale/de-de/dialog/percentage-number.dialog
 locale/de-de/dialog/condition/ash.dialog
+locale/de-de/dialog/condition/clear-sky.dialog
 locale/de-de/dialog/condition/clear.dialog
 locale/de-de/dialog/condition/clouds.dialog
+locale/de-de/dialog/condition/depositing-rime-fog.dialog
+locale/de-de/dialog/condition/drizzle-dense-intensity.dialog
+locale/de-de/dialog/condition/drizzle-light-intensity.dialog
+locale/de-de/dialog/condition/drizzle-moderate-intensity.dialog
 locale/de-de/dialog/condition/drizzle.dialog
 locale/de-de/dialog/condition/dust.dialog
+locale/de-de/dialog/condition/fog.dialog
+locale/de-de/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/de-de/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/de-de/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/de-de/dialog/condition/freezing-rain-light-intensity.dialog
 locale/de-de/dialog/condition/haze.dialog
+locale/de-de/dialog/condition/heavy-rain.dialog
+locale/de-de/dialog/condition/heavy-snow-fall.dialog
+locale/de-de/dialog/condition/heavy-snow-showers.dialog
+locale/de-de/dialog/condition/humidity.dialog
+locale/de-de/dialog/condition/mainly-clear.dialog
 locale/de-de/dialog/condition/mist.dialog
+locale/de-de/dialog/condition/moderate-rain-showers.dialog
+locale/de-de/dialog/condition/moderate-rain.dialog
+locale/de-de/dialog/condition/moderate-snow-fall.dialog
+locale/de-de/dialog/condition/overcast.dialog
+locale/de-de/dialog/condition/partly-cloudy.dialog
 locale/de-de/dialog/condition/rain.dialog
+locale/de-de/dialog/condition/slight-rain-showers.dialog
+locale/de-de/dialog/condition/slight-rain.dialog
+locale/de-de/dialog/condition/slight-snow-fall.dialog
+locale/de-de/dialog/condition/slight-snow-showers.dialog
 locale/de-de/dialog/condition/smoke.dialog
+locale/de-de/dialog/condition/snow-grains.dialog
 locale/de-de/dialog/condition/snow.dialog
 locale/de-de/dialog/condition/squall.dialog
+locale/de-de/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/de-de/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/de-de/dialog/condition/thunderstorm.dialog
 locale/de-de/dialog/condition/tornado.dialog
+locale/de-de/dialog/condition/violent-rain-showers.dialog
 locale/de-de/dialog/current/current-condition-expected-local.dialog
 locale/de-de/dialog/current/current-condition-expected-location.dialog
 locale/de-de/dialog/current/current-condition-not-expected-local.dialog
 locale/de-de/dialog/current/current-condition-not-expected-location.dialog
 locale/de-de/dialog/current/current-humidity-local.dialog
 locale/de-de/dialog/current/current-humidity-location.dialog
 locale/de-de/dialog/current/current-sunrise-future-local.dialog
 locale/de-de/dialog/current/current-sunrise-future-location.dialog
 locale/de-de/dialog/current/current-sunrise-past-local.dialog
 locale/de-de/dialog/current/current-sunrise-past-location.dialog
 locale/de-de/dialog/current/current-sunset-future-local.dialog
 locale/de-de/dialog/current/current-sunset-future-location.dialog
 locale/de-de/dialog/current/current-sunset-past-local.dialog
 locale/de-de/dialog/current/current-sunset-past-location.dialog
-locale/de-de/dialog/current/current-temperature-high-local.dialog
-locale/de-de/dialog/current/current-temperature-high-location.dialog
-locale/de-de/dialog/current/current-temperature-high-low.dialog
 locale/de-de/dialog/current/current-temperature-local.dialog
 locale/de-de/dialog/current/current-temperature-location.dialog
-locale/de-de/dialog/current/current-temperature-low-local.dialog
-locale/de-de/dialog/current/current-temperature-low-location.dialog
 locale/de-de/dialog/current/current-weather-local.dialog
 locale/de-de/dialog/current/current-weather-location.dialog
 locale/de-de/dialog/current/current-wind-light-local.dialog
 locale/de-de/dialog/current/current-wind-light-location.dialog
 locale/de-de/dialog/current/current-wind-moderate-local.dialog
 locale/de-de/dialog/current/current-wind-moderate-location.dialog
 locale/de-de/dialog/current/current-wind-strong-local.dialog
@@ -218,26 +597,33 @@
 locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
 locale/de-de/dialog/daily/daily-sunrise-local.dialog
 locale/de-de/dialog/daily/daily-sunrise-location.dialog
 locale/de-de/dialog/daily/daily-sunset-local.dialog
 locale/de-de/dialog/daily/daily-sunset-location.dialog
 locale/de-de/dialog/daily/daily-temperature-high-local.dialog
 locale/de-de/dialog/daily/daily-temperature-high-location.dialog
+locale/de-de/dialog/daily/daily-temperature-high-low-local.dialog
+locale/de-de/dialog/daily/daily-temperature-high-low-location.dialog
 locale/de-de/dialog/daily/daily-temperature-local.dialog
 locale/de-de/dialog/daily/daily-temperature-location.dialog
 locale/de-de/dialog/daily/daily-temperature-low-local.dialog
 locale/de-de/dialog/daily/daily-temperature-low-location.dialog
 locale/de-de/dialog/daily/daily-weather-local.dialog
 locale/de-de/dialog/daily/daily-weather-location.dialog
 locale/de-de/dialog/daily/daily-wind-light-local.dialog
 locale/de-de/dialog/daily/daily-wind-light-location.dialog
 locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
 locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
 locale/de-de/dialog/daily/daily-wind-strong-local.dialog
 locale/de-de/dialog/daily/daily-wind-strong-location.dialog
+locale/de-de/dialog/date-time/afternoon.dialog
+locale/de-de/dialog/date-time/early morning.dialog
+locale/de-de/dialog/date-time/evening.dialog
+locale/de-de/dialog/date-time/morning.dialog
+locale/de-de/dialog/date-time/overnight.dialog
 locale/de-de/dialog/direction/east.dialog
 locale/de-de/dialog/direction/north.dialog
 locale/de-de/dialog/direction/northeast.dialog
 locale/de-de/dialog/direction/northwest.dialog
 locale/de-de/dialog/direction/south.dialog
 locale/de-de/dialog/direction/southeast.dialog
 locale/de-de/dialog/direction/southwest.dialog
@@ -257,38 +643,43 @@
 locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
 locale/de-de/dialog/hourly/hourly-temperature-local.dialog
 locale/de-de/dialog/hourly/hourly-temperature-location.dialog
 locale/de-de/dialog/hourly/hourly-weather-local.dialog
 locale/de-de/dialog/hourly/hourly-weather-location.dialog
 locale/de-de/dialog/unit/celsius.dialog
 locale/de-de/dialog/unit/fahrenheit.dialog
-locale/de-de/dialog/unit/meters per second.dialog
+locale/de-de/dialog/unit/inch.dialog
+locale/de-de/dialog/unit/meter per second.dialog
 locale/de-de/dialog/unit/miles per hour.dialog
+locale/de-de/dialog/unit/millimeter.dialog
 locale/de-de/dialog/weekly/weekly-condition.dialog
 locale/de-de/dialog/weekly/weekly-temperature.dialog
 locale/de-de/regex/location.rx
 locale/de-de/vocabulary/forecast.voc
 locale/de-de/vocabulary/location.voc
+locale/de-de/vocabulary/outside.voc
 locale/de-de/vocabulary/sunrise.voc
 locale/de-de/vocabulary/sunset.voc
 locale/de-de/vocabulary/weather.voc
 locale/de-de/vocabulary/condition/clear.voc
 locale/de-de/vocabulary/condition/clouds.voc
 locale/de-de/vocabulary/condition/do-i-need-an-umbrella.intent
 locale/de-de/vocabulary/condition/fog.voc
 locale/de-de/vocabulary/condition/humidity.voc
 locale/de-de/vocabulary/condition/precipitation.voc
 locale/de-de/vocabulary/condition/rain.voc
 locale/de-de/vocabulary/condition/snow.voc
 locale/de-de/vocabulary/condition/thunderstorm.voc
 locale/de-de/vocabulary/condition/windy.voc
 locale/de-de/vocabulary/date-time/couple.voc
+locale/de-de/vocabulary/date-time/few.voc
 locale/de-de/vocabulary/date-time/later.voc
 locale/de-de/vocabulary/date-time/next.voc
 locale/de-de/vocabulary/date-time/now.voc
+locale/de-de/vocabulary/date-time/number-days.voc
 locale/de-de/vocabulary/date-time/relative-day.voc
 locale/de-de/vocabulary/date-time/relative-time.voc
 locale/de-de/vocabulary/date-time/today.voc
 locale/de-de/vocabulary/date-time/week.voc
 locale/de-de/vocabulary/date-time/weekend.voc
 locale/de-de/vocabulary/query/confirm-query-current.voc
 locale/de-de/vocabulary/query/confirm-query-future.voc
@@ -357,21 +748,16 @@
 locale/en-us/dialog/current/current-sunrise-future-location.dialog
 locale/en-us/dialog/current/current-sunrise-past-local.dialog
 locale/en-us/dialog/current/current-sunrise-past-location.dialog
 locale/en-us/dialog/current/current-sunset-future-local.dialog
 locale/en-us/dialog/current/current-sunset-future-location.dialog
 locale/en-us/dialog/current/current-sunset-past-local.dialog
 locale/en-us/dialog/current/current-sunset-past-location.dialog
-locale/en-us/dialog/current/current-temperature-high-local.dialog
-locale/en-us/dialog/current/current-temperature-high-location.dialog
-locale/en-us/dialog/current/current-temperature-high-low.dialog
 locale/en-us/dialog/current/current-temperature-local.dialog
 locale/en-us/dialog/current/current-temperature-location.dialog
-locale/en-us/dialog/current/current-temperature-low-local.dialog
-locale/en-us/dialog/current/current-temperature-low-location.dialog
 locale/en-us/dialog/current/current-weather-local.dialog
 locale/en-us/dialog/current/current-weather-location.dialog
 locale/en-us/dialog/current/current-wind-light-local.dialog
 locale/en-us/dialog/current/current-wind-light-location.dialog
 locale/en-us/dialog/current/current-wind-moderate-local.dialog
 locale/en-us/dialog/current/current-wind-moderate-location.dialog
 locale/en-us/dialog/current/current-wind-strong-local.dialog
@@ -389,26 +775,33 @@
 locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
 locale/en-us/dialog/daily/daily-sunrise-local.dialog
 locale/en-us/dialog/daily/daily-sunrise-location.dialog
 locale/en-us/dialog/daily/daily-sunset-local.dialog
 locale/en-us/dialog/daily/daily-sunset-location.dialog
 locale/en-us/dialog/daily/daily-temperature-high-local.dialog
 locale/en-us/dialog/daily/daily-temperature-high-location.dialog
+locale/en-us/dialog/daily/daily-temperature-high-low-local.dialog
+locale/en-us/dialog/daily/daily-temperature-high-low-location.dialog
 locale/en-us/dialog/daily/daily-temperature-local.dialog
 locale/en-us/dialog/daily/daily-temperature-location.dialog
 locale/en-us/dialog/daily/daily-temperature-low-local.dialog
 locale/en-us/dialog/daily/daily-temperature-low-location.dialog
 locale/en-us/dialog/daily/daily-weather-local.dialog
 locale/en-us/dialog/daily/daily-weather-location.dialog
 locale/en-us/dialog/daily/daily-wind-light-local.dialog
 locale/en-us/dialog/daily/daily-wind-light-location.dialog
 locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
 locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
 locale/en-us/dialog/daily/daily-wind-strong-local.dialog
 locale/en-us/dialog/daily/daily-wind-strong-location.dialog
+locale/en-us/dialog/date-time/afternoon.dialog
+locale/en-us/dialog/date-time/early morning.dialog
+locale/en-us/dialog/date-time/evening.dialog
+locale/en-us/dialog/date-time/morning.dialog
+locale/en-us/dialog/date-time/overnight.dialog
 locale/en-us/dialog/direction/east.dialog
 locale/en-us/dialog/direction/north.dialog
 locale/en-us/dialog/direction/northeast.dialog
 locale/en-us/dialog/direction/northwest.dialog
 locale/en-us/dialog/direction/south.dialog
 locale/en-us/dialog/direction/southeast.dialog
 locale/en-us/dialog/direction/southwest.dialog
@@ -425,22 +818,22 @@
 locale/en-us/dialog/hourly/hourly-temperature-local.dialog
 locale/en-us/dialog/hourly/hourly-temperature-location.dialog
 locale/en-us/dialog/hourly/hourly-weather-local.dialog
 locale/en-us/dialog/hourly/hourly-weather-location.dialog
 locale/en-us/dialog/unit/celsius.dialog
 locale/en-us/dialog/unit/fahrenheit.dialog
 locale/en-us/dialog/unit/inch.dialog
-locale/en-us/dialog/unit/meters per second.dialog
+locale/en-us/dialog/unit/kilometer per hour.dialog
+locale/en-us/dialog/unit/meter per second.dialog
 locale/en-us/dialog/unit/miles per hour.dialog
 locale/en-us/dialog/unit/millimeter.dialog
 locale/en-us/dialog/weekly/weekly-condition.dialog
 locale/en-us/dialog/weekly/weekly-temperature.dialog
 locale/en-us/regex/location.rx
 locale/en-us/vocabulary/forecast.voc
-locale/en-us/vocabulary/like.voc
 locale/en-us/vocabulary/location.voc
 locale/en-us/vocabulary/outside.voc
 locale/en-us/vocabulary/sunrise.voc
 locale/en-us/vocabulary/sunset.voc
 locale/en-us/vocabulary/weather.voc
 locale/en-us/vocabulary/condition/clear.voc
 locale/en-us/vocabulary/condition/clouds.voc
@@ -476,48 +869,70 @@
 locale/en-us/vocabulary/temperature/temperature.voc
 locale/en-us/vocabulary/unit/fahrenheit.voc
 locale/en-us/vocabulary/unit/unit.entity
 locale/en-us/vocabulary/unit/unit.voc
 locale/es-es/dialog/and.dialog
 locale/es-es/dialog/percentage-number.dialog
 locale/es-es/dialog/condition/ash.dialog
+locale/es-es/dialog/condition/clear-sky.dialog
 locale/es-es/dialog/condition/clear.dialog
 locale/es-es/dialog/condition/clouds.dialog
+locale/es-es/dialog/condition/depositing-rime-fog.dialog
+locale/es-es/dialog/condition/drizzle-dense-intensity.dialog
+locale/es-es/dialog/condition/drizzle-light-intensity.dialog
+locale/es-es/dialog/condition/drizzle-moderate-intensity.dialog
 locale/es-es/dialog/condition/drizzle.dialog
 locale/es-es/dialog/condition/dust.dialog
+locale/es-es/dialog/condition/fog.dialog
+locale/es-es/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/es-es/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/es-es/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/es-es/dialog/condition/freezing-rain-light-intensity.dialog
 locale/es-es/dialog/condition/haze.dialog
+locale/es-es/dialog/condition/heavy-rain.dialog
+locale/es-es/dialog/condition/heavy-snow-fall.dialog
+locale/es-es/dialog/condition/heavy-snow-showers.dialog
 locale/es-es/dialog/condition/humidity.dialog
+locale/es-es/dialog/condition/mainly-clear.dialog
 locale/es-es/dialog/condition/mist.dialog
+locale/es-es/dialog/condition/moderate-rain-showers.dialog
+locale/es-es/dialog/condition/moderate-rain.dialog
+locale/es-es/dialog/condition/moderate-snow-fall.dialog
+locale/es-es/dialog/condition/overcast.dialog
+locale/es-es/dialog/condition/partly-cloudy.dialog
 locale/es-es/dialog/condition/rain.dialog
+locale/es-es/dialog/condition/slight-rain-showers.dialog
+locale/es-es/dialog/condition/slight-rain.dialog
+locale/es-es/dialog/condition/slight-snow-fall.dialog
+locale/es-es/dialog/condition/slight-snow-showers.dialog
 locale/es-es/dialog/condition/smoke.dialog
+locale/es-es/dialog/condition/snow-grains.dialog
 locale/es-es/dialog/condition/snow.dialog
 locale/es-es/dialog/condition/squall.dialog
+locale/es-es/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/es-es/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/es-es/dialog/condition/thunderstorm.dialog
 locale/es-es/dialog/condition/tornado.dialog
+locale/es-es/dialog/condition/violent-rain-showers.dialog
 locale/es-es/dialog/current/current-condition-expected-local.dialog
 locale/es-es/dialog/current/current-condition-expected-location.dialog
 locale/es-es/dialog/current/current-condition-not-expected-local.dialog
 locale/es-es/dialog/current/current-condition-not-expected-location.dialog
 locale/es-es/dialog/current/current-humidity-local.dialog
 locale/es-es/dialog/current/current-humidity-location.dialog
 locale/es-es/dialog/current/current-sunrise-future-local.dialog
 locale/es-es/dialog/current/current-sunrise-future-location.dialog
 locale/es-es/dialog/current/current-sunrise-past-local.dialog
 locale/es-es/dialog/current/current-sunrise-past-location.dialog
 locale/es-es/dialog/current/current-sunset-future-local.dialog
 locale/es-es/dialog/current/current-sunset-future-location.dialog
 locale/es-es/dialog/current/current-sunset-past-local.dialog
 locale/es-es/dialog/current/current-sunset-past-location.dialog
-locale/es-es/dialog/current/current-temperature-high-local.dialog
-locale/es-es/dialog/current/current-temperature-high-location.dialog
-locale/es-es/dialog/current/current-temperature-high-low.dialog
 locale/es-es/dialog/current/current-temperature-local.dialog
 locale/es-es/dialog/current/current-temperature-location.dialog
-locale/es-es/dialog/current/current-temperature-low-local.dialog
-locale/es-es/dialog/current/current-temperature-low-location.dialog
 locale/es-es/dialog/current/current-weather-local.dialog
 locale/es-es/dialog/current/current-weather-location.dialog
 locale/es-es/dialog/current/current-wind-light-local.dialog
 locale/es-es/dialog/current/current-wind-light-location.dialog
 locale/es-es/dialog/current/current-wind-moderate-local.dialog
 locale/es-es/dialog/current/current-wind-moderate-location.dialog
 locale/es-es/dialog/current/current-wind-strong-local.dialog
@@ -535,14 +950,16 @@
 locale/es-es/dialog/daily/daily-precipitation-next-none-location.dialog
 locale/es-es/dialog/daily/daily-sunrise-local.dialog
 locale/es-es/dialog/daily/daily-sunrise-location.dialog
 locale/es-es/dialog/daily/daily-sunset-local.dialog
 locale/es-es/dialog/daily/daily-sunset-location.dialog
 locale/es-es/dialog/daily/daily-temperature-high-local.dialog
 locale/es-es/dialog/daily/daily-temperature-high-location.dialog
+locale/es-es/dialog/daily/daily-temperature-high-low-local.dialog
+locale/es-es/dialog/daily/daily-temperature-high-low-location.dialog
 locale/es-es/dialog/daily/daily-temperature-local.dialog
 locale/es-es/dialog/daily/daily-temperature-location.dialog
 locale/es-es/dialog/daily/daily-temperature-low-local.dialog
 locale/es-es/dialog/daily/daily-temperature-low-location.dialog
 locale/es-es/dialog/daily/daily-weather-local.dialog
 locale/es-es/dialog/daily/daily-weather-location.dialog
 locale/es-es/dialog/daily/daily-wind-light-local.dialog
@@ -570,21 +987,22 @@
 locale/es-es/dialog/hourly/hourly-precipitation-next-location.dialog
 locale/es-es/dialog/hourly/hourly-temperature-local.dialog
 locale/es-es/dialog/hourly/hourly-temperature-location.dialog
 locale/es-es/dialog/hourly/hourly-weather-local.dialog
 locale/es-es/dialog/hourly/hourly-weather-location.dialog
 locale/es-es/dialog/unit/celsius.dialog
 locale/es-es/dialog/unit/fahrenheit.dialog
-locale/es-es/dialog/unit/meters per second.dialog
+locale/es-es/dialog/unit/inch.dialog
+locale/es-es/dialog/unit/meter per second.dialog
 locale/es-es/dialog/unit/miles per hour.dialog
+locale/es-es/dialog/unit/millimeter.dialog
 locale/es-es/dialog/weekly/weekly-condition.dialog
 locale/es-es/dialog/weekly/weekly-temperature.dialog
 locale/es-es/regex/location.rx
 locale/es-es/vocabulary/forecast.voc
-locale/es-es/vocabulary/like.voc
 locale/es-es/vocabulary/location.voc
 locale/es-es/vocabulary/outside.voc
 locale/es-es/vocabulary/sunrise.voc
 locale/es-es/vocabulary/sunset.voc
 locale/es-es/vocabulary/weather.voc
 locale/es-es/vocabulary/condition/clear.voc
 locale/es-es/vocabulary/condition/clouds.voc
@@ -617,52 +1035,181 @@
 locale/es-es/vocabulary/temperature/high.voc
 locale/es-es/vocabulary/temperature/hot.voc
 locale/es-es/vocabulary/temperature/low.voc
 locale/es-es/vocabulary/temperature/temperature.voc
 locale/es-es/vocabulary/unit/fahrenheit.voc
 locale/es-es/vocabulary/unit/unit.entity
 locale/es-es/vocabulary/unit/unit.voc
+locale/fr-fr/dialog/and.dialog
 locale/fr-fr/dialog/percentage-number.dialog
 locale/fr-fr/dialog/condition/ash.dialog
+locale/fr-fr/dialog/condition/clear-sky.dialog
 locale/fr-fr/dialog/condition/clear.dialog
 locale/fr-fr/dialog/condition/clouds.dialog
+locale/fr-fr/dialog/condition/depositing-rime-fog.dialog
+locale/fr-fr/dialog/condition/drizzle-dense-intensity.dialog
+locale/fr-fr/dialog/condition/drizzle-light-intensity.dialog
+locale/fr-fr/dialog/condition/drizzle-moderate-intensity.dialog
 locale/fr-fr/dialog/condition/drizzle.dialog
 locale/fr-fr/dialog/condition/dust.dialog
+locale/fr-fr/dialog/condition/fog.dialog
+locale/fr-fr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/fr-fr/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/fr-fr/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/fr-fr/dialog/condition/freezing-rain-light-intensity.dialog
 locale/fr-fr/dialog/condition/haze.dialog
+locale/fr-fr/dialog/condition/heavy-rain.dialog
+locale/fr-fr/dialog/condition/heavy-snow-fall.dialog
+locale/fr-fr/dialog/condition/heavy-snow-showers.dialog
+locale/fr-fr/dialog/condition/humidity.dialog
+locale/fr-fr/dialog/condition/mainly-clear.dialog
 locale/fr-fr/dialog/condition/mist.dialog
+locale/fr-fr/dialog/condition/moderate-rain-showers.dialog
+locale/fr-fr/dialog/condition/moderate-rain.dialog
+locale/fr-fr/dialog/condition/moderate-snow-fall.dialog
+locale/fr-fr/dialog/condition/overcast.dialog
+locale/fr-fr/dialog/condition/partly-cloudy.dialog
 locale/fr-fr/dialog/condition/rain.dialog
+locale/fr-fr/dialog/condition/slight-rain-showers.dialog
+locale/fr-fr/dialog/condition/slight-rain.dialog
+locale/fr-fr/dialog/condition/slight-snow-fall.dialog
+locale/fr-fr/dialog/condition/slight-snow-showers.dialog
 locale/fr-fr/dialog/condition/smoke.dialog
+locale/fr-fr/dialog/condition/snow-grains.dialog
 locale/fr-fr/dialog/condition/snow.dialog
 locale/fr-fr/dialog/condition/squall.dialog
+locale/fr-fr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/fr-fr/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/fr-fr/dialog/condition/thunderstorm.dialog
 locale/fr-fr/dialog/condition/tornado.dialog
+locale/fr-fr/dialog/condition/violent-rain-showers.dialog
+locale/fr-fr/dialog/current/current-condition-expected-local.dialog
+locale/fr-fr/dialog/current/current-condition-expected-location.dialog
+locale/fr-fr/dialog/current/current-condition-not-expected-local.dialog
+locale/fr-fr/dialog/current/current-condition-not-expected-location.dialog
+locale/fr-fr/dialog/current/current-humidity-local.dialog
+locale/fr-fr/dialog/current/current-humidity-location.dialog
+locale/fr-fr/dialog/current/current-sunrise-future-local.dialog
+locale/fr-fr/dialog/current/current-sunrise-future-location.dialog
+locale/fr-fr/dialog/current/current-sunrise-past-local.dialog
+locale/fr-fr/dialog/current/current-sunrise-past-location.dialog
+locale/fr-fr/dialog/current/current-sunset-future-local.dialog
+locale/fr-fr/dialog/current/current-sunset-future-location.dialog
+locale/fr-fr/dialog/current/current-sunset-past-local.dialog
+locale/fr-fr/dialog/current/current-sunset-past-location.dialog
+locale/fr-fr/dialog/current/current-temperature-local.dialog
+locale/fr-fr/dialog/current/current-temperature-location.dialog
+locale/fr-fr/dialog/current/current-weather-local.dialog
+locale/fr-fr/dialog/current/current-weather-location.dialog
+locale/fr-fr/dialog/current/current-wind-light-local.dialog
+locale/fr-fr/dialog/current/current-wind-light-location.dialog
+locale/fr-fr/dialog/current/current-wind-moderate-local.dialog
+locale/fr-fr/dialog/current/current-wind-moderate-location.dialog
+locale/fr-fr/dialog/current/current-wind-strong-local.dialog
+locale/fr-fr/dialog/current/current-wind-strong-location.dialog
+locale/fr-fr/dialog/current/currrent-clouds-alternative-local.dialog
+locale/fr-fr/dialog/daily/daily-condition-expected-local.dialog
+locale/fr-fr/dialog/daily/daily-condition-expected-location.dialog
+locale/fr-fr/dialog/daily/daily-condition-not-expected-local.dialog
+locale/fr-fr/dialog/daily/daily-condition-not-expected-location.dialog
+locale/fr-fr/dialog/daily/daily-humidity-local.dialog
+locale/fr-fr/dialog/daily/daily-humidity-location.dialog
+locale/fr-fr/dialog/daily/daily-precipitation-next-local.dialog
+locale/fr-fr/dialog/daily/daily-precipitation-next-location.dialog
+locale/fr-fr/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/fr-fr/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/fr-fr/dialog/daily/daily-sunrise-local.dialog
+locale/fr-fr/dialog/daily/daily-sunrise-location.dialog
+locale/fr-fr/dialog/daily/daily-sunset-local.dialog
+locale/fr-fr/dialog/daily/daily-sunset-location.dialog
+locale/fr-fr/dialog/daily/daily-temperature-high-local.dialog
+locale/fr-fr/dialog/daily/daily-temperature-high-location.dialog
+locale/fr-fr/dialog/daily/daily-temperature-local.dialog
+locale/fr-fr/dialog/daily/daily-temperature-location.dialog
+locale/fr-fr/dialog/daily/daily-temperature-low-local.dialog
+locale/fr-fr/dialog/daily/daily-temperature-low-location.dialog
+locale/fr-fr/dialog/daily/daily-weather-local.dialog
+locale/fr-fr/dialog/daily/daily-weather-location.dialog
+locale/fr-fr/dialog/daily/daily-wind-light-local.dialog
+locale/fr-fr/dialog/daily/daily-wind-light-location.dialog
+locale/fr-fr/dialog/daily/daily-wind-moderate-local.dialog
+locale/fr-fr/dialog/daily/daily-wind-moderate-location.dialog
+locale/fr-fr/dialog/daily/daily-wind-strong-local.dialog
+locale/fr-fr/dialog/daily/daily-wind-strong-location.dialog
 locale/fr-fr/dialog/direction/east.dialog
 locale/fr-fr/dialog/direction/north.dialog
 locale/fr-fr/dialog/direction/northeast.dialog
 locale/fr-fr/dialog/direction/northwest.dialog
 locale/fr-fr/dialog/direction/south.dialog
 locale/fr-fr/dialog/direction/southeast.dialog
 locale/fr-fr/dialog/direction/southwest.dialog
 locale/fr-fr/dialog/direction/west.dialog
+locale/fr-fr/dialog/error/cant-get-forecast.dialog
+locale/fr-fr/dialog/error/forty-eight-hours-available.dialog
+locale/fr-fr/dialog/error/location-not-found.dialog
+locale/fr-fr/dialog/error/no-forecast.dialog
+locale/fr-fr/dialog/error/seven-days-available.dialog
+locale/fr-fr/dialog/hourly/hourly-condition-expected-local.dialog
+locale/fr-fr/dialog/hourly/hourly-condition-expected-location.dialog
+locale/fr-fr/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/fr-fr/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/fr-fr/dialog/hourly/hourly-temperature-local.dialog
+locale/fr-fr/dialog/hourly/hourly-temperature-location.dialog
+locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
+locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
 locale/fr-fr/dialog/unit/celsius.dialog
 locale/fr-fr/dialog/unit/fahrenheit.dialog
-locale/fr-fr/dialog/unit/meters per second.dialog
+locale/fr-fr/dialog/unit/inch.dialog
+locale/fr-fr/dialog/unit/meter per second.dialog
 locale/fr-fr/dialog/unit/miles per hour.dialog
+locale/fr-fr/dialog/unit/millimeter.dialog
+locale/fr-fr/dialog/weekly/weekly-condition.dialog
+locale/fr-fr/dialog/weekly/weekly-temperature.dialog
 locale/fr-fr/regex/location.rx
 locale/fr-fr/vocabulary/forecast.voc
 locale/fr-fr/vocabulary/location.voc
+locale/fr-fr/vocabulary/outside.voc
 locale/fr-fr/vocabulary/sunrise.voc
 locale/fr-fr/vocabulary/sunset.voc
 locale/fr-fr/vocabulary/weather.voc
+locale/fr-fr/vocabulary/condition/clear.voc
+locale/fr-fr/vocabulary/condition/clouds.voc
+locale/fr-fr/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/fr-fr/vocabulary/condition/fog.voc
 locale/fr-fr/vocabulary/condition/humidity.voc
 locale/fr-fr/vocabulary/condition/precipitation.voc
+locale/fr-fr/vocabulary/condition/rain.voc
+locale/fr-fr/vocabulary/condition/snow.voc
+locale/fr-fr/vocabulary/condition/thunderstorm.voc
 locale/fr-fr/vocabulary/condition/windy.voc
+locale/fr-fr/vocabulary/date-time/couple.voc
+locale/fr-fr/vocabulary/date-time/few.voc
 locale/fr-fr/vocabulary/date-time/later.voc
 locale/fr-fr/vocabulary/date-time/next.voc
+locale/fr-fr/vocabulary/date-time/now.voc
+locale/fr-fr/vocabulary/date-time/number-days.voc
+locale/fr-fr/vocabulary/date-time/relative-day.voc
+locale/fr-fr/vocabulary/date-time/relative-time.voc
+locale/fr-fr/vocabulary/date-time/today.voc
+locale/fr-fr/vocabulary/date-time/week.voc
+locale/fr-fr/vocabulary/date-time/weekend.voc
+locale/fr-fr/vocabulary/query/confirm-query-current.voc
+locale/fr-fr/vocabulary/query/confirm-query-future.voc
+locale/fr-fr/vocabulary/query/confirm-query.voc
+locale/fr-fr/vocabulary/query/how.voc
 locale/fr-fr/vocabulary/query/query.voc
+locale/fr-fr/vocabulary/query/when.voc
+locale/fr-fr/vocabulary/temperature/cold.voc
+locale/fr-fr/vocabulary/temperature/high.voc
+locale/fr-fr/vocabulary/temperature/hot.voc
+locale/fr-fr/vocabulary/temperature/low.voc
+locale/fr-fr/vocabulary/temperature/temperature.voc
+locale/fr-fr/vocabulary/unit/fahrenheit.voc
+locale/fr-fr/vocabulary/unit/unit.entity
+locale/fr-fr/vocabulary/unit/unit.voc
 locale/gl-es/dialog/and.dialog
 locale/gl-es/dialog/percentage-number.dialog
 locale/gl-es/dialog/condition/ash.dialog
 locale/gl-es/dialog/condition/clear.dialog
 locale/gl-es/dialog/condition/clouds.dialog
 locale/gl-es/dialog/condition/drizzle.dialog
 locale/gl-es/dialog/condition/dust.dialog
@@ -726,15 +1273,15 @@
 locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
 locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
 locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
 locale/gl-es/dialog/hourly/hourly-weather-local.dialog
 locale/gl-es/dialog/hourly/hourly-weather-location.dialog
 locale/gl-es/dialog/unit/celsius.dialog
 locale/gl-es/dialog/unit/fahrenheit.dialog
-locale/gl-es/dialog/unit/meters per second.dialog
+locale/gl-es/dialog/unit/meter per second.dialog
 locale/gl-es/dialog/unit/miles per hour.dialog
 locale/gl-es/dialog/weekly/weekly-temperature.dialog
 locale/gl-es/regex/location.rx
 locale/gl-es/vocabulary/forecast.voc
 locale/gl-es/vocabulary/location.voc
 locale/gl-es/vocabulary/sunrise.voc
 locale/gl-es/vocabulary/sunset.voc
@@ -768,107 +1315,683 @@
 locale/gl-es/vocabulary/temperature/high.voc
 locale/gl-es/vocabulary/temperature/hot.voc
 locale/gl-es/vocabulary/temperature/low.voc
 locale/gl-es/vocabulary/temperature/temperature.voc
 locale/gl-es/vocabulary/unit/fahrenheit.voc
 locale/gl-es/vocabulary/unit/unit.entity
 locale/gl-es/vocabulary/unit/unit.voc
+locale/hu-hu/dialog/and.dialog
+locale/hu-hu/dialog/percentage-number.dialog
+locale/hu-hu/dialog/condition/ash.dialog
+locale/hu-hu/dialog/condition/clear-sky.dialog
+locale/hu-hu/dialog/condition/clear.dialog
+locale/hu-hu/dialog/condition/clouds.dialog
+locale/hu-hu/dialog/condition/depositing-rime-fog.dialog
+locale/hu-hu/dialog/condition/drizzle-dense-intensity.dialog
+locale/hu-hu/dialog/condition/drizzle-light-intensity.dialog
+locale/hu-hu/dialog/condition/drizzle-moderate-intensity.dialog
+locale/hu-hu/dialog/condition/drizzle.dialog
+locale/hu-hu/dialog/condition/dust.dialog
+locale/hu-hu/dialog/condition/fog.dialog
+locale/hu-hu/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/hu-hu/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/hu-hu/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/hu-hu/dialog/condition/freezing-rain-light-intensity.dialog
+locale/hu-hu/dialog/condition/haze.dialog
+locale/hu-hu/dialog/condition/heavy-rain.dialog
+locale/hu-hu/dialog/condition/heavy-snow-fall.dialog
+locale/hu-hu/dialog/condition/heavy-snow-showers.dialog
+locale/hu-hu/dialog/condition/humidity.dialog
+locale/hu-hu/dialog/condition/mainly-clear.dialog
+locale/hu-hu/dialog/condition/mist.dialog
+locale/hu-hu/dialog/condition/moderate-rain-showers.dialog
+locale/hu-hu/dialog/condition/moderate-rain.dialog
+locale/hu-hu/dialog/condition/moderate-snow-fall.dialog
+locale/hu-hu/dialog/condition/overcast.dialog
+locale/hu-hu/dialog/condition/partly-cloudy.dialog
+locale/hu-hu/dialog/condition/rain.dialog
+locale/hu-hu/dialog/condition/slight-rain-showers.dialog
+locale/hu-hu/dialog/condition/slight-rain.dialog
+locale/hu-hu/dialog/condition/slight-snow-fall.dialog
+locale/hu-hu/dialog/condition/slight-snow-showers.dialog
+locale/hu-hu/dialog/condition/smoke.dialog
+locale/hu-hu/dialog/condition/snow-grains.dialog
+locale/hu-hu/dialog/condition/snow.dialog
+locale/hu-hu/dialog/condition/squall.dialog
+locale/hu-hu/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/hu-hu/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/hu-hu/dialog/condition/thunderstorm.dialog
+locale/hu-hu/dialog/condition/tornado.dialog
+locale/hu-hu/dialog/condition/violent-rain-showers.dialog
+locale/hu-hu/dialog/current/current-condition-expected-local.dialog
+locale/hu-hu/dialog/current/current-condition-expected-location.dialog
+locale/hu-hu/dialog/current/current-condition-not-expected-local.dialog
+locale/hu-hu/dialog/current/current-condition-not-expected-location.dialog
+locale/hu-hu/dialog/current/current-humidity-local.dialog
+locale/hu-hu/dialog/current/current-humidity-location.dialog
+locale/hu-hu/dialog/current/current-sunrise-future-local.dialog
+locale/hu-hu/dialog/current/current-sunrise-future-location.dialog
+locale/hu-hu/dialog/current/current-sunrise-past-local.dialog
+locale/hu-hu/dialog/current/current-sunrise-past-location.dialog
+locale/hu-hu/dialog/current/current-sunset-future-local.dialog
+locale/hu-hu/dialog/current/current-sunset-future-location.dialog
+locale/hu-hu/dialog/current/current-sunset-past-local.dialog
+locale/hu-hu/dialog/current/current-sunset-past-location.dialog
+locale/hu-hu/dialog/current/current-temperature-local.dialog
+locale/hu-hu/dialog/current/current-temperature-location.dialog
+locale/hu-hu/dialog/current/current-weather-local.dialog
+locale/hu-hu/dialog/current/current-weather-location.dialog
+locale/hu-hu/dialog/current/current-wind-light-local.dialog
+locale/hu-hu/dialog/current/current-wind-light-location.dialog
+locale/hu-hu/dialog/current/current-wind-moderate-local.dialog
+locale/hu-hu/dialog/current/current-wind-moderate-location.dialog
+locale/hu-hu/dialog/current/current-wind-strong-local.dialog
+locale/hu-hu/dialog/current/current-wind-strong-location.dialog
+locale/hu-hu/dialog/current/currrent-clouds-alternative-local.dialog
+locale/hu-hu/dialog/daily/daily-condition-expected-local.dialog
+locale/hu-hu/dialog/daily/daily-condition-expected-location.dialog
+locale/hu-hu/dialog/daily/daily-condition-not-expected-local.dialog
+locale/hu-hu/dialog/daily/daily-condition-not-expected-location.dialog
+locale/hu-hu/dialog/daily/daily-humidity-local.dialog
+locale/hu-hu/dialog/daily/daily-humidity-location.dialog
+locale/hu-hu/dialog/daily/daily-precipitation-next-local.dialog
+locale/hu-hu/dialog/daily/daily-precipitation-next-location.dialog
+locale/hu-hu/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/hu-hu/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/hu-hu/dialog/daily/daily-sunrise-local.dialog
+locale/hu-hu/dialog/daily/daily-sunrise-location.dialog
+locale/hu-hu/dialog/daily/daily-sunset-local.dialog
+locale/hu-hu/dialog/daily/daily-sunset-location.dialog
+locale/hu-hu/dialog/daily/daily-temperature-high-local.dialog
+locale/hu-hu/dialog/daily/daily-temperature-high-location.dialog
+locale/hu-hu/dialog/daily/daily-temperature-local.dialog
+locale/hu-hu/dialog/daily/daily-temperature-location.dialog
+locale/hu-hu/dialog/daily/daily-temperature-low-local.dialog
+locale/hu-hu/dialog/daily/daily-temperature-low-location.dialog
+locale/hu-hu/dialog/daily/daily-weather-local.dialog
+locale/hu-hu/dialog/daily/daily-weather-location.dialog
+locale/hu-hu/dialog/daily/daily-wind-light-local.dialog
+locale/hu-hu/dialog/daily/daily-wind-light-location.dialog
+locale/hu-hu/dialog/daily/daily-wind-moderate-local.dialog
+locale/hu-hu/dialog/daily/daily-wind-moderate-location.dialog
+locale/hu-hu/dialog/daily/daily-wind-strong-local.dialog
+locale/hu-hu/dialog/daily/daily-wind-strong-location.dialog
+locale/hu-hu/dialog/direction/east.dialog
+locale/hu-hu/dialog/direction/north.dialog
+locale/hu-hu/dialog/direction/northeast.dialog
+locale/hu-hu/dialog/direction/northwest.dialog
+locale/hu-hu/dialog/direction/south.dialog
+locale/hu-hu/dialog/direction/southeast.dialog
+locale/hu-hu/dialog/direction/southwest.dialog
+locale/hu-hu/dialog/direction/west.dialog
+locale/hu-hu/dialog/error/cant-get-forecast.dialog
+locale/hu-hu/dialog/error/forty-eight-hours-available.dialog
+locale/hu-hu/dialog/error/location-not-found.dialog
+locale/hu-hu/dialog/error/no-forecast.dialog
+locale/hu-hu/dialog/error/seven-days-available.dialog
+locale/hu-hu/dialog/hourly/hourly-condition-expected-local.dialog
+locale/hu-hu/dialog/hourly/hourly-condition-expected-location.dialog
+locale/hu-hu/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/hu-hu/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/hu-hu/dialog/hourly/hourly-temperature-local.dialog
+locale/hu-hu/dialog/hourly/hourly-temperature-location.dialog
+locale/hu-hu/dialog/hourly/hourly-weather-local.dialog
+locale/hu-hu/dialog/hourly/hourly-weather-location.dialog
+locale/hu-hu/dialog/unit/celsius.dialog
+locale/hu-hu/dialog/unit/fahrenheit.dialog
+locale/hu-hu/dialog/unit/inch.dialog
+locale/hu-hu/dialog/unit/meter per second.dialog
+locale/hu-hu/dialog/unit/miles per hour.dialog
+locale/hu-hu/dialog/unit/millimeter.dialog
+locale/hu-hu/dialog/weekly/weekly-condition.dialog
+locale/hu-hu/dialog/weekly/weekly-temperature.dialog
+locale/hu-hu/regex/location.rx
+locale/hu-hu/vocabulary/forecast.voc
+locale/hu-hu/vocabulary/location.voc
+locale/hu-hu/vocabulary/outside.voc
+locale/hu-hu/vocabulary/sunrise.voc
+locale/hu-hu/vocabulary/sunset.voc
+locale/hu-hu/vocabulary/weather.voc
+locale/hu-hu/vocabulary/condition/clear.voc
+locale/hu-hu/vocabulary/condition/clouds.voc
+locale/hu-hu/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/hu-hu/vocabulary/condition/fog.voc
+locale/hu-hu/vocabulary/condition/humidity.voc
+locale/hu-hu/vocabulary/condition/precipitation.voc
+locale/hu-hu/vocabulary/condition/rain.voc
+locale/hu-hu/vocabulary/condition/snow.voc
+locale/hu-hu/vocabulary/condition/thunderstorm.voc
+locale/hu-hu/vocabulary/condition/windy.voc
+locale/hu-hu/vocabulary/date-time/couple.voc
+locale/hu-hu/vocabulary/date-time/few.voc
+locale/hu-hu/vocabulary/date-time/later.voc
+locale/hu-hu/vocabulary/date-time/next.voc
+locale/hu-hu/vocabulary/date-time/now.voc
+locale/hu-hu/vocabulary/date-time/number-days.voc
+locale/hu-hu/vocabulary/date-time/relative-day.voc
+locale/hu-hu/vocabulary/date-time/relative-time.voc
+locale/hu-hu/vocabulary/date-time/today.voc
+locale/hu-hu/vocabulary/date-time/week.voc
+locale/hu-hu/vocabulary/date-time/weekend.voc
+locale/hu-hu/vocabulary/query/confirm-query-current.voc
+locale/hu-hu/vocabulary/query/confirm-query-future.voc
+locale/hu-hu/vocabulary/query/confirm-query.voc
+locale/hu-hu/vocabulary/query/how.voc
+locale/hu-hu/vocabulary/query/query.voc
+locale/hu-hu/vocabulary/query/when.voc
+locale/hu-hu/vocabulary/temperature/cold.voc
+locale/hu-hu/vocabulary/temperature/high.voc
+locale/hu-hu/vocabulary/temperature/hot.voc
+locale/hu-hu/vocabulary/temperature/low.voc
+locale/hu-hu/vocabulary/temperature/temperature.voc
+locale/hu-hu/vocabulary/unit/fahrenheit.voc
+locale/hu-hu/vocabulary/unit/unit.entity
+locale/hu-hu/vocabulary/unit/unit.voc
+locale/it-it/dialog/and.dialog
 locale/it-it/dialog/percentage-number.dialog
 locale/it-it/dialog/condition/ash.dialog
+locale/it-it/dialog/condition/clear-sky.dialog
 locale/it-it/dialog/condition/clear.dialog
 locale/it-it/dialog/condition/clouds.dialog
+locale/it-it/dialog/condition/depositing-rime-fog.dialog
+locale/it-it/dialog/condition/drizzle-dense-intensity.dialog
+locale/it-it/dialog/condition/drizzle-light-intensity.dialog
+locale/it-it/dialog/condition/drizzle-moderate-intensity.dialog
 locale/it-it/dialog/condition/drizzle.dialog
 locale/it-it/dialog/condition/dust.dialog
+locale/it-it/dialog/condition/fog.dialog
+locale/it-it/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/it-it/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/it-it/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/it-it/dialog/condition/freezing-rain-light-intensity.dialog
 locale/it-it/dialog/condition/haze.dialog
+locale/it-it/dialog/condition/heavy-rain.dialog
+locale/it-it/dialog/condition/heavy-snow-fall.dialog
+locale/it-it/dialog/condition/heavy-snow-showers.dialog
+locale/it-it/dialog/condition/humidity.dialog
+locale/it-it/dialog/condition/mainly-clear.dialog
 locale/it-it/dialog/condition/mist.dialog
+locale/it-it/dialog/condition/moderate-rain-showers.dialog
+locale/it-it/dialog/condition/moderate-rain.dialog
+locale/it-it/dialog/condition/moderate-snow-fall.dialog
+locale/it-it/dialog/condition/overcast.dialog
+locale/it-it/dialog/condition/partly-cloudy.dialog
 locale/it-it/dialog/condition/rain.dialog
+locale/it-it/dialog/condition/slight-rain-showers.dialog
+locale/it-it/dialog/condition/slight-rain.dialog
+locale/it-it/dialog/condition/slight-snow-fall.dialog
+locale/it-it/dialog/condition/slight-snow-showers.dialog
 locale/it-it/dialog/condition/smoke.dialog
+locale/it-it/dialog/condition/snow-grains.dialog
 locale/it-it/dialog/condition/snow.dialog
 locale/it-it/dialog/condition/squall.dialog
+locale/it-it/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/it-it/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/it-it/dialog/condition/thunderstorm.dialog
 locale/it-it/dialog/condition/tornado.dialog
+locale/it-it/dialog/condition/violent-rain-showers.dialog
 locale/it-it/dialog/current/current-condition-expected-local.dialog
 locale/it-it/dialog/current/current-condition-expected-location.dialog
+locale/it-it/dialog/current/current-condition-not-expected-local.dialog
+locale/it-it/dialog/current/current-condition-not-expected-location.dialog
+locale/it-it/dialog/current/current-humidity-local.dialog
+locale/it-it/dialog/current/current-humidity-location.dialog
+locale/it-it/dialog/current/current-sunrise-future-local.dialog
+locale/it-it/dialog/current/current-sunrise-future-location.dialog
+locale/it-it/dialog/current/current-sunrise-past-local.dialog
+locale/it-it/dialog/current/current-sunrise-past-location.dialog
+locale/it-it/dialog/current/current-sunset-future-local.dialog
+locale/it-it/dialog/current/current-sunset-future-location.dialog
+locale/it-it/dialog/current/current-sunset-past-local.dialog
+locale/it-it/dialog/current/current-sunset-past-location.dialog
+locale/it-it/dialog/current/current-temperature-local.dialog
+locale/it-it/dialog/current/current-temperature-location.dialog
+locale/it-it/dialog/current/current-weather-local.dialog
+locale/it-it/dialog/current/current-weather-location.dialog
+locale/it-it/dialog/current/current-wind-light-local.dialog
+locale/it-it/dialog/current/current-wind-light-location.dialog
+locale/it-it/dialog/current/current-wind-moderate-local.dialog
+locale/it-it/dialog/current/current-wind-moderate-location.dialog
+locale/it-it/dialog/current/current-wind-strong-local.dialog
+locale/it-it/dialog/current/current-wind-strong-location.dialog
+locale/it-it/dialog/current/currrent-clouds-alternative-local.dialog
+locale/it-it/dialog/daily/daily-condition-expected-local.dialog
+locale/it-it/dialog/daily/daily-condition-expected-location.dialog
+locale/it-it/dialog/daily/daily-condition-not-expected-local.dialog
+locale/it-it/dialog/daily/daily-condition-not-expected-location.dialog
+locale/it-it/dialog/daily/daily-humidity-local.dialog
+locale/it-it/dialog/daily/daily-humidity-location.dialog
+locale/it-it/dialog/daily/daily-precipitation-next-local.dialog
+locale/it-it/dialog/daily/daily-precipitation-next-location.dialog
+locale/it-it/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/it-it/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/it-it/dialog/daily/daily-sunrise-local.dialog
+locale/it-it/dialog/daily/daily-sunrise-location.dialog
+locale/it-it/dialog/daily/daily-sunset-local.dialog
+locale/it-it/dialog/daily/daily-sunset-location.dialog
+locale/it-it/dialog/daily/daily-temperature-high-local.dialog
+locale/it-it/dialog/daily/daily-temperature-high-location.dialog
+locale/it-it/dialog/daily/daily-temperature-local.dialog
+locale/it-it/dialog/daily/daily-temperature-location.dialog
+locale/it-it/dialog/daily/daily-temperature-low-local.dialog
+locale/it-it/dialog/daily/daily-temperature-low-location.dialog
+locale/it-it/dialog/daily/daily-weather-local.dialog
+locale/it-it/dialog/daily/daily-weather-location.dialog
+locale/it-it/dialog/daily/daily-wind-light-local.dialog
+locale/it-it/dialog/daily/daily-wind-light-location.dialog
+locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
+locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
+locale/it-it/dialog/daily/daily-wind-strong-local.dialog
+locale/it-it/dialog/daily/daily-wind-strong-location.dialog
 locale/it-it/dialog/direction/east.dialog
 locale/it-it/dialog/direction/north.dialog
 locale/it-it/dialog/direction/northeast.dialog
 locale/it-it/dialog/direction/northwest.dialog
 locale/it-it/dialog/direction/south.dialog
 locale/it-it/dialog/direction/southeast.dialog
 locale/it-it/dialog/direction/southwest.dialog
 locale/it-it/dialog/direction/west.dialog
+locale/it-it/dialog/error/cant-get-forecast.dialog
+locale/it-it/dialog/error/forty-eight-hours-available.dialog
+locale/it-it/dialog/error/location-not-found.dialog
+locale/it-it/dialog/error/no-forecast.dialog
+locale/it-it/dialog/error/seven-days-available.dialog
+locale/it-it/dialog/hourly/hourly-condition-expected-local.dialog
+locale/it-it/dialog/hourly/hourly-condition-expected-location.dialog
+locale/it-it/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/it-it/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/it-it/dialog/hourly/hourly-temperature-local.dialog
+locale/it-it/dialog/hourly/hourly-temperature-location.dialog
+locale/it-it/dialog/hourly/hourly-weather-local.dialog
+locale/it-it/dialog/hourly/hourly-weather-location.dialog
 locale/it-it/dialog/unit/celsius.dialog
 locale/it-it/dialog/unit/fahrenheit.dialog
-locale/it-it/dialog/unit/meters per second.dialog
+locale/it-it/dialog/unit/inch.dialog
+locale/it-it/dialog/unit/meter per second.dialog
 locale/it-it/dialog/unit/miles per hour.dialog
+locale/it-it/dialog/unit/millimeter.dialog
+locale/it-it/dialog/weekly/weekly-condition.dialog
+locale/it-it/dialog/weekly/weekly-temperature.dialog
 locale/it-it/regex/location.rx
 locale/it-it/vocabulary/forecast.voc
 locale/it-it/vocabulary/location.voc
+locale/it-it/vocabulary/outside.voc
 locale/it-it/vocabulary/sunrise.voc
 locale/it-it/vocabulary/sunset.voc
 locale/it-it/vocabulary/weather.voc
 locale/it-it/vocabulary/condition/clear.voc
 locale/it-it/vocabulary/condition/clouds.voc
+locale/it-it/vocabulary/condition/do-i-need-an-umbrella.intent
 locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
 locale/it-it/vocabulary/condition/fog.voc
 locale/it-it/vocabulary/condition/humidity.voc
 locale/it-it/vocabulary/condition/precipitation.voc
 locale/it-it/vocabulary/condition/rain.voc
 locale/it-it/vocabulary/condition/snow.voc
+locale/it-it/vocabulary/condition/thunderstorm.voc
 locale/it-it/vocabulary/condition/windy.voc
+locale/it-it/vocabulary/date-time/couple.voc
+locale/it-it/vocabulary/date-time/few.voc
 locale/it-it/vocabulary/date-time/later.voc
 locale/it-it/vocabulary/date-time/next.voc
+locale/it-it/vocabulary/date-time/now.voc
+locale/it-it/vocabulary/date-time/number-days.voc
+locale/it-it/vocabulary/date-time/relative-day.voc
+locale/it-it/vocabulary/date-time/relative-time.voc
+locale/it-it/vocabulary/date-time/today.voc
+locale/it-it/vocabulary/date-time/week.voc
 locale/it-it/vocabulary/date-time/weekend.voc
+locale/it-it/vocabulary/query/confirm-query-current.voc
+locale/it-it/vocabulary/query/confirm-query-future.voc
 locale/it-it/vocabulary/query/confirm-query.voc
+locale/it-it/vocabulary/query/how.voc
 locale/it-it/vocabulary/query/query.voc
+locale/it-it/vocabulary/query/when.voc
 locale/it-it/vocabulary/temperature/cold.voc
 locale/it-it/vocabulary/temperature/high.voc
 locale/it-it/vocabulary/temperature/hot.voc
 locale/it-it/vocabulary/temperature/low.voc
 locale/it-it/vocabulary/temperature/temperature.voc
 locale/it-it/vocabulary/unit/fahrenheit.voc
 locale/it-it/vocabulary/unit/unit.entity
 locale/it-it/vocabulary/unit/unit.voc
+locale/nl-nl/dialog/and.dialog
 locale/nl-nl/dialog/percentage-number.dialog
 locale/nl-nl/dialog/condition/ash.dialog
+locale/nl-nl/dialog/condition/clear-sky.dialog
 locale/nl-nl/dialog/condition/clear.dialog
 locale/nl-nl/dialog/condition/clouds.dialog
+locale/nl-nl/dialog/condition/depositing-rime-fog.dialog
+locale/nl-nl/dialog/condition/drizzle-dense-intensity.dialog
+locale/nl-nl/dialog/condition/drizzle-light-intensity.dialog
+locale/nl-nl/dialog/condition/drizzle-moderate-intensity.dialog
 locale/nl-nl/dialog/condition/drizzle.dialog
 locale/nl-nl/dialog/condition/dust.dialog
+locale/nl-nl/dialog/condition/fog.dialog
+locale/nl-nl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/nl-nl/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/nl-nl/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/nl-nl/dialog/condition/freezing-rain-light-intensity.dialog
 locale/nl-nl/dialog/condition/haze.dialog
+locale/nl-nl/dialog/condition/heavy-rain.dialog
+locale/nl-nl/dialog/condition/heavy-snow-fall.dialog
+locale/nl-nl/dialog/condition/heavy-snow-showers.dialog
+locale/nl-nl/dialog/condition/humidity.dialog
+locale/nl-nl/dialog/condition/mainly-clear.dialog
 locale/nl-nl/dialog/condition/mist.dialog
+locale/nl-nl/dialog/condition/moderate-rain-showers.dialog
+locale/nl-nl/dialog/condition/moderate-rain.dialog
+locale/nl-nl/dialog/condition/moderate-snow-fall.dialog
+locale/nl-nl/dialog/condition/overcast.dialog
+locale/nl-nl/dialog/condition/partly-cloudy.dialog
 locale/nl-nl/dialog/condition/rain.dialog
+locale/nl-nl/dialog/condition/slight-rain-showers.dialog
+locale/nl-nl/dialog/condition/slight-rain.dialog
+locale/nl-nl/dialog/condition/slight-snow-fall.dialog
+locale/nl-nl/dialog/condition/slight-snow-showers.dialog
 locale/nl-nl/dialog/condition/smoke.dialog
+locale/nl-nl/dialog/condition/snow-grains.dialog
 locale/nl-nl/dialog/condition/snow.dialog
 locale/nl-nl/dialog/condition/squall.dialog
+locale/nl-nl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/nl-nl/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/nl-nl/dialog/condition/thunderstorm.dialog
 locale/nl-nl/dialog/condition/tornado.dialog
+locale/nl-nl/dialog/condition/violent-rain-showers.dialog
+locale/nl-nl/dialog/current/current-condition-expected-local.dialog
+locale/nl-nl/dialog/current/current-condition-expected-location.dialog
+locale/nl-nl/dialog/current/current-condition-not-expected-local.dialog
+locale/nl-nl/dialog/current/current-condition-not-expected-location.dialog
+locale/nl-nl/dialog/current/current-humidity-local.dialog
+locale/nl-nl/dialog/current/current-humidity-location.dialog
+locale/nl-nl/dialog/current/current-sunrise-future-local.dialog
+locale/nl-nl/dialog/current/current-sunrise-future-location.dialog
+locale/nl-nl/dialog/current/current-sunrise-past-local.dialog
+locale/nl-nl/dialog/current/current-sunrise-past-location.dialog
+locale/nl-nl/dialog/current/current-sunset-future-local.dialog
+locale/nl-nl/dialog/current/current-sunset-future-location.dialog
+locale/nl-nl/dialog/current/current-sunset-past-local.dialog
+locale/nl-nl/dialog/current/current-sunset-past-location.dialog
+locale/nl-nl/dialog/current/current-temperature-local.dialog
+locale/nl-nl/dialog/current/current-temperature-location.dialog
+locale/nl-nl/dialog/current/current-weather-local.dialog
+locale/nl-nl/dialog/current/current-weather-location.dialog
+locale/nl-nl/dialog/current/current-wind-light-local.dialog
+locale/nl-nl/dialog/current/current-wind-light-location.dialog
+locale/nl-nl/dialog/current/current-wind-moderate-local.dialog
+locale/nl-nl/dialog/current/current-wind-moderate-location.dialog
+locale/nl-nl/dialog/current/current-wind-strong-local.dialog
+locale/nl-nl/dialog/current/current-wind-strong-location.dialog
+locale/nl-nl/dialog/current/currrent-clouds-alternative-local.dialog
+locale/nl-nl/dialog/daily/daily-condition-expected-local.dialog
+locale/nl-nl/dialog/daily/daily-condition-expected-location.dialog
+locale/nl-nl/dialog/daily/daily-condition-not-expected-local.dialog
+locale/nl-nl/dialog/daily/daily-condition-not-expected-location.dialog
+locale/nl-nl/dialog/daily/daily-humidity-local.dialog
+locale/nl-nl/dialog/daily/daily-humidity-location.dialog
+locale/nl-nl/dialog/daily/daily-precipitation-next-local.dialog
+locale/nl-nl/dialog/daily/daily-precipitation-next-location.dialog
+locale/nl-nl/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/nl-nl/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/nl-nl/dialog/daily/daily-sunrise-local.dialog
+locale/nl-nl/dialog/daily/daily-sunrise-location.dialog
+locale/nl-nl/dialog/daily/daily-sunset-local.dialog
+locale/nl-nl/dialog/daily/daily-sunset-location.dialog
+locale/nl-nl/dialog/daily/daily-temperature-high-local.dialog
+locale/nl-nl/dialog/daily/daily-temperature-high-location.dialog
+locale/nl-nl/dialog/daily/daily-temperature-local.dialog
+locale/nl-nl/dialog/daily/daily-temperature-location.dialog
+locale/nl-nl/dialog/daily/daily-temperature-low-local.dialog
+locale/nl-nl/dialog/daily/daily-temperature-low-location.dialog
+locale/nl-nl/dialog/daily/daily-weather-local.dialog
+locale/nl-nl/dialog/daily/daily-weather-location.dialog
+locale/nl-nl/dialog/daily/daily-wind-light-local.dialog
+locale/nl-nl/dialog/daily/daily-wind-light-location.dialog
+locale/nl-nl/dialog/daily/daily-wind-moderate-local.dialog
+locale/nl-nl/dialog/daily/daily-wind-moderate-location.dialog
+locale/nl-nl/dialog/daily/daily-wind-strong-local.dialog
+locale/nl-nl/dialog/daily/daily-wind-strong-location.dialog
 locale/nl-nl/dialog/direction/east.dialog
 locale/nl-nl/dialog/direction/north.dialog
 locale/nl-nl/dialog/direction/northeast.dialog
 locale/nl-nl/dialog/direction/northwest.dialog
 locale/nl-nl/dialog/direction/south.dialog
 locale/nl-nl/dialog/direction/southeast.dialog
 locale/nl-nl/dialog/direction/southwest.dialog
+locale/nl-nl/dialog/direction/west.dialog
+locale/nl-nl/dialog/error/cant-get-forecast.dialog
+locale/nl-nl/dialog/error/forty-eight-hours-available.dialog
+locale/nl-nl/dialog/error/location-not-found.dialog
+locale/nl-nl/dialog/error/no-forecast.dialog
+locale/nl-nl/dialog/error/seven-days-available.dialog
+locale/nl-nl/dialog/hourly/hourly-condition-expected-local.dialog
+locale/nl-nl/dialog/hourly/hourly-condition-expected-location.dialog
+locale/nl-nl/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/nl-nl/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/nl-nl/dialog/hourly/hourly-temperature-local.dialog
+locale/nl-nl/dialog/hourly/hourly-temperature-location.dialog
+locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
+locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
 locale/nl-nl/dialog/unit/celsius.dialog
 locale/nl-nl/dialog/unit/fahrenheit.dialog
-locale/nl-nl/dialog/unit/meters per second.dialog
+locale/nl-nl/dialog/unit/inch.dialog
+locale/nl-nl/dialog/unit/meter per second.dialog
 locale/nl-nl/dialog/unit/miles per hour.dialog
+locale/nl-nl/dialog/unit/millimeter.dialog
+locale/nl-nl/dialog/weekly/weekly-condition.dialog
+locale/nl-nl/dialog/weekly/weekly-temperature.dialog
 locale/nl-nl/regex/location.rx
 locale/nl-nl/vocabulary/forecast.voc
 locale/nl-nl/vocabulary/location.voc
+locale/nl-nl/vocabulary/outside.voc
 locale/nl-nl/vocabulary/sunrise.voc
 locale/nl-nl/vocabulary/sunset.voc
 locale/nl-nl/vocabulary/weather.voc
+locale/nl-nl/vocabulary/condition/clear.voc
+locale/nl-nl/vocabulary/condition/clouds.voc
+locale/nl-nl/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/nl-nl/vocabulary/condition/fog.voc
 locale/nl-nl/vocabulary/condition/humidity.voc
 locale/nl-nl/vocabulary/condition/precipitation.voc
+locale/nl-nl/vocabulary/condition/rain.voc
+locale/nl-nl/vocabulary/condition/snow.voc
+locale/nl-nl/vocabulary/condition/thunderstorm.voc
 locale/nl-nl/vocabulary/condition/windy.voc
+locale/nl-nl/vocabulary/date-time/couple.voc
+locale/nl-nl/vocabulary/date-time/few.voc
 locale/nl-nl/vocabulary/date-time/later.voc
 locale/nl-nl/vocabulary/date-time/next.voc
+locale/nl-nl/vocabulary/date-time/now.voc
+locale/nl-nl/vocabulary/date-time/number-days.voc
+locale/nl-nl/vocabulary/date-time/relative-day.voc
+locale/nl-nl/vocabulary/date-time/relative-time.voc
+locale/nl-nl/vocabulary/date-time/today.voc
+locale/nl-nl/vocabulary/date-time/week.voc
+locale/nl-nl/vocabulary/date-time/weekend.voc
+locale/nl-nl/vocabulary/query/confirm-query-current.voc
+locale/nl-nl/vocabulary/query/confirm-query-future.voc
+locale/nl-nl/vocabulary/query/confirm-query.voc
+locale/nl-nl/vocabulary/query/how.voc
 locale/nl-nl/vocabulary/query/query.voc
+locale/nl-nl/vocabulary/query/when.voc
+locale/nl-nl/vocabulary/temperature/cold.voc
+locale/nl-nl/vocabulary/temperature/high.voc
+locale/nl-nl/vocabulary/temperature/hot.voc
+locale/nl-nl/vocabulary/temperature/low.voc
+locale/nl-nl/vocabulary/temperature/temperature.voc
+locale/nl-nl/vocabulary/unit/fahrenheit.voc
+locale/nl-nl/vocabulary/unit/unit.entity
+locale/nl-nl/vocabulary/unit/unit.voc
+locale/pl-pl/dialog/and.dialog
+locale/pl-pl/dialog/percentage-number.dialog
+locale/pl-pl/dialog/condition/ash.dialog
+locale/pl-pl/dialog/condition/clear-sky.dialog
+locale/pl-pl/dialog/condition/clear.dialog
+locale/pl-pl/dialog/condition/clouds.dialog
+locale/pl-pl/dialog/condition/depositing-rime-fog.dialog
+locale/pl-pl/dialog/condition/drizzle-dense-intensity.dialog
+locale/pl-pl/dialog/condition/drizzle-light-intensity.dialog
+locale/pl-pl/dialog/condition/drizzle-moderate-intensity.dialog
+locale/pl-pl/dialog/condition/drizzle.dialog
+locale/pl-pl/dialog/condition/dust.dialog
+locale/pl-pl/dialog/condition/fog.dialog
+locale/pl-pl/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/pl-pl/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/pl-pl/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/pl-pl/dialog/condition/freezing-rain-light-intensity.dialog
+locale/pl-pl/dialog/condition/haze.dialog
+locale/pl-pl/dialog/condition/heavy-rain.dialog
+locale/pl-pl/dialog/condition/heavy-snow-fall.dialog
+locale/pl-pl/dialog/condition/heavy-snow-showers.dialog
+locale/pl-pl/dialog/condition/humidity.dialog
+locale/pl-pl/dialog/condition/mainly-clear.dialog
+locale/pl-pl/dialog/condition/mist.dialog
+locale/pl-pl/dialog/condition/moderate-rain-showers.dialog
+locale/pl-pl/dialog/condition/moderate-rain.dialog
+locale/pl-pl/dialog/condition/moderate-snow-fall.dialog
+locale/pl-pl/dialog/condition/overcast.dialog
+locale/pl-pl/dialog/condition/partly-cloudy.dialog
+locale/pl-pl/dialog/condition/rain.dialog
+locale/pl-pl/dialog/condition/slight-rain-showers.dialog
+locale/pl-pl/dialog/condition/slight-rain.dialog
+locale/pl-pl/dialog/condition/slight-snow-fall.dialog
+locale/pl-pl/dialog/condition/slight-snow-showers.dialog
+locale/pl-pl/dialog/condition/smoke.dialog
+locale/pl-pl/dialog/condition/snow-grains.dialog
+locale/pl-pl/dialog/condition/snow.dialog
+locale/pl-pl/dialog/condition/squall.dialog
+locale/pl-pl/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/pl-pl/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/pl-pl/dialog/condition/thunderstorm.dialog
+locale/pl-pl/dialog/condition/tornado.dialog
+locale/pl-pl/dialog/condition/violent-rain-showers.dialog
+locale/pl-pl/dialog/current/current-condition-expected-local.dialog
+locale/pl-pl/dialog/current/current-condition-expected-location.dialog
+locale/pl-pl/dialog/current/current-condition-not-expected-local.dialog
+locale/pl-pl/dialog/current/current-condition-not-expected-location.dialog
+locale/pl-pl/dialog/current/current-humidity-local.dialog
+locale/pl-pl/dialog/current/current-humidity-location.dialog
+locale/pl-pl/dialog/current/current-sunrise-future-local.dialog
+locale/pl-pl/dialog/current/current-sunrise-future-location.dialog
+locale/pl-pl/dialog/current/current-sunrise-past-local.dialog
+locale/pl-pl/dialog/current/current-sunrise-past-location.dialog
+locale/pl-pl/dialog/current/current-sunset-future-local.dialog
+locale/pl-pl/dialog/current/current-sunset-future-location.dialog
+locale/pl-pl/dialog/current/current-sunset-past-local.dialog
+locale/pl-pl/dialog/current/current-sunset-past-location.dialog
+locale/pl-pl/dialog/current/current-temperature-local.dialog
+locale/pl-pl/dialog/current/current-temperature-location.dialog
+locale/pl-pl/dialog/current/current-weather-local.dialog
+locale/pl-pl/dialog/current/current-weather-location.dialog
+locale/pl-pl/dialog/current/current-wind-light-local.dialog
+locale/pl-pl/dialog/current/current-wind-light-location.dialog
+locale/pl-pl/dialog/current/current-wind-moderate-local.dialog
+locale/pl-pl/dialog/current/current-wind-moderate-location.dialog
+locale/pl-pl/dialog/current/current-wind-strong-local.dialog
+locale/pl-pl/dialog/current/current-wind-strong-location.dialog
+locale/pl-pl/dialog/current/currrent-clouds-alternative-local.dialog
+locale/pl-pl/dialog/daily/daily-condition-expected-local.dialog
+locale/pl-pl/dialog/daily/daily-condition-expected-location.dialog
+locale/pl-pl/dialog/daily/daily-condition-not-expected-local.dialog
+locale/pl-pl/dialog/daily/daily-condition-not-expected-location.dialog
+locale/pl-pl/dialog/daily/daily-humidity-local.dialog
+locale/pl-pl/dialog/daily/daily-humidity-location.dialog
+locale/pl-pl/dialog/daily/daily-precipitation-next-local.dialog
+locale/pl-pl/dialog/daily/daily-precipitation-next-location.dialog
+locale/pl-pl/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/pl-pl/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/pl-pl/dialog/daily/daily-sunrise-local.dialog
+locale/pl-pl/dialog/daily/daily-sunrise-location.dialog
+locale/pl-pl/dialog/daily/daily-sunset-local.dialog
+locale/pl-pl/dialog/daily/daily-sunset-location.dialog
+locale/pl-pl/dialog/daily/daily-temperature-high-local.dialog
+locale/pl-pl/dialog/daily/daily-temperature-high-location.dialog
+locale/pl-pl/dialog/daily/daily-temperature-local.dialog
+locale/pl-pl/dialog/daily/daily-temperature-location.dialog
+locale/pl-pl/dialog/daily/daily-temperature-low-local.dialog
+locale/pl-pl/dialog/daily/daily-temperature-low-location.dialog
+locale/pl-pl/dialog/daily/daily-weather-local.dialog
+locale/pl-pl/dialog/daily/daily-weather-location.dialog
+locale/pl-pl/dialog/daily/daily-wind-light-local.dialog
+locale/pl-pl/dialog/daily/daily-wind-light-location.dialog
+locale/pl-pl/dialog/daily/daily-wind-moderate-local.dialog
+locale/pl-pl/dialog/daily/daily-wind-moderate-location.dialog
+locale/pl-pl/dialog/daily/daily-wind-strong-local.dialog
+locale/pl-pl/dialog/daily/daily-wind-strong-location.dialog
+locale/pl-pl/dialog/direction/east.dialog
+locale/pl-pl/dialog/direction/north.dialog
+locale/pl-pl/dialog/direction/northeast.dialog
+locale/pl-pl/dialog/direction/northwest.dialog
+locale/pl-pl/dialog/direction/south.dialog
+locale/pl-pl/dialog/direction/southeast.dialog
+locale/pl-pl/dialog/direction/southwest.dialog
+locale/pl-pl/dialog/direction/west.dialog
+locale/pl-pl/dialog/error/cant-get-forecast.dialog
+locale/pl-pl/dialog/error/forty-eight-hours-available.dialog
+locale/pl-pl/dialog/error/location-not-found.dialog
+locale/pl-pl/dialog/error/no-forecast.dialog
+locale/pl-pl/dialog/error/seven-days-available.dialog
+locale/pl-pl/dialog/hourly/hourly-condition-expected-local.dialog
+locale/pl-pl/dialog/hourly/hourly-condition-expected-location.dialog
+locale/pl-pl/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/pl-pl/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/pl-pl/dialog/hourly/hourly-temperature-local.dialog
+locale/pl-pl/dialog/hourly/hourly-temperature-location.dialog
+locale/pl-pl/dialog/hourly/hourly-weather-local.dialog
+locale/pl-pl/dialog/hourly/hourly-weather-location.dialog
+locale/pl-pl/dialog/unit/celsius.dialog
+locale/pl-pl/dialog/unit/fahrenheit.dialog
+locale/pl-pl/dialog/unit/inch.dialog
+locale/pl-pl/dialog/unit/meter per second.dialog
+locale/pl-pl/dialog/unit/miles per hour.dialog
+locale/pl-pl/dialog/unit/millimeter.dialog
+locale/pl-pl/dialog/weekly/weekly-condition.dialog
+locale/pl-pl/dialog/weekly/weekly-temperature.dialog
+locale/pl-pl/regex/location.rx
+locale/pl-pl/vocabulary/forecast.voc
+locale/pl-pl/vocabulary/location.voc
+locale/pl-pl/vocabulary/outside.voc
+locale/pl-pl/vocabulary/sunrise.voc
+locale/pl-pl/vocabulary/sunset.voc
+locale/pl-pl/vocabulary/weather.voc
+locale/pl-pl/vocabulary/condition/clear.voc
+locale/pl-pl/vocabulary/condition/clouds.voc
+locale/pl-pl/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/pl-pl/vocabulary/condition/fog.voc
+locale/pl-pl/vocabulary/condition/humidity.voc
+locale/pl-pl/vocabulary/condition/precipitation.voc
+locale/pl-pl/vocabulary/condition/rain.voc
+locale/pl-pl/vocabulary/condition/snow.voc
+locale/pl-pl/vocabulary/condition/thunderstorm.voc
+locale/pl-pl/vocabulary/condition/windy.voc
+locale/pl-pl/vocabulary/date-time/couple.voc
+locale/pl-pl/vocabulary/date-time/few.voc
+locale/pl-pl/vocabulary/date-time/later.voc
+locale/pl-pl/vocabulary/date-time/next.voc
+locale/pl-pl/vocabulary/date-time/now.voc
+locale/pl-pl/vocabulary/date-time/number-days.voc
+locale/pl-pl/vocabulary/date-time/relative-day.voc
+locale/pl-pl/vocabulary/date-time/relative-time.voc
+locale/pl-pl/vocabulary/date-time/today.voc
+locale/pl-pl/vocabulary/date-time/week.voc
+locale/pl-pl/vocabulary/date-time/weekend.voc
+locale/pl-pl/vocabulary/query/confirm-query-current.voc
+locale/pl-pl/vocabulary/query/confirm-query-future.voc
+locale/pl-pl/vocabulary/query/confirm-query.voc
+locale/pl-pl/vocabulary/query/how.voc
+locale/pl-pl/vocabulary/query/query.voc
+locale/pl-pl/vocabulary/query/when.voc
+locale/pl-pl/vocabulary/temperature/cold.voc
+locale/pl-pl/vocabulary/temperature/high.voc
+locale/pl-pl/vocabulary/temperature/hot.voc
+locale/pl-pl/vocabulary/temperature/low.voc
+locale/pl-pl/vocabulary/temperature/temperature.voc
+locale/pl-pl/vocabulary/unit/fahrenheit.voc
+locale/pl-pl/vocabulary/unit/unit.entity
+locale/pl-pl/vocabulary/unit/unit.voc
 locale/pt-br/dialog/and.dialog
 locale/pt-br/dialog/percentage-number.dialog
 locale/pt-br/dialog/condition/ash.dialog
 locale/pt-br/dialog/condition/clear.dialog
 locale/pt-br/dialog/condition/clouds.dialog
 locale/pt-br/dialog/condition/drizzle.dialog
 locale/pt-br/dialog/condition/dust.dialog
@@ -931,15 +2054,15 @@
 locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
 locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
 locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
 locale/pt-br/dialog/hourly/hourly-weather-local.dialog
 locale/pt-br/dialog/hourly/hourly-weather-location.dialog
 locale/pt-br/dialog/unit/celsius.dialog
 locale/pt-br/dialog/unit/fahrenheit.dialog
-locale/pt-br/dialog/unit/meters per second.dialog
+locale/pt-br/dialog/unit/meter per second.dialog
 locale/pt-br/dialog/unit/miles per hour.dialog
 locale/pt-br/dialog/weekly/weekly-temperature.dialog
 locale/pt-br/regex/location.rx
 locale/pt-br/vocabulary/forecast.voc
 locale/pt-br/vocabulary/location.voc
 locale/pt-br/vocabulary/sunrise.voc
 locale/pt-br/vocabulary/sunset.voc
@@ -973,111 +2096,668 @@
 locale/pt-br/vocabulary/temperature/high.voc
 locale/pt-br/vocabulary/temperature/hot.voc
 locale/pt-br/vocabulary/temperature/low.voc
 locale/pt-br/vocabulary/temperature/temperature.voc
 locale/pt-br/vocabulary/unit/fahrenheit.voc
 locale/pt-br/vocabulary/unit/unit.entity
 locale/pt-br/vocabulary/unit/unit.voc
+locale/pt-pt/dialog/and.dialog
+locale/pt-pt/dialog/percentage-number.dialog
+locale/pt-pt/dialog/condition/ash.dialog
+locale/pt-pt/dialog/condition/clear-sky.dialog
+locale/pt-pt/dialog/condition/clear.dialog
+locale/pt-pt/dialog/condition/clouds.dialog
+locale/pt-pt/dialog/condition/depositing-rime-fog.dialog
+locale/pt-pt/dialog/condition/drizzle-dense-intensity.dialog
+locale/pt-pt/dialog/condition/drizzle-light-intensity.dialog
+locale/pt-pt/dialog/condition/drizzle-moderate-intensity.dialog
+locale/pt-pt/dialog/condition/drizzle.dialog
+locale/pt-pt/dialog/condition/dust.dialog
+locale/pt-pt/dialog/condition/fog.dialog
+locale/pt-pt/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/pt-pt/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/pt-pt/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/pt-pt/dialog/condition/freezing-rain-light-intensity.dialog
+locale/pt-pt/dialog/condition/haze.dialog
+locale/pt-pt/dialog/condition/heavy-rain.dialog
+locale/pt-pt/dialog/condition/heavy-snow-fall.dialog
+locale/pt-pt/dialog/condition/heavy-snow-showers.dialog
+locale/pt-pt/dialog/condition/humidity.dialog
+locale/pt-pt/dialog/condition/mainly-clear.dialog
+locale/pt-pt/dialog/condition/mist.dialog
+locale/pt-pt/dialog/condition/moderate-rain-showers.dialog
+locale/pt-pt/dialog/condition/moderate-rain.dialog
+locale/pt-pt/dialog/condition/moderate-snow-fall.dialog
+locale/pt-pt/dialog/condition/overcast.dialog
+locale/pt-pt/dialog/condition/partly-cloudy.dialog
+locale/pt-pt/dialog/condition/rain.dialog
+locale/pt-pt/dialog/condition/slight-rain-showers.dialog
+locale/pt-pt/dialog/condition/slight-rain.dialog
+locale/pt-pt/dialog/condition/slight-snow-fall.dialog
+locale/pt-pt/dialog/condition/slight-snow-showers.dialog
+locale/pt-pt/dialog/condition/smoke.dialog
+locale/pt-pt/dialog/condition/snow-grains.dialog
+locale/pt-pt/dialog/condition/snow.dialog
+locale/pt-pt/dialog/condition/squall.dialog
+locale/pt-pt/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/pt-pt/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/pt-pt/dialog/condition/thunderstorm.dialog
+locale/pt-pt/dialog/condition/tornado.dialog
+locale/pt-pt/dialog/condition/violent-rain-showers.dialog
+locale/pt-pt/dialog/current/current-condition-expected-local.dialog
+locale/pt-pt/dialog/current/current-condition-expected-location.dialog
+locale/pt-pt/dialog/current/current-condition-not-expected-local.dialog
+locale/pt-pt/dialog/current/current-condition-not-expected-location.dialog
+locale/pt-pt/dialog/current/current-humidity-local.dialog
+locale/pt-pt/dialog/current/current-humidity-location.dialog
+locale/pt-pt/dialog/current/current-sunrise-future-local.dialog
+locale/pt-pt/dialog/current/current-sunrise-future-location.dialog
+locale/pt-pt/dialog/current/current-sunrise-past-local.dialog
+locale/pt-pt/dialog/current/current-sunrise-past-location.dialog
+locale/pt-pt/dialog/current/current-sunset-future-local.dialog
+locale/pt-pt/dialog/current/current-sunset-future-location.dialog
+locale/pt-pt/dialog/current/current-sunset-past-local.dialog
+locale/pt-pt/dialog/current/current-sunset-past-location.dialog
+locale/pt-pt/dialog/current/current-temperature-local.dialog
+locale/pt-pt/dialog/current/current-temperature-location.dialog
+locale/pt-pt/dialog/current/current-weather-local.dialog
+locale/pt-pt/dialog/current/current-weather-location.dialog
+locale/pt-pt/dialog/current/current-wind-light-local.dialog
+locale/pt-pt/dialog/current/current-wind-light-location.dialog
+locale/pt-pt/dialog/current/current-wind-moderate-local.dialog
+locale/pt-pt/dialog/current/current-wind-moderate-location.dialog
+locale/pt-pt/dialog/current/current-wind-strong-local.dialog
+locale/pt-pt/dialog/current/current-wind-strong-location.dialog
+locale/pt-pt/dialog/current/currrent-clouds-alternative-local.dialog
+locale/pt-pt/dialog/daily/daily-condition-expected-local.dialog
+locale/pt-pt/dialog/daily/daily-condition-expected-location.dialog
+locale/pt-pt/dialog/daily/daily-condition-not-expected-local.dialog
+locale/pt-pt/dialog/daily/daily-condition-not-expected-location.dialog
+locale/pt-pt/dialog/daily/daily-humidity-local.dialog
+locale/pt-pt/dialog/daily/daily-humidity-location.dialog
+locale/pt-pt/dialog/daily/daily-precipitation-next-local.dialog
+locale/pt-pt/dialog/daily/daily-precipitation-next-location.dialog
+locale/pt-pt/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/pt-pt/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/pt-pt/dialog/daily/daily-sunrise-local.dialog
+locale/pt-pt/dialog/daily/daily-sunrise-location.dialog
+locale/pt-pt/dialog/daily/daily-sunset-local.dialog
+locale/pt-pt/dialog/daily/daily-sunset-location.dialog
+locale/pt-pt/dialog/daily/daily-temperature-high-local.dialog
+locale/pt-pt/dialog/daily/daily-temperature-high-location.dialog
+locale/pt-pt/dialog/daily/daily-temperature-local.dialog
+locale/pt-pt/dialog/daily/daily-temperature-location.dialog
+locale/pt-pt/dialog/daily/daily-temperature-low-local.dialog
+locale/pt-pt/dialog/daily/daily-temperature-low-location.dialog
+locale/pt-pt/dialog/daily/daily-weather-local.dialog
+locale/pt-pt/dialog/daily/daily-weather-location.dialog
+locale/pt-pt/dialog/daily/daily-wind-light-local.dialog
+locale/pt-pt/dialog/daily/daily-wind-light-location.dialog
+locale/pt-pt/dialog/daily/daily-wind-moderate-local.dialog
+locale/pt-pt/dialog/daily/daily-wind-moderate-location.dialog
+locale/pt-pt/dialog/daily/daily-wind-strong-local.dialog
+locale/pt-pt/dialog/daily/daily-wind-strong-location.dialog
+locale/pt-pt/dialog/direction/east.dialog
+locale/pt-pt/dialog/direction/north.dialog
+locale/pt-pt/dialog/direction/northeast.dialog
+locale/pt-pt/dialog/direction/northwest.dialog
+locale/pt-pt/dialog/direction/south.dialog
+locale/pt-pt/dialog/direction/southeast.dialog
+locale/pt-pt/dialog/direction/southwest.dialog
+locale/pt-pt/dialog/direction/west.dialog
+locale/pt-pt/dialog/error/cant-get-forecast.dialog
+locale/pt-pt/dialog/error/forty-eight-hours-available.dialog
+locale/pt-pt/dialog/error/location-not-found.dialog
+locale/pt-pt/dialog/error/no-forecast.dialog
+locale/pt-pt/dialog/error/seven-days-available.dialog
+locale/pt-pt/dialog/hourly/hourly-condition-expected-local.dialog
+locale/pt-pt/dialog/hourly/hourly-condition-expected-location.dialog
+locale/pt-pt/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/pt-pt/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/pt-pt/dialog/hourly/hourly-temperature-local.dialog
+locale/pt-pt/dialog/hourly/hourly-temperature-location.dialog
+locale/pt-pt/dialog/hourly/hourly-weather-local.dialog
+locale/pt-pt/dialog/hourly/hourly-weather-location.dialog
+locale/pt-pt/dialog/unit/celsius.dialog
+locale/pt-pt/dialog/unit/fahrenheit.dialog
+locale/pt-pt/dialog/unit/inch.dialog
+locale/pt-pt/dialog/unit/meter per second.dialog
+locale/pt-pt/dialog/unit/miles per hour.dialog
+locale/pt-pt/dialog/unit/millimeter.dialog
+locale/pt-pt/dialog/weekly/weekly-condition.dialog
+locale/pt-pt/dialog/weekly/weekly-temperature.dialog
+locale/pt-pt/regex/location.rx
+locale/pt-pt/vocabulary/forecast.voc
+locale/pt-pt/vocabulary/location.voc
+locale/pt-pt/vocabulary/outside.voc
+locale/pt-pt/vocabulary/sunrise.voc
+locale/pt-pt/vocabulary/sunset.voc
+locale/pt-pt/vocabulary/weather.voc
+locale/pt-pt/vocabulary/condition/clear.voc
+locale/pt-pt/vocabulary/condition/clouds.voc
+locale/pt-pt/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/pt-pt/vocabulary/condition/fog.voc
+locale/pt-pt/vocabulary/condition/humidity.voc
+locale/pt-pt/vocabulary/condition/precipitation.voc
+locale/pt-pt/vocabulary/condition/rain.voc
+locale/pt-pt/vocabulary/condition/snow.voc
+locale/pt-pt/vocabulary/condition/thunderstorm.voc
+locale/pt-pt/vocabulary/condition/windy.voc
+locale/pt-pt/vocabulary/date-time/couple.voc
+locale/pt-pt/vocabulary/date-time/few.voc
+locale/pt-pt/vocabulary/date-time/later.voc
+locale/pt-pt/vocabulary/date-time/next.voc
+locale/pt-pt/vocabulary/date-time/now.voc
+locale/pt-pt/vocabulary/date-time/number-days.voc
+locale/pt-pt/vocabulary/date-time/relative-day.voc
+locale/pt-pt/vocabulary/date-time/relative-time.voc
+locale/pt-pt/vocabulary/date-time/today.voc
+locale/pt-pt/vocabulary/date-time/week.voc
+locale/pt-pt/vocabulary/date-time/weekend.voc
+locale/pt-pt/vocabulary/query/confirm-query-current.voc
+locale/pt-pt/vocabulary/query/confirm-query-future.voc
+locale/pt-pt/vocabulary/query/confirm-query.voc
+locale/pt-pt/vocabulary/query/how.voc
+locale/pt-pt/vocabulary/query/query.voc
+locale/pt-pt/vocabulary/query/when.voc
+locale/pt-pt/vocabulary/temperature/cold.voc
+locale/pt-pt/vocabulary/temperature/high.voc
+locale/pt-pt/vocabulary/temperature/hot.voc
+locale/pt-pt/vocabulary/temperature/low.voc
+locale/pt-pt/vocabulary/temperature/temperature.voc
+locale/pt-pt/vocabulary/unit/fahrenheit.voc
+locale/pt-pt/vocabulary/unit/unit.entity
+locale/pt-pt/vocabulary/unit/unit.voc
+locale/ru-ru/dialog/and.dialog
 locale/ru-ru/dialog/percentage-number.dialog
 locale/ru-ru/dialog/condition/ash.dialog
+locale/ru-ru/dialog/condition/clear-sky.dialog
 locale/ru-ru/dialog/condition/clear.dialog
 locale/ru-ru/dialog/condition/clouds.dialog
+locale/ru-ru/dialog/condition/depositing-rime-fog.dialog
+locale/ru-ru/dialog/condition/drizzle-dense-intensity.dialog
+locale/ru-ru/dialog/condition/drizzle-light-intensity.dialog
+locale/ru-ru/dialog/condition/drizzle-moderate-intensity.dialog
 locale/ru-ru/dialog/condition/drizzle.dialog
 locale/ru-ru/dialog/condition/dust.dialog
+locale/ru-ru/dialog/condition/fog.dialog
+locale/ru-ru/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/ru-ru/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/ru-ru/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/ru-ru/dialog/condition/freezing-rain-light-intensity.dialog
 locale/ru-ru/dialog/condition/haze.dialog
+locale/ru-ru/dialog/condition/heavy-rain.dialog
+locale/ru-ru/dialog/condition/heavy-snow-fall.dialog
+locale/ru-ru/dialog/condition/heavy-snow-showers.dialog
+locale/ru-ru/dialog/condition/humidity.dialog
+locale/ru-ru/dialog/condition/mainly-clear.dialog
 locale/ru-ru/dialog/condition/mist.dialog
+locale/ru-ru/dialog/condition/moderate-rain-showers.dialog
+locale/ru-ru/dialog/condition/moderate-rain.dialog
+locale/ru-ru/dialog/condition/moderate-snow-fall.dialog
+locale/ru-ru/dialog/condition/overcast.dialog
+locale/ru-ru/dialog/condition/partly-cloudy.dialog
 locale/ru-ru/dialog/condition/rain.dialog
+locale/ru-ru/dialog/condition/slight-rain-showers.dialog
+locale/ru-ru/dialog/condition/slight-rain.dialog
+locale/ru-ru/dialog/condition/slight-snow-fall.dialog
+locale/ru-ru/dialog/condition/slight-snow-showers.dialog
 locale/ru-ru/dialog/condition/smoke.dialog
+locale/ru-ru/dialog/condition/snow-grains.dialog
 locale/ru-ru/dialog/condition/snow.dialog
 locale/ru-ru/dialog/condition/squall.dialog
+locale/ru-ru/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/ru-ru/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/ru-ru/dialog/condition/thunderstorm.dialog
 locale/ru-ru/dialog/condition/tornado.dialog
+locale/ru-ru/dialog/condition/violent-rain-showers.dialog
+locale/ru-ru/dialog/current/current-condition-expected-local.dialog
+locale/ru-ru/dialog/current/current-condition-expected-location.dialog
+locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
+locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
+locale/ru-ru/dialog/current/current-humidity-local.dialog
+locale/ru-ru/dialog/current/current-humidity-location.dialog
+locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
+locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
+locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
+locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
+locale/ru-ru/dialog/current/current-sunset-future-local.dialog
+locale/ru-ru/dialog/current/current-sunset-future-location.dialog
+locale/ru-ru/dialog/current/current-sunset-past-local.dialog
+locale/ru-ru/dialog/current/current-sunset-past-location.dialog
+locale/ru-ru/dialog/current/current-temperature-local.dialog
+locale/ru-ru/dialog/current/current-temperature-location.dialog
+locale/ru-ru/dialog/current/current-weather-local.dialog
+locale/ru-ru/dialog/current/current-weather-location.dialog
+locale/ru-ru/dialog/current/current-wind-light-local.dialog
+locale/ru-ru/dialog/current/current-wind-light-location.dialog
+locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
+locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
+locale/ru-ru/dialog/current/current-wind-strong-local.dialog
+locale/ru-ru/dialog/current/current-wind-strong-location.dialog
+locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
+locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
+locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
+locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
+locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
+locale/ru-ru/dialog/daily/daily-humidity-local.dialog
+locale/ru-ru/dialog/daily/daily-humidity-location.dialog
+locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
+locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
+locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
+locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
+locale/ru-ru/dialog/daily/daily-sunset-local.dialog
+locale/ru-ru/dialog/daily/daily-sunset-location.dialog
+locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
+locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
+locale/ru-ru/dialog/daily/daily-temperature-local.dialog
+locale/ru-ru/dialog/daily/daily-temperature-location.dialog
+locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
+locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
 locale/ru-ru/dialog/daily/daily-weather-loation.dialog
+locale/ru-ru/dialog/daily/daily-weather-local.dialog
+locale/ru-ru/dialog/daily/daily-weather-location.dialog
+locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
+locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
+locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
+locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
+locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
+locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
 locale/ru-ru/dialog/direction/east.dialog
 locale/ru-ru/dialog/direction/north.dialog
 locale/ru-ru/dialog/direction/northeast.dialog
 locale/ru-ru/dialog/direction/northwest.dialog
 locale/ru-ru/dialog/direction/south.dialog
 locale/ru-ru/dialog/direction/southeast.dialog
 locale/ru-ru/dialog/direction/southwest.dialog
 locale/ru-ru/dialog/direction/west.dialog
+locale/ru-ru/dialog/error/cant-get-forecast.dialog
+locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
+locale/ru-ru/dialog/error/location-not-found.dialog
+locale/ru-ru/dialog/error/no-forecast.dialog
+locale/ru-ru/dialog/error/seven-days-available.dialog
+locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
+locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
+locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
+locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
+locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
+locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
 locale/ru-ru/dialog/unit/celsius.dialog
 locale/ru-ru/dialog/unit/fahrenheit.dialog
-locale/ru-ru/dialog/unit/meters per second.dialog
+locale/ru-ru/dialog/unit/inch.dialog
+locale/ru-ru/dialog/unit/meter per second.dialog
 locale/ru-ru/dialog/unit/miles per hour.dialog
+locale/ru-ru/dialog/unit/millimeter.dialog
+locale/ru-ru/dialog/weekly/weekly-condition.dialog
+locale/ru-ru/dialog/weekly/weekly-temperature.dialog
 locale/ru-ru/regex/location.rx
 locale/ru-ru/vocabulary/forecast.voc
 locale/ru-ru/vocabulary/location.voc
+locale/ru-ru/vocabulary/outside.voc
 locale/ru-ru/vocabulary/sunrise.voc
 locale/ru-ru/vocabulary/sunset.voc
 locale/ru-ru/vocabulary/weather.voc
+locale/ru-ru/vocabulary/condition/clear.voc
+locale/ru-ru/vocabulary/condition/clouds.voc
+locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/ru-ru/vocabulary/condition/fog.voc
 locale/ru-ru/vocabulary/condition/humidity.voc
 locale/ru-ru/vocabulary/condition/precipitation.voc
+locale/ru-ru/vocabulary/condition/rain.voc
+locale/ru-ru/vocabulary/condition/snow.voc
+locale/ru-ru/vocabulary/condition/thunderstorm.voc
 locale/ru-ru/vocabulary/condition/windy.voc
+locale/ru-ru/vocabulary/date-time/couple.voc
+locale/ru-ru/vocabulary/date-time/few.voc
 locale/ru-ru/vocabulary/date-time/later.voc
 locale/ru-ru/vocabulary/date-time/next.voc
+locale/ru-ru/vocabulary/date-time/now.voc
+locale/ru-ru/vocabulary/date-time/number-days.voc
+locale/ru-ru/vocabulary/date-time/relative-day.voc
+locale/ru-ru/vocabulary/date-time/relative-time.voc
+locale/ru-ru/vocabulary/date-time/today.voc
+locale/ru-ru/vocabulary/date-time/week.voc
+locale/ru-ru/vocabulary/date-time/weekend.voc
+locale/ru-ru/vocabulary/query/confirm-query-current.voc
+locale/ru-ru/vocabulary/query/confirm-query-future.voc
+locale/ru-ru/vocabulary/query/confirm-query.voc
+locale/ru-ru/vocabulary/query/how.voc
 locale/ru-ru/vocabulary/query/query.voc
+locale/ru-ru/vocabulary/query/when.voc
+locale/ru-ru/vocabulary/temperature/cold.voc
+locale/ru-ru/vocabulary/temperature/high.voc
+locale/ru-ru/vocabulary/temperature/hot.voc
+locale/ru-ru/vocabulary/temperature/low.voc
+locale/ru-ru/vocabulary/temperature/temperature.voc
+locale/ru-ru/vocabulary/unit/fahrenheit.voc
+locale/ru-ru/vocabulary/unit/unit.entity
+locale/ru-ru/vocabulary/unit/unit.voc
+locale/sv-fi/dialog/and.dialog
+locale/sv-fi/dialog/percentage-number.dialog
+locale/sv-fi/dialog/condition/ash.dialog
+locale/sv-fi/dialog/condition/clear-sky.dialog
+locale/sv-fi/dialog/condition/clear.dialog
+locale/sv-fi/dialog/condition/clouds.dialog
+locale/sv-fi/dialog/condition/depositing-rime-fog.dialog
+locale/sv-fi/dialog/condition/drizzle-dense-intensity.dialog
+locale/sv-fi/dialog/condition/drizzle-light-intensity.dialog
+locale/sv-fi/dialog/condition/drizzle-moderate-intensity.dialog
+locale/sv-fi/dialog/condition/drizzle.dialog
+locale/sv-fi/dialog/condition/dust.dialog
+locale/sv-fi/dialog/condition/fog.dialog
+locale/sv-fi/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/sv-fi/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/sv-fi/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/sv-fi/dialog/condition/freezing-rain-light-intensity.dialog
+locale/sv-fi/dialog/condition/haze.dialog
+locale/sv-fi/dialog/condition/heavy-rain.dialog
+locale/sv-fi/dialog/condition/heavy-snow-fall.dialog
+locale/sv-fi/dialog/condition/heavy-snow-showers.dialog
+locale/sv-fi/dialog/condition/humidity.dialog
+locale/sv-fi/dialog/condition/mainly-clear.dialog
+locale/sv-fi/dialog/condition/mist.dialog
+locale/sv-fi/dialog/condition/moderate-rain-showers.dialog
+locale/sv-fi/dialog/condition/moderate-rain.dialog
+locale/sv-fi/dialog/condition/moderate-snow-fall.dialog
+locale/sv-fi/dialog/condition/overcast.dialog
+locale/sv-fi/dialog/condition/partly-cloudy.dialog
+locale/sv-fi/dialog/condition/rain.dialog
+locale/sv-fi/dialog/condition/slight-rain-showers.dialog
+locale/sv-fi/dialog/condition/slight-rain.dialog
+locale/sv-fi/dialog/condition/slight-snow-fall.dialog
+locale/sv-fi/dialog/condition/slight-snow-showers.dialog
+locale/sv-fi/dialog/condition/smoke.dialog
+locale/sv-fi/dialog/condition/snow-grains.dialog
+locale/sv-fi/dialog/condition/snow.dialog
+locale/sv-fi/dialog/condition/squall.dialog
+locale/sv-fi/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/sv-fi/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/sv-fi/dialog/condition/thunderstorm.dialog
+locale/sv-fi/dialog/condition/tornado.dialog
+locale/sv-fi/dialog/condition/violent-rain-showers.dialog
+locale/sv-fi/dialog/current/current-condition-expected-local.dialog
+locale/sv-fi/dialog/current/current-condition-expected-location.dialog
+locale/sv-fi/dialog/current/current-condition-not-expected-local.dialog
+locale/sv-fi/dialog/current/current-condition-not-expected-location.dialog
+locale/sv-fi/dialog/current/current-humidity-local.dialog
+locale/sv-fi/dialog/current/current-humidity-location.dialog
+locale/sv-fi/dialog/current/current-sunrise-future-local.dialog
+locale/sv-fi/dialog/current/current-sunrise-future-location.dialog
+locale/sv-fi/dialog/current/current-sunrise-past-local.dialog
+locale/sv-fi/dialog/current/current-sunrise-past-location.dialog
+locale/sv-fi/dialog/current/current-sunset-future-local.dialog
+locale/sv-fi/dialog/current/current-sunset-future-location.dialog
+locale/sv-fi/dialog/current/current-sunset-past-local.dialog
+locale/sv-fi/dialog/current/current-sunset-past-location.dialog
+locale/sv-fi/dialog/current/current-temperature-local.dialog
+locale/sv-fi/dialog/current/current-temperature-location.dialog
+locale/sv-fi/dialog/current/current-weather-local.dialog
+locale/sv-fi/dialog/current/current-weather-location.dialog
+locale/sv-fi/dialog/current/current-wind-light-local.dialog
+locale/sv-fi/dialog/current/current-wind-light-location.dialog
+locale/sv-fi/dialog/current/current-wind-moderate-local.dialog
+locale/sv-fi/dialog/current/current-wind-moderate-location.dialog
+locale/sv-fi/dialog/current/current-wind-strong-local.dialog
+locale/sv-fi/dialog/current/current-wind-strong-location.dialog
+locale/sv-fi/dialog/current/currrent-clouds-alternative-local.dialog
+locale/sv-fi/dialog/daily/daily-condition-expected-local.dialog
+locale/sv-fi/dialog/daily/daily-condition-expected-location.dialog
+locale/sv-fi/dialog/daily/daily-condition-not-expected-local.dialog
+locale/sv-fi/dialog/daily/daily-condition-not-expected-location.dialog
+locale/sv-fi/dialog/daily/daily-humidity-local.dialog
+locale/sv-fi/dialog/daily/daily-humidity-location.dialog
+locale/sv-fi/dialog/daily/daily-precipitation-next-local.dialog
+locale/sv-fi/dialog/daily/daily-precipitation-next-location.dialog
+locale/sv-fi/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/sv-fi/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/sv-fi/dialog/daily/daily-sunrise-local.dialog
+locale/sv-fi/dialog/daily/daily-sunrise-location.dialog
+locale/sv-fi/dialog/daily/daily-sunset-local.dialog
+locale/sv-fi/dialog/daily/daily-sunset-location.dialog
+locale/sv-fi/dialog/daily/daily-temperature-high-local.dialog
+locale/sv-fi/dialog/daily/daily-temperature-high-location.dialog
+locale/sv-fi/dialog/daily/daily-temperature-local.dialog
+locale/sv-fi/dialog/daily/daily-temperature-location.dialog
+locale/sv-fi/dialog/daily/daily-temperature-low-local.dialog
+locale/sv-fi/dialog/daily/daily-temperature-low-location.dialog
+locale/sv-fi/dialog/daily/daily-weather-local.dialog
+locale/sv-fi/dialog/daily/daily-weather-location.dialog
+locale/sv-fi/dialog/daily/daily-wind-light-local.dialog
+locale/sv-fi/dialog/daily/daily-wind-light-location.dialog
+locale/sv-fi/dialog/daily/daily-wind-moderate-local.dialog
+locale/sv-fi/dialog/daily/daily-wind-moderate-location.dialog
+locale/sv-fi/dialog/daily/daily-wind-strong-local.dialog
+locale/sv-fi/dialog/daily/daily-wind-strong-location.dialog
+locale/sv-fi/dialog/direction/east.dialog
+locale/sv-fi/dialog/direction/north.dialog
+locale/sv-fi/dialog/direction/northeast.dialog
+locale/sv-fi/dialog/direction/northwest.dialog
+locale/sv-fi/dialog/direction/south.dialog
+locale/sv-fi/dialog/direction/southeast.dialog
+locale/sv-fi/dialog/direction/southwest.dialog
+locale/sv-fi/dialog/direction/west.dialog
+locale/sv-fi/dialog/error/cant-get-forecast.dialog
+locale/sv-fi/dialog/error/forty-eight-hours-available.dialog
+locale/sv-fi/dialog/error/location-not-found.dialog
+locale/sv-fi/dialog/error/no-forecast.dialog
+locale/sv-fi/dialog/error/seven-days-available.dialog
+locale/sv-fi/dialog/hourly/hourly-condition-expected-local.dialog
+locale/sv-fi/dialog/hourly/hourly-condition-expected-location.dialog
+locale/sv-fi/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/sv-fi/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/sv-fi/dialog/hourly/hourly-temperature-local.dialog
+locale/sv-fi/dialog/hourly/hourly-temperature-location.dialog
+locale/sv-fi/dialog/hourly/hourly-weather-local.dialog
+locale/sv-fi/dialog/hourly/hourly-weather-location.dialog
+locale/sv-fi/dialog/unit/celsius.dialog
+locale/sv-fi/dialog/unit/fahrenheit.dialog
+locale/sv-fi/dialog/unit/inch.dialog
+locale/sv-fi/dialog/unit/meter per second.dialog
+locale/sv-fi/dialog/unit/miles per hour.dialog
+locale/sv-fi/dialog/unit/millimeter.dialog
+locale/sv-fi/dialog/weekly/weekly-condition.dialog
+locale/sv-fi/dialog/weekly/weekly-temperature.dialog
+locale/sv-fi/regex/location.rx
+locale/sv-fi/vocabulary/forecast.voc
+locale/sv-fi/vocabulary/location.voc
+locale/sv-fi/vocabulary/outside.voc
+locale/sv-fi/vocabulary/sunrise.voc
+locale/sv-fi/vocabulary/sunset.voc
+locale/sv-fi/vocabulary/weather.voc
+locale/sv-fi/vocabulary/condition/clear.voc
+locale/sv-fi/vocabulary/condition/clouds.voc
+locale/sv-fi/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/sv-fi/vocabulary/condition/fog.voc
+locale/sv-fi/vocabulary/condition/humidity.voc
+locale/sv-fi/vocabulary/condition/precipitation.voc
+locale/sv-fi/vocabulary/condition/rain.voc
+locale/sv-fi/vocabulary/condition/snow.voc
+locale/sv-fi/vocabulary/condition/thunderstorm.voc
+locale/sv-fi/vocabulary/condition/windy.voc
+locale/sv-fi/vocabulary/date-time/couple.voc
+locale/sv-fi/vocabulary/date-time/few.voc
+locale/sv-fi/vocabulary/date-time/later.voc
+locale/sv-fi/vocabulary/date-time/next.voc
+locale/sv-fi/vocabulary/date-time/now.voc
+locale/sv-fi/vocabulary/date-time/number-days.voc
+locale/sv-fi/vocabulary/date-time/relative-day.voc
+locale/sv-fi/vocabulary/date-time/relative-time.voc
+locale/sv-fi/vocabulary/date-time/today.voc
+locale/sv-fi/vocabulary/date-time/week.voc
+locale/sv-fi/vocabulary/date-time/weekend.voc
+locale/sv-fi/vocabulary/query/confirm-query-current.voc
+locale/sv-fi/vocabulary/query/confirm-query-future.voc
+locale/sv-fi/vocabulary/query/confirm-query.voc
+locale/sv-fi/vocabulary/query/how.voc
+locale/sv-fi/vocabulary/query/query.voc
+locale/sv-fi/vocabulary/query/when.voc
+locale/sv-fi/vocabulary/temperature/cold.voc
+locale/sv-fi/vocabulary/temperature/high.voc
+locale/sv-fi/vocabulary/temperature/hot.voc
+locale/sv-fi/vocabulary/temperature/low.voc
+locale/sv-fi/vocabulary/temperature/temperature.voc
+locale/sv-fi/vocabulary/unit/fahrenheit.voc
+locale/sv-fi/vocabulary/unit/unit.entity
+locale/sv-fi/vocabulary/unit/unit.voc
 locale/sv-se/dialog/and.dialog
 locale/sv-se/dialog/percentage-number.dialog
 locale/sv-se/dialog/condition/ash.dialog
+locale/sv-se/dialog/condition/clear-sky.dialog
 locale/sv-se/dialog/condition/clear.dialog
 locale/sv-se/dialog/condition/clouds.dialog
+locale/sv-se/dialog/condition/depositing-rime-fog.dialog
+locale/sv-se/dialog/condition/drizzle-dense-intensity.dialog
+locale/sv-se/dialog/condition/drizzle-light-intensity.dialog
+locale/sv-se/dialog/condition/drizzle-moderate-intensity.dialog
 locale/sv-se/dialog/condition/drizzle.dialog
 locale/sv-se/dialog/condition/dust.dialog
+locale/sv-se/dialog/condition/fog.dialog
+locale/sv-se/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/sv-se/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/sv-se/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/sv-se/dialog/condition/freezing-rain-light-intensity.dialog
 locale/sv-se/dialog/condition/haze.dialog
+locale/sv-se/dialog/condition/heavy-rain.dialog
+locale/sv-se/dialog/condition/heavy-snow-fall.dialog
+locale/sv-se/dialog/condition/heavy-snow-showers.dialog
+locale/sv-se/dialog/condition/humidity.dialog
+locale/sv-se/dialog/condition/mainly-clear.dialog
 locale/sv-se/dialog/condition/mist.dialog
+locale/sv-se/dialog/condition/moderate-rain-showers.dialog
+locale/sv-se/dialog/condition/moderate-rain.dialog
+locale/sv-se/dialog/condition/moderate-snow-fall.dialog
+locale/sv-se/dialog/condition/overcast.dialog
+locale/sv-se/dialog/condition/partly-cloudy.dialog
 locale/sv-se/dialog/condition/rain.dialog
+locale/sv-se/dialog/condition/slight-rain-showers.dialog
+locale/sv-se/dialog/condition/slight-rain.dialog
+locale/sv-se/dialog/condition/slight-snow-fall.dialog
+locale/sv-se/dialog/condition/slight-snow-showers.dialog
 locale/sv-se/dialog/condition/smoke.dialog
+locale/sv-se/dialog/condition/snow-grains.dialog
 locale/sv-se/dialog/condition/snow.dialog
 locale/sv-se/dialog/condition/squall.dialog
+locale/sv-se/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/sv-se/dialog/condition/thunderstorm-with-slight-hail.dialog
 locale/sv-se/dialog/condition/thunderstorm.dialog
 locale/sv-se/dialog/condition/tornado.dialog
+locale/sv-se/dialog/condition/violent-rain-showers.dialog
 locale/sv-se/dialog/current/current-condition-expected-local.dialog
 locale/sv-se/dialog/current/current-condition-expected-location.dialog
+locale/sv-se/dialog/current/current-condition-not-expected-local.dialog
+locale/sv-se/dialog/current/current-condition-not-expected-location.dialog
+locale/sv-se/dialog/current/current-humidity-local.dialog
+locale/sv-se/dialog/current/current-humidity-location.dialog
+locale/sv-se/dialog/current/current-sunrise-future-local.dialog
+locale/sv-se/dialog/current/current-sunrise-future-location.dialog
+locale/sv-se/dialog/current/current-sunrise-past-local.dialog
+locale/sv-se/dialog/current/current-sunrise-past-location.dialog
+locale/sv-se/dialog/current/current-sunset-future-local.dialog
+locale/sv-se/dialog/current/current-sunset-future-location.dialog
+locale/sv-se/dialog/current/current-sunset-past-local.dialog
+locale/sv-se/dialog/current/current-sunset-past-location.dialog
+locale/sv-se/dialog/current/current-temperature-local.dialog
+locale/sv-se/dialog/current/current-temperature-location.dialog
+locale/sv-se/dialog/current/current-weather-local.dialog
+locale/sv-se/dialog/current/current-weather-location.dialog
+locale/sv-se/dialog/current/current-wind-light-local.dialog
+locale/sv-se/dialog/current/current-wind-light-location.dialog
+locale/sv-se/dialog/current/current-wind-moderate-local.dialog
+locale/sv-se/dialog/current/current-wind-moderate-location.dialog
+locale/sv-se/dialog/current/current-wind-strong-local.dialog
+locale/sv-se/dialog/current/current-wind-strong-location.dialog
+locale/sv-se/dialog/current/currrent-clouds-alternative-local.dialog
+locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
 locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
+locale/sv-se/dialog/daily/daily-condition-not-expected-local.dialog
+locale/sv-se/dialog/daily/daily-condition-not-expected-location.dialog
+locale/sv-se/dialog/daily/daily-humidity-local.dialog
+locale/sv-se/dialog/daily/daily-humidity-location.dialog
+locale/sv-se/dialog/daily/daily-precipitation-next-local.dialog
+locale/sv-se/dialog/daily/daily-precipitation-next-location.dialog
+locale/sv-se/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/sv-se/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/sv-se/dialog/daily/daily-sunrise-local.dialog
+locale/sv-se/dialog/daily/daily-sunrise-location.dialog
+locale/sv-se/dialog/daily/daily-sunset-local.dialog
+locale/sv-se/dialog/daily/daily-sunset-location.dialog
+locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
+locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
+locale/sv-se/dialog/daily/daily-temperature-local.dialog
+locale/sv-se/dialog/daily/daily-temperature-location.dialog
+locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
+locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
+locale/sv-se/dialog/daily/daily-weather-local.dialog
+locale/sv-se/dialog/daily/daily-weather-location.dialog
+locale/sv-se/dialog/daily/daily-wind-light-local.dialog
+locale/sv-se/dialog/daily/daily-wind-light-location.dialog
+locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
+locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
+locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
+locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
 locale/sv-se/dialog/direction/east.dialog
 locale/sv-se/dialog/direction/north.dialog
 locale/sv-se/dialog/direction/northeast.dialog
 locale/sv-se/dialog/direction/northwest.dialog
 locale/sv-se/dialog/direction/south.dialog
 locale/sv-se/dialog/direction/southeast.dialog
 locale/sv-se/dialog/direction/southwest.dialog
 locale/sv-se/dialog/direction/west.dialog
 locale/sv-se/dialog/error/cant-get-forecast.dialog
+locale/sv-se/dialog/error/forty-eight-hours-available.dialog
+locale/sv-se/dialog/error/location-not-found.dialog
 locale/sv-se/dialog/error/no-forecast.dialog
+locale/sv-se/dialog/error/seven-days-available.dialog
 locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
 locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
 locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
 locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
 locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
 locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
+locale/sv-se/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/sv-se/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
+locale/sv-se/dialog/hourly/hourly-temperature-location.dialog
+locale/sv-se/dialog/hourly/hourly-weather-local.dialog
+locale/sv-se/dialog/hourly/hourly-weather-location.dialog
 locale/sv-se/dialog/unit/celsius.dialog
 locale/sv-se/dialog/unit/fahrenheit.dialog
-locale/sv-se/dialog/unit/meters per second.dialog
+locale/sv-se/dialog/unit/inch.dialog
+locale/sv-se/dialog/unit/meter per second.dialog
 locale/sv-se/dialog/unit/miles per hour.dialog
+locale/sv-se/dialog/unit/millimeter.dialog
+locale/sv-se/dialog/weekly/weekly-condition.dialog
 locale/sv-se/dialog/weekly/weekly-temperature.dialog
 locale/sv-se/regex/location.rx
 locale/sv-se/vocabulary/forecast.voc
 locale/sv-se/vocabulary/location.voc
+locale/sv-se/vocabulary/outside.voc
 locale/sv-se/vocabulary/sunrise.voc
 locale/sv-se/vocabulary/sunset.voc
 locale/sv-se/vocabulary/weather.voc
 locale/sv-se/vocabulary/condition/clear.voc
 locale/sv-se/vocabulary/condition/clouds.voc
+locale/sv-se/vocabulary/condition/do-i-need-an-umbrella.intent
 locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
 locale/sv-se/vocabulary/condition/humidity.voc
 locale/sv-se/vocabulary/condition/precipitation.voc
 locale/sv-se/vocabulary/condition/rain.voc
 locale/sv-se/vocabulary/condition/snow.voc
 locale/sv-se/vocabulary/condition/thunderstorm.voc
 locale/sv-se/vocabulary/condition/windy.voc
 locale/sv-se/vocabulary/date-time/couple.voc
+locale/sv-se/vocabulary/date-time/few.voc
 locale/sv-se/vocabulary/date-time/later.voc
 locale/sv-se/vocabulary/date-time/next.voc
 locale/sv-se/vocabulary/date-time/now.voc
+locale/sv-se/vocabulary/date-time/number-days.voc
 locale/sv-se/vocabulary/date-time/relative-day.voc
 locale/sv-se/vocabulary/date-time/relative-time.voc
 locale/sv-se/vocabulary/date-time/today.voc
 locale/sv-se/vocabulary/date-time/week.voc
 locale/sv-se/vocabulary/date-time/weekend.voc
 locale/sv-se/vocabulary/query/confirm-query-current.voc
 locale/sv-se/vocabulary/query/confirm-query-future.voc
@@ -1090,14 +2770,181 @@
 locale/sv-se/vocabulary/temperature/high.voc
 locale/sv-se/vocabulary/temperature/hot.voc
 locale/sv-se/vocabulary/temperature/low.voc
 locale/sv-se/vocabulary/temperature/temperature.voc
 locale/sv-se/vocabulary/unit/fahrenheit.voc
 locale/sv-se/vocabulary/unit/unit.entity
 locale/sv-se/vocabulary/unit/unit.voc
+locale/tr-tr/dialog/and.dialog
+locale/tr-tr/dialog/percentage-number.dialog
+locale/tr-tr/dialog/condition/ash.dialog
+locale/tr-tr/dialog/condition/clear-sky.dialog
+locale/tr-tr/dialog/condition/clear.dialog
+locale/tr-tr/dialog/condition/clouds.dialog
+locale/tr-tr/dialog/condition/depositing-rime-fog.dialog
+locale/tr-tr/dialog/condition/drizzle-dense-intensity.dialog
+locale/tr-tr/dialog/condition/drizzle-light-intensity.dialog
+locale/tr-tr/dialog/condition/drizzle-moderate-intensity.dialog
+locale/tr-tr/dialog/condition/drizzle.dialog
+locale/tr-tr/dialog/condition/dust.dialog
+locale/tr-tr/dialog/condition/fog.dialog
+locale/tr-tr/dialog/condition/freezing-drizzle-dense-intensity.dialog
+locale/tr-tr/dialog/condition/freezing-drizzle-light-intensity.dialog
+locale/tr-tr/dialog/condition/freezing-rain-dense-intensity.dialog
+locale/tr-tr/dialog/condition/freezing-rain-light-intensity.dialog
+locale/tr-tr/dialog/condition/haze.dialog
+locale/tr-tr/dialog/condition/heavy-rain.dialog
+locale/tr-tr/dialog/condition/heavy-snow-fall.dialog
+locale/tr-tr/dialog/condition/heavy-snow-showers.dialog
+locale/tr-tr/dialog/condition/humidity.dialog
+locale/tr-tr/dialog/condition/mainly-clear.dialog
+locale/tr-tr/dialog/condition/mist.dialog
+locale/tr-tr/dialog/condition/moderate-rain-showers.dialog
+locale/tr-tr/dialog/condition/moderate-rain.dialog
+locale/tr-tr/dialog/condition/moderate-snow-fall.dialog
+locale/tr-tr/dialog/condition/overcast.dialog
+locale/tr-tr/dialog/condition/partly-cloudy.dialog
+locale/tr-tr/dialog/condition/rain.dialog
+locale/tr-tr/dialog/condition/slight-rain-showers.dialog
+locale/tr-tr/dialog/condition/slight-rain.dialog
+locale/tr-tr/dialog/condition/slight-snow-fall.dialog
+locale/tr-tr/dialog/condition/slight-snow-showers.dialog
+locale/tr-tr/dialog/condition/smoke.dialog
+locale/tr-tr/dialog/condition/snow-grains.dialog
+locale/tr-tr/dialog/condition/snow.dialog
+locale/tr-tr/dialog/condition/squall.dialog
+locale/tr-tr/dialog/condition/thunderstorm-with-heavy-hail.dialog
+locale/tr-tr/dialog/condition/thunderstorm-with-slight-hail.dialog
+locale/tr-tr/dialog/condition/thunderstorm.dialog
+locale/tr-tr/dialog/condition/tornado.dialog
+locale/tr-tr/dialog/condition/violent-rain-showers.dialog
+locale/tr-tr/dialog/current/current-condition-expected-local.dialog
+locale/tr-tr/dialog/current/current-condition-expected-location.dialog
+locale/tr-tr/dialog/current/current-condition-not-expected-local.dialog
+locale/tr-tr/dialog/current/current-condition-not-expected-location.dialog
+locale/tr-tr/dialog/current/current-humidity-local.dialog
+locale/tr-tr/dialog/current/current-humidity-location.dialog
+locale/tr-tr/dialog/current/current-sunrise-future-local.dialog
+locale/tr-tr/dialog/current/current-sunrise-future-location.dialog
+locale/tr-tr/dialog/current/current-sunrise-past-local.dialog
+locale/tr-tr/dialog/current/current-sunrise-past-location.dialog
+locale/tr-tr/dialog/current/current-sunset-future-local.dialog
+locale/tr-tr/dialog/current/current-sunset-future-location.dialog
+locale/tr-tr/dialog/current/current-sunset-past-local.dialog
+locale/tr-tr/dialog/current/current-sunset-past-location.dialog
+locale/tr-tr/dialog/current/current-temperature-local.dialog
+locale/tr-tr/dialog/current/current-temperature-location.dialog
+locale/tr-tr/dialog/current/current-weather-local.dialog
+locale/tr-tr/dialog/current/current-weather-location.dialog
+locale/tr-tr/dialog/current/current-wind-light-local.dialog
+locale/tr-tr/dialog/current/current-wind-light-location.dialog
+locale/tr-tr/dialog/current/current-wind-moderate-local.dialog
+locale/tr-tr/dialog/current/current-wind-moderate-location.dialog
+locale/tr-tr/dialog/current/current-wind-strong-local.dialog
+locale/tr-tr/dialog/current/current-wind-strong-location.dialog
+locale/tr-tr/dialog/current/currrent-clouds-alternative-local.dialog
+locale/tr-tr/dialog/daily/daily-condition-expected-local.dialog
+locale/tr-tr/dialog/daily/daily-condition-expected-location.dialog
+locale/tr-tr/dialog/daily/daily-condition-not-expected-local.dialog
+locale/tr-tr/dialog/daily/daily-condition-not-expected-location.dialog
+locale/tr-tr/dialog/daily/daily-humidity-local.dialog
+locale/tr-tr/dialog/daily/daily-humidity-location.dialog
+locale/tr-tr/dialog/daily/daily-precipitation-next-local.dialog
+locale/tr-tr/dialog/daily/daily-precipitation-next-location.dialog
+locale/tr-tr/dialog/daily/daily-precipitation-next-none-local.dialog
+locale/tr-tr/dialog/daily/daily-precipitation-next-none-location.dialog
+locale/tr-tr/dialog/daily/daily-sunrise-local.dialog
+locale/tr-tr/dialog/daily/daily-sunrise-location.dialog
+locale/tr-tr/dialog/daily/daily-sunset-local.dialog
+locale/tr-tr/dialog/daily/daily-sunset-location.dialog
+locale/tr-tr/dialog/daily/daily-temperature-high-local.dialog
+locale/tr-tr/dialog/daily/daily-temperature-high-location.dialog
+locale/tr-tr/dialog/daily/daily-temperature-local.dialog
+locale/tr-tr/dialog/daily/daily-temperature-location.dialog
+locale/tr-tr/dialog/daily/daily-temperature-low-local.dialog
+locale/tr-tr/dialog/daily/daily-temperature-low-location.dialog
+locale/tr-tr/dialog/daily/daily-weather-local.dialog
+locale/tr-tr/dialog/daily/daily-weather-location.dialog
+locale/tr-tr/dialog/daily/daily-wind-light-local.dialog
+locale/tr-tr/dialog/daily/daily-wind-light-location.dialog
+locale/tr-tr/dialog/daily/daily-wind-moderate-local.dialog
+locale/tr-tr/dialog/daily/daily-wind-moderate-location.dialog
+locale/tr-tr/dialog/daily/daily-wind-strong-local.dialog
+locale/tr-tr/dialog/daily/daily-wind-strong-location.dialog
+locale/tr-tr/dialog/direction/east.dialog
+locale/tr-tr/dialog/direction/north.dialog
+locale/tr-tr/dialog/direction/northeast.dialog
+locale/tr-tr/dialog/direction/northwest.dialog
+locale/tr-tr/dialog/direction/south.dialog
+locale/tr-tr/dialog/direction/southeast.dialog
+locale/tr-tr/dialog/direction/southwest.dialog
+locale/tr-tr/dialog/direction/west.dialog
+locale/tr-tr/dialog/error/cant-get-forecast.dialog
+locale/tr-tr/dialog/error/forty-eight-hours-available.dialog
+locale/tr-tr/dialog/error/location-not-found.dialog
+locale/tr-tr/dialog/error/no-forecast.dialog
+locale/tr-tr/dialog/error/seven-days-available.dialog
+locale/tr-tr/dialog/hourly/hourly-condition-expected-local.dialog
+locale/tr-tr/dialog/hourly/hourly-condition-expected-location.dialog
+locale/tr-tr/dialog/hourly/hourly-precipitation-next-local.dialog
+locale/tr-tr/dialog/hourly/hourly-precipitation-next-location.dialog
+locale/tr-tr/dialog/hourly/hourly-temperature-local.dialog
+locale/tr-tr/dialog/hourly/hourly-temperature-location.dialog
+locale/tr-tr/dialog/hourly/hourly-weather-local.dialog
+locale/tr-tr/dialog/hourly/hourly-weather-location.dialog
+locale/tr-tr/dialog/unit/celsius.dialog
+locale/tr-tr/dialog/unit/fahrenheit.dialog
+locale/tr-tr/dialog/unit/inch.dialog
+locale/tr-tr/dialog/unit/meter per second.dialog
+locale/tr-tr/dialog/unit/miles per hour.dialog
+locale/tr-tr/dialog/unit/millimeter.dialog
+locale/tr-tr/dialog/weekly/weekly-condition.dialog
+locale/tr-tr/dialog/weekly/weekly-temperature.dialog
+locale/tr-tr/regex/location.rx
+locale/tr-tr/vocabulary/forecast.voc
+locale/tr-tr/vocabulary/location.voc
+locale/tr-tr/vocabulary/outside.voc
+locale/tr-tr/vocabulary/sunrise.voc
+locale/tr-tr/vocabulary/sunset.voc
+locale/tr-tr/vocabulary/weather.voc
+locale/tr-tr/vocabulary/condition/clear.voc
+locale/tr-tr/vocabulary/condition/clouds.voc
+locale/tr-tr/vocabulary/condition/do-i-need-an-umbrella.intent
+locale/tr-tr/vocabulary/condition/fog.voc
+locale/tr-tr/vocabulary/condition/humidity.voc
+locale/tr-tr/vocabulary/condition/precipitation.voc
+locale/tr-tr/vocabulary/condition/rain.voc
+locale/tr-tr/vocabulary/condition/snow.voc
+locale/tr-tr/vocabulary/condition/thunderstorm.voc
+locale/tr-tr/vocabulary/condition/windy.voc
+locale/tr-tr/vocabulary/date-time/couple.voc
+locale/tr-tr/vocabulary/date-time/few.voc
+locale/tr-tr/vocabulary/date-time/later.voc
+locale/tr-tr/vocabulary/date-time/next.voc
+locale/tr-tr/vocabulary/date-time/now.voc
+locale/tr-tr/vocabulary/date-time/number-days.voc
+locale/tr-tr/vocabulary/date-time/relative-day.voc
+locale/tr-tr/vocabulary/date-time/relative-time.voc
+locale/tr-tr/vocabulary/date-time/today.voc
+locale/tr-tr/vocabulary/date-time/week.voc
+locale/tr-tr/vocabulary/date-time/weekend.voc
+locale/tr-tr/vocabulary/query/confirm-query-current.voc
+locale/tr-tr/vocabulary/query/confirm-query-future.voc
+locale/tr-tr/vocabulary/query/confirm-query.voc
+locale/tr-tr/vocabulary/query/how.voc
+locale/tr-tr/vocabulary/query/query.voc
+locale/tr-tr/vocabulary/query/when.voc
+locale/tr-tr/vocabulary/temperature/cold.voc
+locale/tr-tr/vocabulary/temperature/high.voc
+locale/tr-tr/vocabulary/temperature/hot.voc
+locale/tr-tr/vocabulary/temperature/low.voc
+locale/tr-tr/vocabulary/temperature/temperature.voc
+locale/tr-tr/vocabulary/unit/fahrenheit.voc
+locale/tr-tr/vocabulary/unit/unit.entity
+locale/tr-tr/vocabulary/unit/unit.voc
 ovos_skill_weather.egg-info/PKG-INFO
 ovos_skill_weather.egg-info/SOURCES.txt
 ovos_skill_weather.egg-info/dependency_links.txt
 ovos_skill_weather.egg-info/entry_points.txt
 ovos_skill_weather.egg-info/requires.txt
 ovos_skill_weather.egg-info/top_level.txt
 res/desktop/skill.json
@@ -1122,14 +2969,15 @@
 ui/backgrounds/Rainy.qml
 ui/backgrounds/Simple.qml
 ui/backgrounds/Snowy.qml
 ui/backgrounds/qmldir
 ui/backgrounds/components/Rain.qml
 ui/backgrounds/components/Snow.qml
 ui/backgrounds/components/qmldir
+ui/images/chanceprecipitation.svg
 ui/images/clouds.svg
 ui/images/day.jpg
 ui/images/fog.svg
 ui/images/high_temperature.svg
 ui/images/humidity.svg
 ui/images/low_temperature.svg
 ui/images/moon.svg
```

## skill_ovos_weather/ovos_skill_weather.egg-info/requires.txt

```diff
@@ -1,8 +1,8 @@
-requests
+requests>=2.31.0
 pytz
 ovos-utils>=0.0.28a4,~=0.0
 ovos_workshop>=0.0.12a27,~=0.0
 
 [test]
 pytest
 pytest-cov
```

## skill_ovos_weather/ui/CurrentWeather.qml

```diff
@@ -15,14 +15,60 @@
         anchors.top: parent.top
         anchors.right: parent.right
         width: parent.width / 4
         height: locBoxHeight + locBoxHeight * 0.5
         spacing: Kirigami.Units.smallSpacing * 0.5
 
         Row {
+            id: precipitationRow
+            spacing: Mycroft.Units.gridUnit
+            height: parent.height / 2
+            width: parent.width
+
+            Item {
+                id: precipitationIconBox
+                width: parent.width / 2
+                height: parent.height
+
+                Image {
+                    id: precipitationIcon
+                    anchors.verticalCenter: parent.verticalCenter
+                    anchors.horizontalCenter: parent.horizontalCenter
+                    width: parent.height * 0.90
+                    height: width
+                    fillMode: Image.PreserveAspectFit
+                    source: "images/chanceprecipitation.svg"
+                }
+            }
+
+            Item {
+                width: parent.width - (windIconBox.width + Mycroft.Units.gridUnit)
+                height: parent.height
+                anchors.bottom: parent.bottom
+
+                Label {
+                    id: precipitation
+                    width: parent.width
+                    height: parent.height
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    font.weight: Font.Bold
+                    font.pixelSize: parent.width > parent.height ? height * 0.90 : width * 0.90
+                    color: dayNightTime == "day" ? "black" : "white"
+                    text: sessionData.chanceOfPrecipitation
+                }
+            }
+        }
+
+        Kirigami.Separator {
+            width: parent.width
+            height: 1
+        }
+
+        Row {
             id: windRow
             spacing: Mycroft.Units.gridUnit
             height: parent.height / 2
             width: parent.width
 
             Item {
                 id: windIconBox
```

## skill_ovos_weather/ui/SingleDay.qml

```diff
@@ -7,14 +7,109 @@
 import org.kde.lottie 1.0
 
 WeatherDelegate {
     id: root
     weatherCode: sessionData.weatherCode
     dateTimeLabelText: sessionData.weatherDate
 
+    Column {
+        id: locBoxDetailsArea
+        anchors.top: parent.top
+        anchors.right: parent.right
+        width: parent.width / 4
+        height: locBoxHeight + locBoxHeight * 0.5
+        spacing: Kirigami.Units.smallSpacing * 0.5
+
+        Row {
+            id: windRow
+            spacing: Mycroft.Units.gridUnit
+            height: parent.height / 2
+            width: parent.width
+
+            Item {
+                id: windIconBox
+                width: parent.width / 2
+                height: parent.height
+
+                Image {
+                    id: windIcon
+                    anchors.verticalCenter: parent.verticalCenter
+                    anchors.horizontalCenter: parent.horizontalCenter
+                    width: parent.height * 0.90
+                    height: width
+                    fillMode: Image.PreserveAspectFit
+                    source: "images/wind.svg"
+                }
+            }
+
+            Item {
+                width: parent.width - (windIconBox.width + Mycroft.Units.gridUnit)
+                height: parent.height
+                anchors.bottom: parent.bottom
+
+                Label {
+                    id: windSpeed
+                    width: parent.width
+                    height: parent.height
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    font.weight: Font.Bold
+                    font.pixelSize: parent.width > parent.height ? height * 0.90 : width * 0.90
+                    color: dayNightTime == "day" ? "black" : "white"
+                    text: sessionData.windSpeed
+                }
+            }
+        }
+
+        Kirigami.Separator {
+            width: parent.width
+            height: 1
+        }
+
+        Row {
+            id: humidityRow
+            spacing: Mycroft.Units.gridUnit
+            height: parent.height / 2
+            width: parent.width
+
+            Item {
+                id: humidityIconBox
+                width: parent.width / 2
+                height: parent.height
+
+                Image {
+                    id: humidityIcon
+                    anchors.verticalCenter: parent.verticalCenter
+                    anchors.horizontalCenter: parent.horizontalCenter
+                    width: parent.height * 0.90
+                    height: width
+                    fillMode: Image.PreserveAspectFit
+                    source: "images/humidity.svg"
+                }
+            }
+
+            Item {
+                width: parent.width - (humidityIconBox.width + Mycroft.Units.gridUnit)
+                height: parent.height
+
+                Label {
+                    id: humidityPercentage
+                    width: parent.width
+                    height: parent.height
+                    horizontalAlignment: Text.AlignHCenter
+                    verticalAlignment: Text.AlignVCenter
+                    font.weight: Font.Bold
+                    font.pixelSize: parent.width > parent.height ? height * 0.90 : width * 0.90
+                    color: dayNightTime == "day" ? "black" : "white"
+                    text: sessionData.humidity
+                }
+            }
+        }
+    }
+
     Rectangle {
         anchors.top: parent.top
         anchors.topMargin: root.locBoxHeight
         anchors.bottom: weatherInfoBox.top
         color: "transparent"
         width: parent.width
 
@@ -35,32 +130,61 @@
         id: weatherInfoBox
         anchors.bottom: parent.bottom
         anchors.horizontalCenter: parent.horizontalCenter
         width: parent.width
         color: "transparent"
         height: parent.height / 2
 
-        Item {
+        ColumnLayout {
             anchors.left: parent.left
             anchors.right: sept1.left
-            anchors.rightMargin: Mycroft.Units.gridUnit
+            anchors.leftMargin: Mycroft.Units.gridUnit
             height: parent.height
 
-            Label {
-                id: precipitation
-                width: parent.width
-                height: parent.height
-                anchors.centerIn: parent
-                horizontalAlignment: Text.AlignHCenter
-                verticalAlignment: Text.AlignVCenter
-                font.weight: Font.Bold
-                font.pixelSize: parent.width > parent.height ? height * 0.60 : width * 0.60
-                rightPadding: -font.pixelSize * 0.1
-                color: dayNightTime == "day" ? "black" : "white"
-                text: sessionData.chanceOfPrecipitation + "%"
+            Row {
+                Layout.fillWidth: true
+                Layout.preferredHeight: parent.height * 0.50
+                spacing: parent.width > parent.height ? Mycroft.Units.gridUnit * 2 : Mycroft.Units.gridUnit
+
+                Rectangle {
+                    id: pricipitationChanceBox
+                    width: parent.width / 4
+                    height: parent.height
+                    color: "transparent"
+
+                    Image {
+                            id: precipitationIcon
+                            anchors.verticalCenter: parent.verticalCenter
+                            anchors.left: parent.left
+                            width: parent.height * 0.50
+                            height: width
+                            fillMode: Image.PreserveAspectFit
+                            source: "images/chanceprecipitation.svg"
+                    }
+                }
+
+                Rectangle {
+                    width: parent.width - precipitationIcon.width
+                    height: parent.height
+                    anchors.bottom: parent.bottom
+                    color: "transparent"
+
+                    Label {
+                        id: precipitation
+                        width: parent.width
+                        height: parent.height
+                        horizontalAlignment: precipitationIcon.AlignLeft
+                        verticalAlignment: Text.AlignVCenter
+                        font.weight: Font.Bold
+                        font.pixelSize: parent.width > parent.height ? height * 0.75 : width * 0.75
+                        rightPadding: -font.pixelSize * 0.1
+                        color: dayNightTime == "day" ? "black" : "white"
+                        text: sessionData.chanceOfPrecipitation + "%"
+                    }
+                }
             }
         }
 
         Kirigami.Separator {
             id: sept1
             width: 1
             height: parent.height * 0.60
```

## skill_ovos_weather/ui/SunriseSunset.qml

```diff
@@ -7,88 +7,76 @@
 
 WeatherDelegate {
     id: root
 
     GridLayout {
         id: sunriseSunset
         anchors.top: parent.top
-        anchors.topMargin: root.locBoxHeight
+        anchors.topMargin: parent.parent.locBoxHeight
         anchors.bottom: parent.bottom
+        rows: 2
+        columns: 1
+        rowSpacing: 0
         width: parent.width
-        columns: 2
-        columnSpacing: Mycroft.Units.gridUnit * 2
 
-        ColumnLayout {
+        RowLayout {
             id: sunrise
-            Layout.fillWidth: true
-            Layout.fillHeight: true
-            spacing: Mycroft.Units.gridUnit
-
-            Image {
-                Layout.preferredWidth: width
-                Layout.preferredHeight: width
+
+            Rectangle {
+                id: sunriseBackground
+                color: "transparent"
+                Layout.preferredWidth: sunriseSunset.width * 0.15
+                Layout.preferredHeight: sunriseSunset.width * 0.15
+                Layout.leftMargin: sunriseSunset.width * 0.15
                 Layout.alignment: Qt.AlignHCenter | Qt.AlignVCenter
-                id: sunriseImage
-                source: "images/sunrise.svg"
+
+                Image {
+                    id: sunriseImage
+                    source: "images/sunrise.svg"
+                    anchors.fill: parent
+                }
             }
 
             Label {
                 id: sunriseTime
                 Layout.fillWidth: true
                 horizontalAlignment: Text.AlignHCenter
+                verticalAlignment: Text.AlignVCenter
                 font.weight: Font.Bold
-                font.pixelSize: width * 0.3
+                font.pixelSize: sunriseSunset.width * 0.1
                 color: dayNightTime == "day" ? "black" : "white"
                 text: sessionData.sunrise
             }
-
-            Label {
-                id: sunriseAm
-                Layout.fillWidth: true
-                horizontalAlignment: Text.AlignHCenter
-                font.styleName: "Thin"
-                font.pixelSize: width * 0.25
-                visible: sessionData.ampm
-                enabled: sessionData.ampm
-                color: dayNightTime == "day" ? "black" : "white"
-                text: sessionData.ampm ? "AM" : ""
-            }
         }
 
-        ColumnLayout {
+        RowLayout {
             id: sunset
-            Layout.fillWidth: true
-            Layout.fillHeight: true
-            spacing: Mycroft.Units.gridUnit
-
-            Image {
-                Layout.preferredWidth: width
-                Layout.preferredHeight: width
+
+            Rectangle {
+                id: sunsetBackground
+                color: "transparent"
+                Layout.preferredWidth: sunriseSunset.width * 0.15
+                Layout.preferredHeight: sunriseSunset.width * 0.15
+                Layout.leftMargin: sunriseSunset.width * 0.15
                 Layout.alignment: Qt.AlignHCenter | Qt.AlignVCenter
-                id: sunsetImage
-                source: "images/sunset.svg"
+
+                Image {
+                    id: sunsetImage
+                    source: "images/sunset.svg"
+                    anchors.fill: parent
+                }
             }
 
             Label {
                 id: sunsetTime
+                // Layout.fillWidth: true
                 Layout.fillWidth: true
                 horizontalAlignment: Text.AlignHCenter
+                verticalAlignment: Text.AlignVCenter
                 font.weight: Font.Bold
-                font.pixelSize: width * 0.3
+                font.pixelSize: sunriseSunset.width * 0.1
                 color: dayNightTime == "day" ? "black" : "white"
                 text: sessionData.sunset
             }
-
-            Label {
-                id: sunsetPm
-                Layout.fillWidth: true
-                horizontalAlignment: Text.AlignHCenter
-                font.styleName: "Thin"
-                font.pixelSize: width * 0.25
-                visible: sessionData.ampm
-                enabled: sessionData.ampm
-                color: dayNightTime == "day" ? "black" : "white"
-                text: sessionData.ampm ? "PM" : ""
-            }
         }
     }
 }
```

## skill_ovos_weather/ui/images/rain.svg

```diff
@@ -151,15 +151,15 @@
 00000960: 3034 2e34 3943 3236 2e31 3133 3220 3330  04.49C26.1132 30
 00000970: 382e 3335 3720 3236 2e31 3133 3220 3331  8.357 26.1132 31
 00000980: 312e 3934 3820 3237 2e32 3138 3120 3331  1.948 27.2181 31
 00000990: 352e 3831 3543 3238 2e31 3834 3820 3331  5.815C28.1848 31
 000009a0: 392e 3534 3420 3330 2e31 3138 3320 3332  9.544 30.1183 32
 000009b0: 322e 3835 3820 3332 2e38 3830 3520 3332  2.858 32.8805 32
 000009c0: 352e 3632 315a 2220 6669 6c6c 3d22 2332  5.621Z" fill="#2
-000009d0: 3241 3746 3022 2f3e 0a3c 7061 7468 2064  2A7F0"/>.<path d
+000009d0: 3636 3639 3122 2f3e 0a3c 7061 7468 2064  66691"/>.<path d
 000009e0: 3d22 4d31 3935 2e37 3139 2032 3730 2e37  ="M195.719 270.7
 000009f0: 3932 4331 3932 2e34 3035 2032 3736 2e38  92C192.405 276.8
 00000a00: 3639 2031 3839 2e37 3820 3238 332e 3038  69 189.78 283.08
 00000a10: 3420 3138 382e 3132 3320 3238 392e 3731  4 188.123 289.71
 00000a20: 3343 3138 372e 3031 3820 3239 332e 3538  3C187.018 293.58
 00000a30: 2031 3835 2e37 3735 2032 3938 2e39 3636   185.775 298.966
 00000a40: 2031 3834 2e35 3332 2033 3036 2e30 3039   184.532 306.009
@@ -243,15 +243,15 @@
 00000f20: 2e32 3138 2033 3034 2e34 3943 3132 362e  .218 304.49C126.
 00000f30: 3131 3320 3330 382e 3335 3720 3132 362e  113 308.357 126.
 00000f40: 3131 3320 3331 312e 3934 3820 3132 372e  113 311.948 127.
 00000f50: 3231 3820 3331 352e 3831 3543 3132 382e  218 315.815C128.
 00000f60: 3138 3520 3331 392e 3534 3420 3133 302e  185 319.544 130.
 00000f70: 3131 3820 3332 322e 3835 3820 3133 322e  118 322.858 132.
 00000f80: 3838 2033 3235 2e36 3231 5a22 2066 696c  88 325.621Z" fil
-00000f90: 6c3d 2223 3232 4137 4630 222f 3e0a 3c70  l="#22A7F0"/>.<p
+00000f90: 6c3d 2223 3236 3636 3931 222f 3e0a 3c70  l="#266691"/>.<p
 00000fa0: 6174 6820 643d 224d 3239 352e 3731 3920  ath d="M295.719 
 00000fb0: 3237 302e 3739 3243 3239 322e 3430 3420  270.792C292.404 
 00000fc0: 3237 362e 3836 3920 3238 392e 3738 2032  276.869 289.78 2
 00000fd0: 3833 2e30 3834 2032 3838 2e31 3233 2032  83.084 288.123 2
 00000fe0: 3839 2e37 3133 4332 3837 2e30 3138 2032  89.713C287.018 2
 00000ff0: 3933 2e35 3820 3238 352e 3737 3520 3239  93.58 285.775 29
 00001000: 382e 3936 3620 3238 342e 3533 3220 3330  8.966 284.532 30
@@ -335,9 +335,9 @@
 000014e0: 2032 3237 2e32 3138 2033 3034 2e34 3943   227.218 304.49C
 000014f0: 3232 362e 3131 3320 3330 382e 3335 3720  226.113 308.357 
 00001500: 3232 362e 3131 3320 3331 312e 3934 3820  226.113 311.948 
 00001510: 3232 372e 3231 3820 3331 352e 3831 3543  227.218 315.815C
 00001520: 3232 382e 3138 3520 3331 392e 3534 3420  228.185 319.544 
 00001530: 3233 302e 3131 3820 3332 322e 3835 3820  230.118 322.858 
 00001540: 3233 322e 3838 2033 3235 2e36 3231 5a22  232.88 325.621Z"
-00001550: 2066 696c 6c3d 2223 3232 4137 4630 222f   fill="#22A7F0"/
+00001550: 2066 696c 6c3d 2223 3236 3636 3931 222f   fill="#266691"/
 00001560: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
```

## skill_ovos_weather/weather_helpers/config.py

```diff
@@ -14,19 +14,19 @@
 """Parse the device configuration and skill settings to determine the """
 from ovos_config import Configuration
 
 FAHRENHEIT = "fahrenheit"
 CELSIUS = "celsius"
 METRIC = "metric"
 IMPERIAL = "imperial"
-METERS_PER_SECOND = "meters per second"
-KILOMETERS_PER_HOUR = "kilometers per hour"
+METER_PER_SECOND = "meter per second"
+KILOMETER_PER_HOUR = "kilometer per hour"
 MILES_PER_HOUR = "miles per hour"
 INCH = "inch"
-MILLIMETERS = "millimeters"
+MILLIMETER = "millimeter"
 
 
 class WeatherConfig:
     """Build an object representing the configuration values for the weather skill."""
 
     def __init__(self, core_config: dict = None, settings: dict = None):
         self.core_config = core_config or Configuration()
@@ -82,15 +82,15 @@
     @property
     def speed_unit(self) -> str:
         """Use the core configuration to determine the unit of speed.
 
         Returns: (str) 'meters_sec' or 'mph'
         """
         if self.scale == METRIC:
-            return METERS_PER_SECOND
+            return METER_PER_SECOND
         else:
             return MILES_PER_HOUR
 
     @property
     def temperature_unit(self) -> str:
         """Use the core configuration to determine the unit of temperature.
 
@@ -102,10 +102,10 @@
 
     @property
     def precipitation_unit(self) -> str:
         """Use the core configuration to determine the unit of precipitation.
 
         Returns: "millimeters" or "inch"""
         if self.scale == METRIC:
-            return MILLIMETERS
+            return MILLIMETER
         else:
             return INCH
```

## skill_ovos_weather/weather_helpers/dialog.py

```diff
@@ -29,20 +29,21 @@
         example, temperature can be qualified by "high" or "low".
     * Locale: indicates if the dialog is for local weather or weather in a remote
         location.
 
 The skill class will use the "name" and "data" attributes to pass to the TTS process.
 """
 # TODO - get rid of relative imports as soon as skills can be properly packaged with arbitrary module structures
-from typing import List, Tuple
+from typing import List
+from os.path import dirname
 
-from lingua_franca.format import join_list, nice_number, nice_time
+from lingua_franca.format import join_list, nice_time
 from ovos_utils.time import now_local
+from ovos_workshop.resource_files import SkillResources
 
-from .config import WeatherConfig
 from .intent import WeatherIntent
 from .util import get_speakable_day_of_week, get_time_period
 from .weather import (
     CURRENT,
     DAILY,
     HOURLY,
     Weather,
@@ -59,26 +60,28 @@
 class WeatherDialog:
     """Abstract base class for the weather dialog builders."""
 
     def __init__(self, intent_data: WeatherIntent):
         self.intent_data = intent_data
         self.name = None
         self.data = None
+        self.resources = SkillResources(dirname(dirname(__file__)),
+                                        self.lang)
 
     @property
     def config(self):
         return self.intent_data.config
 
     @property
     def lang(self):
         return self.config.lang
 
-    @property
-    def temperature_unit(self):
-        return self.config.temperature_unit
+    def translate(self, dialog, data=None):
+        data = data or dict()
+        return self.resources.render_dialog(dialog, data=data)   
 
     def _add_location(self):
         """Add location information to the dialog."""
         if self.intent_data.location is None:
             self.name += "-local"
         else:
             self.name += "-location"
@@ -107,28 +110,20 @@
         self.weather = weather
         self.name = CURRENT
 
     def build_weather_dialog(self):
         """Build the components necessary to speak current weather."""
         self.name += "-weather"
         self.data = dict(
-            condition=self.weather.condition.description,
+            condition=self.translate(self.weather.condition.description),
             temperature=self.weather.temperature,
-            temperature_unit=self.temperature_unit,
+            temperature_unit=self.translate(self.config.temperature_unit),
         )
         self._add_location()
 
-    def build_high_low_temperature_dialog(self):
-        """Build the components necessary to speak high and low temperature."""
-        self.name += "-temperature-high-low"
-        self.data = dict(
-            high_temperature=self.weather.temperature_high,
-            low_temperature=self.weather.temperature_low,
-        )
-
     def build_temperature_dialog(self, temperature_type: str):
         """Build the components necessary to speak the current temperature.
 
         :param temperature_type: indicates if temperature is current, high or low
         """
         self.name += "-temperature"
         if temperature_type == "high":
@@ -136,29 +131,32 @@
             self.data = dict(temperature=self.weather.temperature_high)
         elif temperature_type == "low":
             self.name += "-low"
             self.data = dict(temperature=self.weather.temperature_low)
         else:
             self.data = dict(temperature=self.weather.temperature)
         self.data.update(
-            temperature_unit=self.temperature_unit
+            temperature_unit=self.translate(self.config.temperature_unit)
         )
         self._add_location()
 
     def build_condition_dialog(self, intent_match: bool):
         """Select the relevant dialog file for condition based reports.
 
         A condition can for example be "snow" or "rain".
 
         :param intent_match: true if intent matches a vocabulary for the condition
         """
-        self.data = dict(condition=self.weather.condition.description.lower())
+        self.data = dict(condition=self.translate(
+            self.weather.condition.description)
+        )
         if intent_match:
             self.name += "-condition-expected"
         else:
+            # TODO nothing to format
             self.name += "-condition-not-expected".format(
                 self.weather.condition.category.lower()
             )
         self._add_location()
 
     def build_sunrise_dialog(self):
         """Build the components necessary to speak the sunrise time."""
@@ -186,99 +184,104 @@
         self.data = dict(time=nice_time(self.weather.sunset, lang=self.lang))
         self._add_location()
 
     def build_wind_dialog(self):
         """Build the components necessary to speak the wind conditions."""
         wind_strength = self.weather.determine_wind_strength(self.config.speed_unit)
         self.data = dict(
-            speed=nice_number(self.weather.wind_speed, lang=self.lang),
-            speed_unit=self.config.speed_unit,
-            direction=self.weather.wind_direction,
+            speed=self.weather.wind_speed,
+            speed_unit=self.translate(self.config.speed_unit),
+            direction=self.translate(self.weather.wind_direction.lower()),
         )
         self.name += "-wind-" + wind_strength
         self._add_location()
 
     def build_humidity_dialog(self):
         """Build the components necessary to speak the percentage humidity."""
-        self.data = dict(percent=self.weather.humidity)
+        self.data = dict(
+            percent=self.translate("percentage-number",
+                                   {"number": self.weather.humidity})
+        )
         self.name += "-humidity"
         self._add_location()
 
 
 class HourlyDialog(WeatherDialog):
     """Weather dialog builder for hourly weather."""
 
     def __init__(self, intent_data: WeatherIntent, weather: Weather):
         super().__init__(intent_data)
         self.weather = weather
         self.name = HOURLY
-
+    
     def build_weather_dialog(self):
         """Build the components necessary to speak the forecast for a hour."""
         self.name += "-weather"
         self.data = dict(
-            condition=self.weather.condition.description,
-            time=self.weather.date_time.strftime("%H:00"),
+            condition=self.translate(self.weather.condition.description),
+            time=nice_time(self.weather.date_time, lang=self.lang),
             temperature=self.weather.temperature,
         )
         self._add_location()
 
-    def build_temperature_dialog(self, _):
+    def build_temperature_dialog(self, _ = None):
         """Build the components necessary to speak the hourly temperature."""
         self.name += "-temperature"
         self.data = dict(
             temperature=self.weather.temperature,
-            time=get_time_period(self.weather.date_time),
-            temperature_unit=self.temperature_unit,
+            time=self.translate(get_time_period(self.weather.date_time)),
+            temperature_unit=self.translate(self.config.temperature_unit),
         )
         self._add_location()
 
     def build_condition_dialog(self, intent_match: bool):
         """Select the relevant dialog file for condition based reports.
 
         A condition can for example be "snow" or "rain".
 
         :param intent_match: true if intent matches a vocabulary for the condition
         """
         self.data = dict(
-            condition=self.weather.condition.description.lower(),
+            condition=self.translate(self.weather.condition.description),
             time=nice_time(self.weather.date_time, lang=self.lang),
         )
         if intent_match:
             self.name += "-condition-expected"
         else:
+            # TODO nothing to format
             self.name += "-condition-not-expected".format(
                 self.weather.condition.category.lower()
             )
         self._add_location()
 
     def build_wind_dialog(self):
         """Build the components necessary to speak the wind conditions."""
         wind_strength = self.weather.determine_wind_strength(self.config.speed_unit)
         self.data = dict(
-            speed=nice_number(self.weather.wind_speed, lang=self.lang),
-            speed_unit=self.config.speed_unit,
-            direction=self.weather.wind_direction,
+            speed=self.weather.wind_speed,
+            speed_unit=self.translate(self.config.speed_unit),
+            direction=self.translate(self.weather.wind_direction.lower()),
             time=nice_time(self.weather.date_time, lang=self.lang),
         )
         self.name += "-wind-" + wind_strength
         self._add_location()
 
     def build_next_precipitation_dialog(self):
         """Build the components necessary to speak the next chance of rain."""
         if self.weather is None:
             self.name += "-precipitation-next-none"
             self.data = dict()
         else:
             self.name += "-precipitation-next"
             self.data = dict(
-                percent=self.weather.chance_of_precipitation,
-                precipitation="rain",
+                percent=self.translate("percentage-number",
+                                       {"number": self.weather.chance_of_precipitation}),
+                precipitation=self.translate(self.weather.condition.description),
                 day=get_speakable_day_of_week(self.weather.date_time, self.lang),
-                time=get_time_period(self.weather.date_time),
+                time=self.translate(get_time_period(self.weather.date_time)),
             )
         self._add_location()
 
 
 class DailyDialog(WeatherDialog):
     """Weather dialog builder for daily weather."""
 
@@ -287,55 +290,58 @@
         self.weather = weather
         self.name = DAILY
 
     def build_weather_dialog(self):
         """Build the components necessary to speak the forecast for a day."""
         self.name += "-weather"
         self.data = dict(
-            condition=self.weather.condition.description,
+            condition=self.translate(self.weather.condition.description),
             day=get_speakable_day_of_week(self.weather.date_time, self.lang),
             high_temperature=self.weather.temperature_high,
             low_temperature=self.weather.temperature_low,
         )
         self._add_location()
 
-    def build_temperature_dialog(self, temperature_type: str):
+    def build_temperature_dialog(self, temperature_type: str = "both"):
         """Build the components necessary to speak the daily temperature.
 
         :param temperature_type: indicates if temperature is day, high or low
         """
         self.name += "-temperature"
         if temperature_type == "high":
             self.name += "-high"
             self.data = dict(temperature=self.weather.temperature_high)
         elif temperature_type == "low":
             self.name += "-low"
             self.data = dict(temperature=self.weather.temperature_low)
         else:
-            self.data = dict(temperature=self.weather.temperature)
+            self.name += "-high-low"
+            self.data = dict(high_temperature=self.weather.temperature_high,
+                             low_temperature=self.weather.temperature_low)
         self.data.update(
             day=get_speakable_day_of_week(self.weather.date_time, self.lang),
-            temperature_unit=self.temperature_unit,
+            temperature_unit=self.translate(self.config.temperature_unit),
         )
         self._add_location()
 
     def build_condition_dialog(self, intent_match: bool):
         """Select the relevant dialog file for condition based reports.
 
         A condition can for example be "snow" or "rain".
 
         :param intent_match: true if intent matches a vocabulary for the condition
         """
         self.data = dict(
-            condition=self.weather.condition.description.lower(),
+            condition=self.translate(self.weather.condition.description),
             day=get_speakable_day_of_week(self.weather.date_time, self.lang),
         )
         if intent_match:
             self.name += "-condition-expected"
         else:
+            # TODO nothing to format
             self.name += "-condition-not-expected".format(
                 self.weather.condition.category.lower()
             )
         self._add_location()
 
     def build_sunrise_dialog(self):
         """Build the components necessary to speak the sunrise time."""
@@ -352,40 +358,42 @@
         self._add_location()
 
     def build_wind_dialog(self):
         """Build the components necessary to speak the wind conditions."""
         wind_strength = self.weather.determine_wind_strength(self.config.speed_unit)
         self.data = dict(
             day=get_speakable_day_of_week(self.weather.date_time, self.lang),
-            speed=nice_number(self.weather.wind_speed, lang=self.lang),
-            speed_unit=self.config.speed_unit,
-            direction=self.weather.wind_direction,
+            speed=self.weather.wind_speed_max,
+            speed_unit=self.translate(self.config.speed_unit),
+            direction=self.translate(self.weather.wind_direction.lower()),
         )
         self.name += "-wind-" + wind_strength
         self._add_location()
 
     def build_humidity_dialog(self):
         """Build the components necessary to speak the percentage humidity."""
         self.data = dict(
-            percent=self.weather.humidity,
+            percent=self.translate("percentage-number",
+                                   {"number": self.weather.humidity}),
             day=get_speakable_day_of_week(self.weather.date_time, self.lang)
         )
         self.name += "-humidity"
         self._add_location()
 
     def build_next_precipitation_dialog(self):
         """Build the components necessary to speak the next chance of rain."""
         if self.weather is None:
             self.name += "-precipitation-next-none"
             self.data = dict()
         else:
             self.name += "-precipitation-next"
             self.data = dict(
-                percent=self.weather.chance_of_precipitation,
-                precipitation="rain",
+                percent=self.translate("percentage-number",
+                                       {"number": self.weather.chance_of_precipitation}),
+                precipitation=self.translate(self.weather.condition.description),
                 day=get_speakable_day_of_week(self.weather.date_time, self.lang),
             )
         self._add_location()
 
 
 class WeeklyDialog(WeatherDialog):
     """Weather dialog builder for weekly weather."""
@@ -410,15 +418,15 @@
             high_min=min(high_temperatures),
             high_max=max(high_temperatures),
         )
 
     def build_condition_dialog(self, condition: str):
         """Build the components necessary to speak the days of week for a condition."""
         self.name += "-condition"
-        self.data = dict(condition=condition)
+        self.data = dict(condition=self.translate(condition))
         days_with_condition = []
         for daily in self.forecast:
             if daily.condition.category == condition:
                 day = get_speakable_day_of_week(daily.date_time, lang=self.lang)
                 days_with_condition.append(day)
         self.data.update(days=join_list(days_with_condition, "and"))
```

## skill_ovos_weather/weather_helpers/intent.py

```diff
@@ -13,20 +13,20 @@
 # limitations under the License.
 """Parse the intent into data used by the weather skill."""
 # TODO - get rid of relative imports as soon as skills can be properly packaged with arbitrary module structures
 
 from datetime import timedelta
 
 from ovos_utils.time import now_local
+from lingua_franca.parse import normalize
 
 from .util import (
     get_utterance_datetime,
     get_geolocation,
-    get_tz_info,
-    LocationNotFoundError,
+    get_tz_info
 )
 from .weather import CURRENT
 from .config import WeatherConfig
 
 
 class WeatherIntent:
     _geolocation = None
@@ -35,15 +35,17 @@
 
     def __init__(self, message, weather_config: WeatherConfig):
         """Constructor
 
         :param message: Intent data from the message bus
         :param language: The configured language of the device
         """
-        self.utterance = message.data["utterance"]
+        self.utterance = normalize(message.data["utterance"],
+                                   weather_config.lang,
+                                   remove_articles=False)
         self.location = message.data.get("location")
         self.config = weather_config
         self.scale = None
         self.timeframe = CURRENT
 
     @property
     def latitude(self):
```

## skill_ovos_weather/weather_helpers/openmeteo.py

```diff
@@ -4,37 +4,65 @@
 # TODO - get rid of relative imports
 # /home/miro/PycharmProjects/.venvs/ovos/bin/python /home/miro/PycharmProjects/skill-ovos-weather/weather_helpers/openmeteo.py
 # Traceback (most recent call last):
 #   File "/home/miro/PycharmProjects/skill-ovos-weather/weather_helpers/openmeteo.py", line 3, in <module>
 #     from .config import *
 # ImportError: attempted relative import with no known parent package
 # so annoying
+from datetime import datetime as dt
+
+from .util import chunk_list
 from .config import *
 from .weather import WeatherReport
 
+def sliced(data: dict) -> dict:
+    """
+    Openmeteo is sending data starting at 00:00 local-time,
+    This slices the hourly data up until the current hour.
+
+    Args:
+        data (dict): the weather json report sent from om
+
+    Returns:
+        dict: the sliced report
+    """
+    time = data.get("current_weather",{}).get("time")
+    hour = dt.fromisoformat(time).hour
+
+    for k, v in data["hourly"].items():
+        # compute missing/nice to have daily parameters
+        if k == "relativehumidity_2m":
+            data["daily"][k] = [int(sum(tup)/len(tup)) for tup
+                                in chunk_list(v, 24)]
+        # slice data
+        if isinstance(v, list):
+            data["hourly"][k] = v[hour:]
+
+    return data
+
 
 @timed_lru_cache(seconds=60 * 15)  # cache for 15 mins
 def get_report(cfg: WeatherConfig):
     if cfg.speed_unit == MILES_PER_HOUR:
         windspeed_unit = "mph"
-    elif cfg.speed_unit == METERS_PER_SECOND:
+    elif cfg.speed_unit == METER_PER_SECOND:
         windspeed_unit = "ms"
-    elif cfg.speed_unit == KILOMETERS_PER_HOUR:
+    elif cfg.speed_unit == KILOMETER_PER_HOUR:
         windspeed_unit = "kmh"
     else:
         raise ValueError("invalid speed unit")
 
     if cfg.temperature_unit == CELSIUS:
         temperature_unit = "celsius"
     elif cfg.temperature_unit == FAHRENHEIT:
         temperature_unit = "fahrenheit"
     else:
         raise ValueError("invalid temperature unit")
 
-    if cfg.precipitation_unit == MILLIMETERS:
+    if cfg.precipitation_unit == MILLIMETER:
         precipitation_unit = "mm"
     elif cfg.precipitation_unit == INCH:
         precipitation_unit = "inch"
     else:
         raise ValueError("invalid precipitation unit")
 
     daily_params = [
@@ -111,9 +139,9 @@
         "current_weather": True,
         "temperature_unit": temperature_unit,  # fahrenheit
         "windspeed_unit": windspeed_unit,  # ms, mph, kn
         "precipitation_unit": precipitation_unit,  # inch
         "timezone": cfg.timezone  # gmt ...
     }
     url = f"https://api.open-meteo.com/v1/forecast"
-    data = requests.get(url, params=args).json()
+    data = sliced(requests.get(url, params=args).json())
     return WeatherReport(data)
```

## skill_ovos_weather/weather_helpers/util.py

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utility functions for the weather skill."""
 from datetime import datetime, timedelta, tzinfo
+from typing import List
+from itertools import islice
 
 import pytz
 from lingua_franca.format import nice_date
 from lingua_franca.parse import extract_datetime
 from ovos_backend_client.api import GeolocationApi
 from ovos_utils.time import now_local, to_local
 
@@ -62,15 +64,14 @@
         anchor_date = None
     else:
         intent_timezone = get_tz_info(timezone)
         anchor_date = datetime.now(intent_timezone)
     extract = extract_datetime(utterance, anchor_date, language)
     if extract is not None:
         utterance_datetime, _ = extract
-
     return utterance_datetime
 
 
 def get_tz_info(timezone: str) -> tzinfo:
     """Generate a tzinfo object from a timezone string.
 
     Args:
@@ -104,15 +105,15 @@
     # convert the dict to a simpler format
     return {
         "city": geolocation["city"]["name"],
         "region": geolocation["city"]["state"]["name"],
         "country":  geolocation["city"]["state"]["country"]["name"],
         "latitude": geolocation["coordinate"]["latitude"],
         "longitude": geolocation["coordinate"]["longitude"],
-        "timezone": geolocation["timezone"]["name"]
+        "timezone": geolocation["timezone"]["code"]
     }
 
 
 def get_time_period(intent_datetime: datetime) -> str:
     """Translate a specific time '9am' to period of the day 'morning'
 
     Args:
@@ -153,7 +154,21 @@
     else:
         now_arg = now
 
     speakable_date = nice_date(date_to_speak, now=now_arg, lang=lang)
     day_of_week = speakable_date.split(",")[0]
 
     return day_of_week
+
+
+def chunk_list(it: list, size: int) -> List[tuple]:
+    """Takes in a list and chops it in `size` length tuples
+
+    Args:
+        it (list): list to chop
+        size (int): size of the chunks
+
+    Returns:
+        List[tuple]: a list of tuple containing the chunks
+    """
+    it = iter(it)
+    return list(iter(lambda: tuple(islice(it, size)), ()))
```

## skill_ovos_weather/weather_helpers/weather.py

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Representations and conversions of the data returned by the weather API."""
 from datetime import timedelta
 from pathlib import Path
-from typing import List
+from typing import List, Tuple
 
 # TODO - get rid of relative imports as soon as skills can be properly packaged with arbitrary module structures
 from .config import MILES_PER_HOUR
 from .util import convert_to_local_datetime
 
 # Forecast timeframes
 CURRENT = "current"
@@ -165,69 +165,69 @@
             self.category = "thunderstorm"
             if is_day:
                 self.icon = "11d"
             else:
                 self.icon = "11n"
 
         if weather_code == 0:
-            self.description = "clear sky"
+            self.description = "clear-sky"
         elif weather_code == 1:
-            self.description = "mainly clear"
+            self.description = "mainly-clear"
         elif weather_code == 2:
-            self.description = "partly cloudy"
+            self.description = "partly-cloudy"
         elif weather_code == 3:
             self.description = "overcast"
         elif weather_code == 45:
             self.description = "fog"
         elif weather_code == 48:
-            self.description = "depositing rime fog"
+            self.description = "depositing-rime-fog"
         elif weather_code == 51:
-            self.description = "Drizzle, light intensity"
+            self.description = "drizzle-light-intensity"
         elif weather_code == 53:
-            self.description = "Drizzle, moderate intensity"
+            self.description = "drizzle-moderate-intensity"
         elif weather_code == 55:
-            self.description = "Drizzle, dense intensity"
+            self.description = "drizzle-dense-intensity"
         elif weather_code == 56:
-            self.description = "Freezing Drizzle, light intensity"
+            self.description = "freezing-drizzle-light-intensity"
         elif weather_code == 57:
-            self.description = "Freezing Drizzle, dense intensity"
+            self.description = "freezing-drizzle-dense-intensity"
         elif weather_code == 61:
-            self.description = "Slight Rain"
+            self.description = "slight-rain"
         elif weather_code == 63:
-            self.description = "Moderate Rain"
+            self.description = "moderate-rain"
         elif weather_code == 65:
-            self.description = "Heavy Rain"
+            self.description = "heavy-rain"
         elif weather_code == 66:
-            self.description = "Freezing Rain, light intensity"
+            self.description = "freezing-rain-light-intensity"
         elif weather_code == 67:
-            self.description = "Freezing Rain, dense intensity"
+            self.description = "freezing-rain-dense-intensity"
         elif weather_code == 71:
-            self.description = "Slight Snow fall"
+            self.description = "slight-snow-fall"
         elif weather_code == 73:
-            self.description = "Moderate Snow fall"
+            self.description = "moderate-snow-fall"
         elif weather_code == 75:
-            self.description = "Heavy Snow fall"
+            self.description = "heavy-snow-fall"
         elif weather_code == 77:
-            self.description = "Snow grains"
+            self.description = "snow-grains"
         elif weather_code == 80:
-            self.description = "Slight Rain showers"
+            self.description = "slight-rain-showers"
         elif weather_code == 81:
-            self.description = "Moderate Rain showers"
+            self.description = "moderate-rain-showers"
         elif weather_code == 82:
-            self.description = "Violent Rain showers"
+            self.description = "violent-rain-showers"
         elif weather_code == 85:
-            self.description = "Slight Snow showers"
+            self.description = "slight-snow-showers"
         elif weather_code == 86:
-            self.description = "Heavy Snow showers"
+            self.description = "heavy-snow-showers"
         elif weather_code == 95:
-            self.description = "Thunderstorm"
+            self.description = "thunderstorm"
         elif weather_code == 96:
-            self.description = "Thunderstorm with slight hail"
+            self.description = "thunderstorm-with-slight-hail"
         elif weather_code == 99:
-            self.description = "Thunderstorm with heavy hail"
+            self.description = "thunderstorm-with-heavy-hail"
         self.id = weather_code
 
     @property
     def image(self) -> str:
         """Use the icon to image mapping to determine which image to display."""
         image_path = Path("images")
         for icons, image_file_name in ICON_IMAGE_MAP:
@@ -272,31 +272,35 @@
         # TODO - handle any missing data that we can derive
         self.pressure = weather.get("surface_pressure")
         self.humidity = weather.get("relativehumidity_2m") or \
                         weather.get("relativehumidity_1000hPa")
         self.dew_point = weather.get("dewpoint_2m")
         self.clouds = weather.get("cloudcover")
         self.wind_speed = weather.get("windspeed_10m")
-        self.wind_direction = weather.get("winddirection_10m")
+        self.wind_speed_max = weather.get("windspeed_10m_max") or self.wind_speed
+        self.wind_direction = weather.get("winddirection_10m") or weather.get("winddirection_10m_dominant")
         if self.wind_direction:
             self.wind_direction = self._determine_wind_direction(self.wind_direction)
         self.sunrise = weather.get("sunrise")
         if self.sunrise and isinstance(self.sunrise, str):
             self.sunrise = convert_to_local_datetime(self.sunrise, timezone)
         self.sunset = weather.get("sunset")
         if self.sunset and isinstance(self.sunset, str):
             self.sunset = convert_to_local_datetime(self.sunset, timezone)
-        self.temperature = weather.get("temperature")
+        self.temperature = weather.get("temperature_2m")
         self.visibility = weather.get("visibility")
         self.temperature_low = weather.get("temperature_2m_min") or self.temperature
         self.temperature_high = weather.get("temperature_2m_max") or self.temperature
         self.chance_of_precipitation = weather.get("precipitation_probability_mean") or \
                                        weather.get("precipitation_probability_max") or \
                                        weather.get("precipitation_probability_min") or \
                                        weather.get("precipitation_probability") or 0
+        self.precipitation = weather.get("precipitation_sum") or weather.get("precipitation")
+        self.uvindex = weather.get("uv_index_max") or \
+                int(weather.get("shortwave_radiation") * 3.6 / 27.8 )
         self.condition = WeatherCondition(weather["weathercode"])
 
     @staticmethod
     def _determine_wind_direction(degree_direction: int):
         """Convert wind direction from compass degrees to compass direction.
 
         Args:
@@ -323,89 +327,76 @@
         Returns:
             a string representation of the wind strength
         """
         if speed_unit == MILES_PER_HOUR:
             limits = dict(strong=20, moderate=11)
         else:
             limits = dict(strong=9, moderate=5)
-        if self.wind_speed >= limits["strong"]:
+
+        speed = self.wind_speed or self.wind_speed_max
+        if speed >= limits["strong"]:
             wind_strength = "strong"
-        elif self.wind_speed >= limits["moderate"]:
+        elif speed >= limits["moderate"]:
             wind_strength = "moderate"
         else:
             wind_strength = "light"
 
         return wind_strength
 
 
 class WeatherReport:
     """Full representation of the data returned by the OpenMeteo API"""
 
     def __init__(self, report):
         timezone = report["timezone"]
-        curr = report["current_weather"]
-        for k, v in report["daily"].items():
-            if isinstance(v, list):
-                curr[k] = v[0]
-        for k, v in report["hourly"].items():
-            if isinstance(v, list):
-                curr[k] = v[0]
-        self.current = Weather(curr, timezone, report["hourly_units"])
-
         self.hourly = []
         for idx, _ in enumerate(report["hourly"]["time"]):
             r = {k: hour[idx] for k, hour in report["hourly"].items()}
-            # fill missing data with current weather
-            for k, v in self.current.__dict__.items():
-                if k not in r:
-                    r[k] = v
             # ['time', 'temperature_2m', 'relativehumidity_2m', 'dewpoint_2m', 'apparent_temperature',
             # 'pressure_msl', 'surface_pressure', 'cloudcover', 'cloudcover_low', 'cloudcover_mid',
             # 'cloudcover_high', 'windspeed_10m', 'windspeed_80m', 'windspeed_120m', 'windspeed_180m',
             # 'winddirection_10m', 'winddirection_80m', 'winddirection_120m', 'winddirection_180m',
             # 'windgusts_10m', 'shortwave_radiation', 'direct_radiation', 'diffuse_radiation',
             # 'vapor_pressure_deficit', 'cape', 'evapotranspiration', 'et0_fao_evapotranspiration',
             # 'precipitation', 'weathercode', 'snow_depth', 'showers', 'snowfall', 'visibility',
             # 'precipitation_probability', 'freezinglevel_height', 'soil_temperature_0cm',
             # 'soil_temperature_6cm', 'soil_temperature_18cm', 'soil_temperature_54cm',
             # 'soil_moisture_0_1cm', 'soil_moisture_1_3cm', 'soil_moisture_3_9cm', 'soil_moisture_9_27cm',
             # 'soil_moisture_27_81cm', 'is_day']
             self.hourly.append(Weather(r, timezone, report["hourly_units"]))
+        
+        self.current = self.hourly[0]
 
         self.daily = []
         for idx, _ in enumerate(report["daily"]["time"]):
             r = {k: hour[idx] for k, hour in report["daily"].items()}
-            if idx == 0:  # fill missing data with current weather for today's prediction
-                for k, v in self.current.__dict__.items():
-                    if k not in r:
-                        r[k] = v
             # ['time', 'temperature_2m_max', 'temperature_2m_min', 'apparent_temperature_max',
             # 'apparent_temperature_min', 'precipitation_sum', 'precipitation_hours', 'weathercode',
             # 'sunrise', 'sunset', 'windspeed_10m_max', 'windgusts_10m_max', 'winddirection_10m_dominant',
             # 'shortwave_radiation_sum', 'et0_fao_evapotranspiration', 'uv_index_max',
             # 'precipitation_probability_mean', 'precipitation_probability_min', 'precipitation_probability_max',
             # 'uv_index_clear_sky_max']
             self.daily.append(Weather(r, timezone, report["daily_units"]))
 
-    def get_weather_for_intent(self, intent_data):
+    def get_weather_for_intent(self, intent_data) -> Weather:
         """Use the intent to determine which forecast satisfies the request.
 
         Args:
             intent_data: Parsed intent data
         """
         if intent_data.timeframe == "hourly":
             weather = self.get_forecast_for_hour(intent_data)
         elif intent_data.timeframe == "daily":
             weather = self.get_forecast_for_date(intent_data)
         else:
             weather = self.current
 
         return weather
 
-    def get_forecast_for_date(self, intent_data):
+    def get_forecast_for_date(self, intent_data) -> Weather:
         """Use the intent to determine which daily forecast(s) satisfies the request.
 
         Args:
             intent_data: Parsed intent data
         """
         if intent_data.intent_datetime.date() == intent_data.location_datetime.date():
             forecast = self.daily[0]
@@ -432,45 +423,62 @@
         if days > 7:
             raise IndexError("Only seven days of forecasted weather available.")
 
         forecast = self.daily[1: days + 1]
 
         return forecast
 
-    def get_forecast_for_hour(self, intent_data):
-        """Use the intent to determine which hourly forecast(s) satisfies the request.
+    def get_forecast_for_hour(self, intent_data) -> Weather:
+        """Use the intent to determine which hourly forecast satisfies the request.
 
         Args:
             intent_data: Parsed intent data
 
         Returns:
             A single hour of forecast data based on the intent data
         """
         delta = intent_data.intent_datetime - intent_data.location_datetime
         hour_delta = int(delta / timedelta(hours=1))
         hour_index = hour_delta + 1
         report = self.hourly[hour_index]
 
         return report
 
-    def get_weekend_forecast(self):
+    def get_forecast_for_multiple_hours(self, intent_data) ->List[Weather]:
+        """Use the intent to determine which hourly forecasts satisfies the request.
+        The hourly up from the requested timeframe are returned
+
+        Args:
+            intent_data: Parsed intent data
+
+        Returns:
+            List of hourly forecasts
+        """
+        delta = intent_data.intent_datetime - intent_data.location_datetime
+        hour_delta = int(delta / timedelta(hours=1))
+        hour_index = hour_delta + 1
+        forecast = self.hourly[hour_index:]
+
+        return forecast 
+
+    def get_weekend_forecast(self) -> List[Weather]:
         """Use the intent to determine which daily forecast(s) satisfies the request.
 
         Returns:
             The Saturday and Sunday forecast from the list of daily forecasts
         """
         forecast = list()
         for forecast_day in self.daily:
             report_date = forecast_day.date_time.date()
             if report_date.weekday() in (SATURDAY, SUNDAY):
                 forecast.append(forecast_day)
 
         return forecast
 
-    def get_next_precipitation(self, intent_data):
+    def get_next_precipitation(self, intent_data) -> Tuple[Weather, str]:
         """Determine when the next chance of precipitation is in the forecast.
 
         Args:
             intent_data: Parsed intent data
 
         Returns:
             The weather report containing the next chance of rain and the timeframe of
```

## Comparing `ovos_skill_weather-0.0.1a8.dist-info/LICENSE` & `ovos_skill_weather-0.0.1a9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_skill_weather-0.0.1a8.dist-info/METADATA` & `ovos_skill_weather-0.0.1a9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ovos-skill-weather
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: ovos skill plugin
 Home-page: https://github.com/OpenVoiceOS/skill-ovos-weather
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos skill plugin
 Platform: UNKNOWN
-Requires-Dist: requests
+Requires-Dist: requests (>=2.31.0)
 Requires-Dist: pytz
 Requires-Dist: ovos-utils (>=0.0.28a4,~=0.0)
 Requires-Dist: ovos-workshop (>=0.0.12a27,~=0.0)
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-cov ; extra == 'test'
 Requires-Dist: pytest-timeout ; extra == 'test'
```


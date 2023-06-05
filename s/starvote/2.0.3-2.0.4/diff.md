# Comparing `tmp/starvote-2.0.3.tar.gz` & `tmp/starvote-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-2.0.3.tar` & `starvote-2.0.4.tar`

### file list

```diff
@@ -1,162 +1,176 @@
--rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.3/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.3/LICENSE
--rw-r--r--   0        0        0    34907 2023-06-03 01:10:41.133110 starvote-2.0.3/README.md
--rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.3/docs/clarifying_star_voting.md
--rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.3/docs/formatting_fractions_in_columns_of_text.txt
--rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.3/example.py
--rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.3/pyproject.toml
--rw-r--r--   0        0        0    89957 2023-06-03 00:56:46.533647 starvote-2.0.3/starvote/__init__.py
--rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.3/starvote/__main__.py
--rw-r--r--   0        0        0     5872 2023-06-03 01:02:33.216747 starvote-2.0.3/starvote/reference.py
--rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.3/test_elections/README.md
--rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
--rw-r--r--   0        0        0     1358 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.starvote
--rw-r--r--   0        0        0     1395 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
--rw-r--r--   0        0        0     1404 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
--rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
--rw-r--r--   0        0        0     1402 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
--rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.3/test_elections/bad_syntax_invalid_method.starvote
--rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_method.txt
--rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.3/test_elections/bad_syntax_invalid_option.starvote
--rw-r--r--   0        0        0     1374 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_option.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.starvote
--rw-r--r--   0        0        0     1376 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.txt
--rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
--rw-r--r--   0        0        0     1335 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.txt
--rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.starvote
--rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.txt
--rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.starvote
--rw-r--r--   0        0        0     1360 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.txt
--rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.starvote
--rw-r--r--   0        0        0     1382 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.txt
--rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.3/test_elections/bad_syntax_malformed_section.starvote
--rw-r--r--   0        0        0     1371 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_malformed_section.txt
--rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.3/test_elections/bad_syntax_no_ballots.starvote
--rw-r--r--   0        0        0     1314 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_ballots.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.3/test_elections/bad_syntax_no_equals.starvote
--rw-r--r--   0        0        0     1346 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_equals.txt
--rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.3/test_elections/bad_syntax_no_method.starvote
--rw-r--r--   0        0        0     1409 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_method.txt
--rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.3/test_elections/bad_syntax_no_section.starvote
--rw-r--r--   0        0        0     1364 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_no_section.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.starvote
--rw-r--r--   0        0        0     1375 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.txt
--rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.starvote
--rw-r--r--   0        0        0     1387 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.3/test_elections/bad_syntax_repeated_option.starvote
--rw-r--r--   0        0        0     1380 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_repeated_option.txt
--rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.3/test_elections/bad_syntax_repeated_section.starvote
--rw-r--r--   0        0        0     1383 2023-06-03 00:24:26.568301 starvote-2.0.3/test_elections/bad_syntax_repeated_section.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
--rw-r--r--   0        0        0     1403 2023-06-03 00:24:26.576301 starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
--rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
--rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
--rw-r--r--   0        0        0     3193 2023-06-03 00:24:26.584301 starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.pdf
--rw-r--r--   0        0        0     1331 2023-06-03 00:24:26.588301 starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
--rw-r--r--   0        0        0     2879 2023-06-03 00:24:26.592301 starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
--rw-r--r--   0        0        0     1596 2023-06-03 00:24:26.612301 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
--rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
--rw-r--r--   0        0        0    12586 2023-06-03 00:24:26.932304 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
--rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
--rw-r--r--   0        0        0    12586 2023-06-03 00:24:27.260307 starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.pdf
--rw-r--r--   0        0        0      814 2023-06-03 00:24:27.264307 starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
--rw-r--r--   0        0        0      799 2023-06-03 00:24:27.264307 starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
--rw-r--r--   0        0        0     1434 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
--rw-r--r--   0        0        0      747 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.3/test_elections/test_election_all_fives_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-03 00:24:27.276307 starvote-2.0.3/test_elections/test_election_all_fives_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.3/test_elections/test_election_all_fives_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_fives_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.3/test_elections/test_election_all_fives_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_fives_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.txt
--rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.3/test_elections/test_election_all_threes_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_rrv.txt
--rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.3/test_elections/test_election_all_threes_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.3/test_elections/test_election_all_threes_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_threes_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.starvote
--rw-r--r--   0        0        0     1077 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.3/test_elections/test_election_all_zeroes_rrv.starvote
--rw-r--r--   0        0        0      481 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.3/test_elections/test_election_all_zeroes_star-pr.starvote
--rw-r--r--   0        0        0      473 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.3/test_elections/test_election_all_zeroes_star.starvote
--rw-r--r--   0        0        0     1027 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_all_zeroes_star.txt
--rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.starvote
--rw-r--r--   0        0        0     3383 2023-06-03 00:24:27.280307 starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.txt
--rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
--rw-r--r--   0        0        0     1606 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
--rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      831 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
--rw-r--r--   0        0        0      965 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
--rw-r--r--   0        0        0      744 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
--rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.starvote
--rw-r--r--   0        0        0      542 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.txt
--rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.starvote
--rw-r--r--   0        0        0     1087 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.txt
--rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.3/test_elections/test_election_extra_candidates_in_permutation.starvote
--rw-r--r--   0        0        0      142 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_extra_candidates_in_permutation.txt
--rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.3/test_elections/test_election_incomplete_permutation.starvote
--rw-r--r--   0        0        0      138 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_incomplete_permutation.txt
--rw-r--r--   0        0        0      132 2023-06-03 00:43:08.954337 starvote-2.0.3/test_elections/test_election_no_output.starvote
--rw-r--r--   0        0        0       17 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_no_output.txt
--rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
--rw-r--r--   0        0        0     1329 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
--rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.3/test_elections/test_election_only_one_candidate_star.starvote
--rw-r--r--   0        0        0      505 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_one_candidate_star.txt
--rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.3/test_elections/test_election_only_two_candidates_bloc_star.starvote
--rw-r--r--   0        0        0      487 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_bloc_star.txt
--rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.starvote
--rw-r--r--   0        0        0      523 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.txt
--rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.starvote
--rw-r--r--   0        0        0      545 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.txt
--rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.3/test_elections/test_election_proportional_star_unbreakable_tie.starvote
--rw-r--r--   0        0        0      480 2023-06-03 00:24:27.284307 starvote-2.0.3/test_elections/test_election_proportional_star_unbreakable_tie.txt
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.html
--rw-r--r--   0        0        0      450 2023-06-03 00:37:52.439507 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.starvote
--rw-r--r--   0        0        0     1150 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
--rw-r--r--   0        0        0     1023 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
--rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0     1788 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
--rw-r--r--   0        0        0     2029 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      938 2023-06-03 00:24:27.288307 starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
--rw-r--r--   0        0        0     1081 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
--rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.starvote
--rw-r--r--   0        0        0     1103 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.txt
--rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.starvote
--rw-r--r--   0        0        0     1030 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.txt
--rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.3/test_elections/test_election_use_only_heading_tiebreaker.starvote
--rw-r--r--   0        0        0      152 2023-06-03 00:24:27.292307 starvote-2.0.3/test_elections/test_election_use_only_heading_tiebreaker.txt
--rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.3/tests/harness.py
--rw-r--r--   0        0        0    36446 2023-06-03 01:08:39.424022 starvote-2.0.3/tests/run_tests.py
--rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.3/tools/is_ok
--rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.3/tools/remake_test_elections_output
--rw-r--r--   0        0        0    35477 1970-01-01 00:00:00.000000 starvote-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.4/LICENSE
+-rw-r--r--   0        0        0    42414 2023-06-05 17:24:51.330751 starvote-2.0.4/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.4/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.4/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.4/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0    99015 2023-06-05 17:42:03.467249 starvote-2.0.4/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.4/starvote/__main__.py
+-rw-r--r--   0        0        0     5872 2023-06-03 01:02:33.216747 starvote-2.0.4/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.4/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1365 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1402 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1411 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1409 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.4/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.4/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1383 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1342 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1338 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1367 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1389 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.4/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1378 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.4/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1321 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.4/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1353 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.4/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1416 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.4/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1382 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1394 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.4/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1387 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.4/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1390 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-05 15:58:25.632403 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-05 15:58:25.644404 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-05 15:58:25.648404 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-05 15:58:25.648404 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-05 15:58:25.668404 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.starvote
+-rw-r--r--   0        0        0    12601 2023-06-05 17:37:55.077204 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt
+-rw-r--r--   0        0        0      170 2023-06-05 16:53:17.023154 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0     7239 2023-06-05 16:54:13.803622 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      135 2023-06-05 16:03:25.302834 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.starvote
+-rw-r--r--   0        0        0    60069 2023-06-05 17:20:24.228552 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-05 15:58:26.312409 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-05 15:58:26.316409 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-05 15:58:26.324409 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.4/test_elections/test_election_all_fives_allocated.starvote
+-rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.4/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      145 2023-06-05 16:03:21.998808 starvote-2.0.4/test_elections/test_election_all_fives_sss.starvote
+-rw-r--r--   0        0        0      491 2023-06-05 17:36:55.760715 starvote-2.0.4/test_elections/test_election_all_fives_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.4/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.4/test_elections/test_election_all_threes_allocated.starvote
+-rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.4/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       92 2023-06-05 16:03:19.338786 starvote-2.0.4/test_elections/test_election_all_threes_sss.starvote
+-rw-r--r--   0        0        0      491 2023-06-05 17:36:48.748658 starvote-2.0.4/test_elections/test_election_all_threes_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.4/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.4/test_elections/test_election_all_zeroes_allocated.starvote
+-rw-r--r--   0        0        0      473 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.4/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      145 2023-06-05 16:03:16.750765 starvote-2.0.4/test_elections/test_election_all_zeroes_sss.starvote
+-rw-r--r--   0        0        0      488 2023-06-05 17:36:35.116545 starvote-2.0.4/test_elections/test_election_all_zeroes_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.4/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0      220 2023-06-05 17:40:04.326268 starvote-2.0.4/test_elections/test_election_all_zeroes_with_tiebreaker_sss.starvote
+-rw-r--r--   0        0        0     1921 2023-06-05 17:40:54.170678 starvote-2.0.4/test_elections/test_election_all_zeroes_with_tiebreaker_sss.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.4/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.4/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-03 00:43:08.954337 starvote-2.0.4/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1336 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.4/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.4/test_elections/test_election_only_two_candidates_allocated.starvote
+-rw-r--r--   0        0        0      547 2023-06-05 16:34:32.017979 starvote-2.0.4/test_elections/test_election_only_two_candidates_allocated.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.4/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      176 2023-06-05 16:03:13.610740 starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.starvote
+-rw-r--r--   0        0        0      556 2023-06-05 17:36:16.484392 starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.4/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-06-03 00:37:52.439507 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.starvote
+-rw-r--r--   0        0        0     2033 2023-06-05 17:25:28.231055 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt
+-rw-r--r--   0        0        0      137 2023-06-05 16:03:10.882717 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.starvote
+-rw-r--r--   0        0        0     2343 2023-06-05 17:23:26.814055 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1103 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.4/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.4/tests/harness.py
+-rw-r--r--   0        0        0    36446 2023-06-03 01:08:39.424022 starvote-2.0.4/tests/run_tests.py
+-rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.4/tools/is_ok
+-rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.4/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    42984 1970-01-01 00:00:00.000000 starvote-2.0.4/PKG-INFO
```

### Comparing `starvote-2.0.3/LICENSE` & `starvote-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/README.md` & `starvote-2.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 # starvote
 
-## A simple STAR Voting tabulator
+## A STAR Voting election tabulator
 
 ## Copyright 2023 by Larry Hastings
 
 [STAR voting](https://www.starvoting.org/) is a
-relatively-new [electoral system](https://en.wikipedia.org/wiki/Electoral_system).
-It's simple to vote and simple to tabulate.  While a completely fair and perfect
-electoral system is impossible, STAR Voting's approach makes reasonable tradeoffs
+relatively-new ["electoral system"](https://en.wikipedia.org/wiki/Electoral_system)--a
+method of running an election.  STAR Voting is simple--it's
+simple to vote, and simple to tabulate.  And while a completely
+fair and perfect electoral system is impossible,
+STAR Voting's approach makes sensible tradeoffs
 and avoids the worst pitfalls.  It's really great!
 
-This module, **starvote**, implements a simple STAR Voting tabulator.
+This module, **starvote**, implements a STAR Voting tabulator.
 It requires Python 3.7 or newer, but also supports CPython 3.6.
 (**starvote** relies on dictionaries preserving insertion order,
 which is guaranteed as of Python 3.7, but happened to work in CPython 3.6.)
 
 Features:
 
 * Supports four
   [electoral systems](https://en.wikipedia.org/wiki/Electoral_system):
 
   - [STAR Voting](https://www.starvoting.org/star), the snazzy
     new single-winner voting system.
   - [Bloc STAR Voting](https://www.starvoting.org/multi_winner),
-    a multi-winner variant of STAR voting that fills multiple
+    a multiwinner variant of STAR voting that fills multiple
     seats with the *most popular* candidates.
   - [Allocated Score Voting](https://electowiki.org/wiki/Allocated_Score),
     a [proportional representation](https://en.wikipedia.org/wiki/Proportional_representation)
     electoral system, and so far the only such system officially
     authorized to be a "Proportional STAR Voting" method.
   - [Reweighted Range Voting](https://rangevoting.org/RRV.html)
     (aka "RRV"), an alternative proportional representation
     electoral system.  RRV isn't a STAR variant, but like STAR
     it's a form of
     [score voting.](https://en.wikipedia.org/wiki/Score_voting)
     So the ballot and instructions to the voter are identical
     to a STAR-PR election.  The RRV algorithm is much simpler
     than Proportional STAR Voting, and its "never discard a voter"
     approach is appealing.
+  - [Sequentially Spent Score](https://electowiki.org/wiki/Sequentially_Spent_Score),
+    a third variety of score-based proportional representation
+    electoral system.
 
-* Implements the [Official Tiebreaker Protocol](https://www.starvoting.org/ties)
+* Implements the
+  [Official Tiebreaker Protocol](https://www.starvoting.org/ties)
   for STAR Voting and Bloc STAR Voting elections.
 
 * Provides a user-configurable final tiebreaker mechanism
   if the election (or one round in the election) ends in a tie.
 
   - The default tiebreaker mechanism randomly shuffles
     all the candidates in advance of running the election,
     then breaks the tie in favor of the candidate(s) that
     appear earliest in the list.
-  - Alternatively, you may choose to randomly pick a candidate
-    (or candidates) from the tied candidates, on demand.
+  - Alternatively, you can break ties by randomly picking
+    a candidate (or candidates) from the tied candidates,
+    on demand.
   - You can also implement your own custom tiebreaker.
-  - If you specify that there should be no tiebreaker, in
-    the event of an unbreakable tie the election will raise
-    an `UnbreakableTieError` exception.
+  - If you specify that there should be no tiebreaker,
+    and the election ends in an unbreakable tie, it will
+    raise an `UnbreakableTieError` exception.
 
 * All election tabulation calculations are performed using only integers
   and [fractions](https://docs.python.org/3/library/fractions.html).
-  This guarantees the calculations are 100% consistent and accurate
+  This guarantees results are 100% consistent and accurate
   across all platforms.  Floating-point rounding errors are
   impossible--because floats are never used!
 
 * Supports running elections specified in CSV files using
   [`https://star.vote/`](https://star.vote/) format.
 
-* Also supports running elections specified in a convenient custom
-  file format called *starvote format*.
+* Also supports running elections specified in
+  a convenient custom file format called *starvote format*.
 
-* *starvote* 2.0 passes its test suite with 100% coverage on
+* **starvote** 2.0.3 passes its test suite with 100% coverage on
   all supported versions.
 
-* *starvote* has no external dependencies.
+* **starvote** has no external dependencies.
 
 
 ## A quick STAR Voting primer
 
 When you vote using STAR Voting, your ballot looks something like this:
 
 ```
@@ -87,58 +94,67 @@
 
 To vote, give every candidate a score from 0 to 5.  5 means you like
 them the most, 0 means you like them the least.  (If you don't pick one
 of the scores, that's the same as a 0.)  If you give two candidates
 the same score, that means you like them equally--you don't have a
 preference between them.
 
-To figure out who won, you apply the **STAR** method: **S**core,
-**T**hen **A**utomatic **R**unoff.
+Tabulating the election is easy!  You apply the **STAR** method:
+**S**core, **T**hen **A**utomatic **R**unoff.
 
-In the first round, the score round, you add up the scores of all the
+In the first round, the *Scoring Round,* you add up the scores of all the
 candidates.  The top two scoring candidates automatically advance to
 the second round.
 
-In the second round, you examine every ballot to see which of the
-two remaining candidates they preferred.  If one has a higher score,
-that ballot prefers that candidate.  If the ballot scored both
-candidates the same, they have no preference.  The candidate that
-was preferred by more ballots wins the election.  It's that simple!
+In the second round, the *Automatic Runoff Round,* you examine every
+ballot to see which of the two remaining candidates they preferred.
+If one has a higher score, that ballot prefers that candidate.  If the
+ballot scored both candidates the same, they have no preference.
+The candidate preferred by more ballots wins the election.  It's that
+simple!
+
+And notice--you always examine every ballot.  STAR Voting never throws
+away ballots.  When you vote, your vote always matters,
+every step of the way.
 
 
 ## What's so good about STAR Voting?
 
 Electoral systems are a surprisingly deep topic.  They've been studied
-for hundreds of years, and there are many many different approaches.
+for hundreds of years, and there are many *many* different approaches.
 There are a number of desirable properties *and* undesirable properties
-that electoral systems can have.  And, bad news: it's impossible for
-there to be one best-possible voting system.  There are mutually
-exclusive desirable properties.  You can't make a one-size-fits-all
-system that avoids every problem.
+that electoral systems can have.  And here's the bad news: it's
+*impossible* for there to be one best-possible voting system.  There
+are mutually exclusive desirable properties, and there are desirable
+properties that bring with them downsides.  You just can't make a
+one-size-fits-all best system that avoids every problem--every electoral
+system has to be a compromise.  Wikipedia has
+[a comprehensive article](https://en.wikipedia.org/wiki/Comparison_of_electoral_systems)
+on the topic.
 
 STAR Voting avoid the worst problems of electoral systems.
 The remaining undesirable properties were chosen as the least-bad
 option.
 
-Here are some desirable properites STAR Voting displays:
+Here are some desirable properites STAR Voting has:
 
 * It's [monotonic.](https://en.wikipedia.org/wiki/Monotonicity_criterion)
   Giving a candidate a higher score can never hurt them, and
   giving a candidate a lower score can never help them.  (And yes,
   this is not always true of voting systems.  The increasingly popular
   [Instant Runoff Voting](https://en.wikipedia.org/wiki/Instant-runoff_voting)
   fails this; paradoxically, it's possible to *hurt* a candidate you
   prefer by giving them a *higher* score.)
 * It's [resolvable.](https://en.wikipedia.org/wiki/Resolvability_criterion)
   Ties are unlikely.
 * It complies with the [majority loser criterion.](https://en.wikipedia.org/wiki/Majority_loser_criterion)
   If a majority of candidates like one candidate the least, that candidate will
   never win a STAR Voting election.
 
-Here are some desirable properties STAR Voting doesn't have:
+But here are some desirable properties STAR Voting doesn't have:
 
 * It's not a [Condorcet method,](https://en.wikipedia.org/wiki/Condorcet_winner_criterion)
   which is a very particular property of an electoral system.
   Let's say you have an election with three candidates, A, B, and C.  You ask each voter
   to vote in three head-to-head races: "which do you like better, A or B?", "which do
   you like better, B or C?", and "which do you like better, A or C?"  If there's one
   candidate that wins in every such head-to-head vote in the election, they would be
@@ -160,62 +176,71 @@
   elected.  The STAR Voting team [wrote an essay on why they gave up on this criterion.](https://www.starvoting.org/pass_fail)
   The short version is: electoral systems that satisfy later-no-harm generally also
   exhibit
   [the spoiler effect,](https://en.wikipedia.org/wiki/Vote_splitting#%22Spoiler_effect%22)
   which is a worse property.  But achieving later-no-harm *and* avoiding the spoiler effect
   makes your electoral system even worse!
 
+(If there isn't a best-possible voting system, is there a worst-possible?  Maybe!
+If there *is* a worst electoral system, it's almost certainly
+[Plurality voting](https://en.wikipedia.org/wiki/Plurality_voting)...
+the predominant electoral system used here in the United States.  Sigh.)
+
 
 ## API
 
 ### `election`
 
-To use `starvote`, `import starvote`, then call the `election` method:
+To use `starvote`, first `import starvote`,
+then call its `election` function:
 
 ```Python
 def election(method, ballots, *,
     maximum_score=5,
     print=None,
     seats=1,
     verbosity=0,
     ):
 ```
 
-`election` tabulates an election based on your
-parameter and returns a `list` containing the
-winners. (Even for single-winner STAR Voting--in
+`election` tabulates an election based on the
+arguments you pass in and returns a `list` containing
+the winners. (Even for single-winner STAR Voting--in
 that case, the list will only contain one element.)
 
-`method` specifies which election system you want to use,
-via predefined `Method` objects. The allowed values are:
+`method` specifies which method (which "election system")
+you want to use in this election, via predefined `Method`
+objects. The supported values are:
 
 * `starvote.STAR_Voting`,
 * `starvote.Bloc_STAR_Voting`,
-* `starvote.Allocated_Score_Voting`, and
-* `starvote.Reweighted_Range_Voting`.
+* `starvote.Allocated_Score_Voting`,
+* `starvote.Reweighted_Range_Voting`, and
+* `starvote.Sequentially_Spent_Score`.
 
-Since those are a lot to
-type, `starvote` also provides nicknames, respectively:
+Since those are a lot to type, `starvote` also provides
+nicknames for these methods, respectively:
 
 * `starvote.star`,
 * `starvote.bloc`,
-* `starvote.allocated`, and
-* `starvote.rrv`.
+* `starvote.allocated`,
+* `starvote.rrv`, and
+* `starvote.sss`, and
 
 `ballots` should be an iterable containing individual ballots.
-Ballots are `dict` objects, mapping the candidate to that ballot's
-score for that candidate.  The candidate can be any Python value;
-the score must be an `int`.
+A ballot is a `dict` mapping the candidate to that ballot's
+score for that candidate.  The candidate can be any hashable
+Python value; the score must be an `int`.
 
-`maximum_score` specifies the maximum score allowed for any vote
-on any ballot.
+`maximum_score` specifies the maximum score allowed for
+any vote on any ballot.
 
 `seats` specifies how many seats the election should fill.
 STAR Voting is a single-winner method, so this should be
-`1` when using STAR Voting; for all the other methods,
+`1` when using STAR Voting; for the other methods,
 `seats` must be greater than or equal to `2`.
 
 `verbosity` specifies how much output you want.
 The current supported values are `0` (no output)
 and `1` (output); values higher than `1` are
 currently equivalent to `1`.
 
@@ -228,72 +253,79 @@
 
 ### Functions for specific electoral systems
 
 `starvote` also exports functions implementing each of
 the supported electoral systems:
 
 * `star_voting` implements single-winner STAR Voting.
-* `bloc_star_voting` implements multi-winner Bloc STAR Voting.
+* `bloc_star_voting` implements multiwinner Bloc STAR Voting.
 * `allocated_score_voting` implements Allocated Score Voting.
 * `reweighted_range_voting` implements Reweighted Range Voting.
+* `sequentially_spent_score` implements Sequentially Spent Score.
 
-These functions take much the same signature as `election`,
+These functions have much the same signature as `election`,
 with the following changes:
 
-* They don't take the `method` positional parameter;
-  the method is implicit in the function.  All four only
-  take one positional parameter, `ballots`, which is
-  required.
-* `star` doesn't take a `seats` parameter.  The other three
+* They don't have a `method` parameter; the method is implicit
+  in the function.  All four only take one positional parameter,
+  `ballots`, which is required.
+* `star` doesn't have a `seats` parameter.  The other three
   have a `seats` keyword-only parameter, and this parameter
-  is required--it doesn't have a default.  (A required
+  is required--it doesn't have a default.  (A *required*
   keyword-only parameter is pretty rare in Python!)
-* Note that these functions also always return a list,
-  even `star_voting`.
+* Note that, like `election`, these functions always
+  return a list, even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
 `starvote` ships a copy of the reference implementation
-of Allocated Score Voting.  Since this requires both NumPy
-and Pandas, it's not imported by default.  (I didn't want
+of Allocated Score Voting.  Since this requires both
+[NumPy](https://numpy.org/)
+and
+[Pandas](https://pandas.pydata.org/),
+it's not imported by default.  (I didn't want
 `starvote` to have any external dependencies.  The unit
 test suite runs correctly whether or not these external
 dependencies are installed.)
 
 You can import it with `import starvote.reference`;
 the directly-callable function is
 `starvote.reference.allocated_score_voting_reference`.
 You can also use the `Method` object
+`starvote.reference.Allocated_Score_Voting_reference`,
+with the nickname
+`starvote.reference.allocated_r`.
 
 If you want to integrate it into the `starvote` module,
 call`starvote.reference.monkey_patch()`.  This does
 three things:
 
-* Adds the function to the `starvote` module directly,
-  as `starvote.allocated_score_voting_reference`.
-* Adds it to `starvote.__all__` so that symbol
-  gets brought in by `from starvote import *`.
-*
+* Adds the function and `Method` objects to the `starvote`
+  module directly.
+
+  - Also adds them to `starvote.__all__` so they get
+    brought in by `from starvote import *`.
+
 * Adds the appropriate `Method` object
   to `starvote.methods`, using the name
   `'Allocated Score Voting (reference)'`
   and the nickname `allocated_r`.
 
 *Note:* the reference implementation doesn't support
 tiebreakers.  `allocated_score_voting_reference` *does*
 accept a `tiebreaker` argument, but currently it *must*
 be `None`.
 
 ### Ties
 
-The good news is, STAR Voting elections rarely result in a tie in the
-real world.  But ties can still happen.  The good news is, STAR Voting
-has a sensible, thorough protocol on how to break a tie.  The bad news is,
-not all ties are breakable--some ties genuinely represent the ambivalent
-will of the voters.
+STAR Voting elections rarely result in a tie in the real world.
+But ties can still happen.  The good news is, STAR Voting has a
+sensible, thorough protocol on how to break a tie.  The bad news is,
+not all ties are breakable--some ties genuinely represent the
+indecisive will of the voters.
 
 **starvote** gives you control over how to break ties in elections,
 through the `tiebreaker` parameter to `election` and the election-specific
 functions.  **starvote** also has two predefined tiebreaker functions,
 but you can substitute your own--or none at all.
 
 The default tiebreaker in **starvote** is
@@ -344,14 +376,22 @@
 
 If you pass in your own `candidates` list,
 you may also pass in a string for the
 `description` keyword-only parameter, which
 should be text describing the source of
 this ordered list of candidates.
 
+Note that, if you pass in your own
+`candidates` list, **starvote**'s tabulation
+of the election will be 100% deterministic
+and repeatable.  You can run that election
+a million times and you'll always get the
+same result.
+
+
 #### `on_demand_random_tiebreaker`
 
 If you prefer more unpredictability in your life,
 you can choose `on_demand_random_tiebreaker`
 to break ties.  `on_demand_random_tiebreaker` will
 simply pick a random candidate (or candidates)
 on demand, using Python's `random.sample` function.
@@ -547,17 +587,19 @@
 
 The `options` section specifies how to run the election.
 Assignment lines in the `options` section specify options;
 each name maps to a parameter to the `election` function.
 Here are all the supported names:
 
 ```
+    csv_path = <string>
     maximum score = <integer>
     method = <string>
     seats = <integer>
+    starvote_path = <string>
     tiebreaker = <string | list>
     verbosity = <integer>
 ```
 
 A *starvote format election* can specify each of these a maximum of once.
 
 An assignment line in the `options` section can also use
@@ -573,15 +615,16 @@
 
 * If you set a value to `[]`, it's set to an empty
   list, and the parser doesn't enable *list mode.*
 * You can't use pragmas or change sections while
   in *list mode.*
 * You can't nest lists.
 
-The only option that supports lists is `tiebreaker`.
+The only assignment that supports lists is the
+`tiebreaker` option in the `options` section.
 If `tiebreaker` is set to a string, this specifies
 the name of the tiebreaker in the `starvote.tiebreakers`
 dict to use for this election.  If `tiebreaker` is set
 to a string, `parse_starvote` looks up that string in
 the `options.tiebreakers` dict and uses the tiebreaker
 found there.  If `tiebreaker` is set
 to a list, this defines a pre-permuted list of candidates
@@ -611,14 +654,25 @@
 ```
     5 ballots:
 ```
 
 (You're explicitly permitted to have blank lines between the
 `ballots` pragma and the ballot it's repeating.)
 
+The `starvote_path` and `csv_path` options allow you to
+"import" another file into the current election.  They
+can specify relative or absolute paths; if relative,
+they will be resolved using the directory the *starvote
+format* file is in (if the *starvote format election* was
+loaded from a file) or the current directory.  Both settings
+will load ballots from the file specified; `starvote_path`
+will also load the options from the file specified, however
+any options set in the current election will override those
+options.
+
 #### Example
 
 Here's a sample starvote format election:
 
     [options]
 
     seats=3
@@ -690,66 +744,172 @@
 You may specify the text encoding using the
 `encoding` keyword-only parameter; the default
 encoding is `'utf-8'`.
 
 
 ### Command-line module
 
-The `starvote` module supports being run as a script (`python -m starvote`).
+The `starvote` module supports being run as a script
+(`python -m starvote`).
 Run it without arguments to see usage.
 
 To use, specify the path to a single file on the
 command-line.  `starvote` will read in the file,
 run the election, and print the result.
 
 The path may be a
 [CSV file.](https://en.wikipedia.org/wiki/Comma-separated_values)
 CSV files should end with the file extension `.csv`,
 and be in
 [`https://star.vote/`](https://star.vote/)
 format.  By default elections in CSV files are run
-using STAR Voting.
+using STAR Voting, for one seat, with `verbosity=1`
+and the default tiebreaker.
 
 Alternatively, the path may be a *starvote format* file.
-*starvote format* files should end with the file extension `.starvote`
-and contain a *starvote format election* in UTF-8 format.
+*starvote format* files should end with the file extension
+`.starvote` and contain a *starvote format election* in
+UTF-8 format.  *starvote format elections* explicitly
+specify all the parameters of the election.
 
 For example, you can run this from the root of the
 source-code repository:
 
 ```
 % python3 -m starvote test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
 ```
 
 to see how **starvote** handles ties during the automatic runoff round.
 
 
 ## Multiple-winner elections
 
-**starvote** also implements several multi-winner electoral systems:
-
-Simply instantiate your `Poll` object passing in the enum constant
-`starvote.Bloc_STAR`, `starvote.Proportional_STAR`,
-or `starvote.Reweighted_Range`
-for the `electoral_system` parameter, and the number of seats in
-the `seats` keyword-only parameter:
+**starvote** also implements several multiwinner electoral systems.
+All you need to do is pass in one of the multiwinner methods, such as
+`starvote.bloc`, `starvote.allocated`,
+or `starvote.rrv`, when you call `election`:
 
 ```Python
-poll = starvote.Poll(electoral_system=starvote.Bloc_STAR, seats=2)
+poll = election(starvote.bloc, ballots, seats=2)
 ```
 
 You can experiment with these with the command-line version of the
-module, too.  You can specify the electoral system with `-e`,
+module too.  Simply specify the method with `-m`,
 the number of seats with `-s`,
-and the maximum score with `-m`:
+and the maximum score with `-x`.
+These will override the settings from inside a *starvote format* file
+(and the default settings for CSV files).
+
+### Multiwinner vs proportional
+
+Here's a quick explanation about what "proportional voting" means,
+in the context of multiwinner elections.
+As with every other topic, you can read more about it
+[at Wikipedia.](https://en.wikipedia.org/wiki/Proportional_representation)
+
+A straight multiwinner election simply means you're electing
+2 or more candidates instead of one candidate.  The candidates
+that get the most votes--or however the election is tabulated--win.
+
+But electing only the most popular candidates can be a poor
+representation of the electorate.  Let's say you have a city
+election to fill five seats.  In this city, 60% of the voters
+vote only for party A, and 40% of the voters vote only for
+party B.  Bloc STAR Voting would very likely award all five
+seats to party A candidates.  Is that fair?  It seems like the
+["tyranny of the majority".](https://en.wikipedia.org/wiki/Tyranny_of_the_majority)
+
+There's an alternate approach to apportioning seats, used
+in political systems across the world, called "Proportional
+Representation".  The idea is, you have N seats, and you
+assign portions of them based on representing portions of
+the populace.  In the above example, you'd *want* to give
+three seats to party A and two seats to party B.  What
+system could do that?
+
+Often proportional representation is done based on voting
+for parties rather than voting for candidates.  This is
+called
+[Party-list proportional representation,](https://en.wikipedia.org/wiki/Party-list_proportional_representation)
+and it's used to elect governmental bodies across the world.
+
+But there are voting methods that permit voting directly for
+candidates and produces proportional representation.
+Allocated Score Voting, Reweighted Range Voting, and
+Sequentially Spent Score are three such methods.
+They all work something like this:
+
+* Each vote is a number, with higher numbers
+  indicating a stronger preference.
+* You run N rounds of the election to fill N seats,
+  each round electing one candidate.
+* When a candidate is elected, we may *allocate* ballots
+  to that candidate, which means we consider them used-up
+  and we remove them from the election.  If you vote
+  for candidate A1, and candidate A1 wins the first round,
+  your ballot might get "allocated" to candidate A1 and
+  ignored for the rest of the election.
+* Alternatively, we may *re-weigh* the
+  ballots of voters who voted for that candidate.
+  That means we reduce the voting power of those ballots.
+  If in the election, you voted for candidate A1, and A1
+  wins the first round, in the second round your vote
+  will count for less.  But if I gave A1 a score of 0,
+  my ballot would still be at full strength.
+
+The differences between the three is how they allocate
+vs. reweigh ballots. Allocated Score Voting and Sequentially
+Spent Score both allocate ballots, Reweighted Range Voting
+never does--with RRV every vote is counted in every round.
+Also, the three systems use different formulae to compute the
+new weight of a ballot after each round.  In Allocated Score
+and Sequentially Spent Score,
+the new weight is based on how many excess voters were needed
+to fill a quota (called a
+[Hare quota](https://en.wikipedia.org/wiki/Hare_quota));
+in Reweighted Range Voting, the new weight is based on the
+sum of the score(s) you contribute to the winning candidate(s).
+
+**starvote** ships a sample election that nicely demonstrates
+how direct-elected proportional representation elections can work:
+
+```
+test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+This election is like the example election I used in the description
+above.  It uses Reweighted Range Voting to fill three seats, and each
+vote has a maximum score of 10.
+60 of the voters prefer party A, and give high scores to candidates A1, A2, and A3;
+40 of the voters prefer party B, and give high scores to candidates B1 and B2.
+
+You can run the election in the `starvote` main directory with this command:
 
 ```
 % python3 -m starvote test_elections/test_election_reweighted_range_sample_election.starvote
 ```
 
+To see how the tabulation works using Allocated Score Voting, run this:
+
+```
+% python3 -m starvote -m allocated test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+You can also see how it changes with Sequentially Spent Score by running this:
+
+```
+% python3 -m starvote -m allocated test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+And to see the tyrrany of the majority in action, this command will tabulate the election using Bloc STAR Voting:
+
+```
+% python3 -m starvote -m bloc test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
 ### Warning
 
 I haven't found a single test corpus for Bloc STAR Voting.
 I'm following the rules as best I can, and the results I'm getting
 make sense.  But so far I can't confirm my implementation is
 correct--there's a very real possibility I got something wrong.
 
@@ -763,15 +923,16 @@
 ## Thanks
 
 Huge thanks to Tim Peters for his continuous input during the
 development of this library.  Although Tim didn't have any input
 on the library itself--if you don't like the library it's 100%
 my fault!--he tirelessly answered all my questions about voting
 during its development, and convinced me to change my approach
-several times.
+several times.  In particular, Tim's feedback pushed me to
+develop the `tiebreaker` plug-in interface.
 
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
@@ -789,15 +950,31 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
-**2.0.3** - *2023/05/27*
+**2.0.4** - *2023/06/05*
+
+* Added support for Sequentially Spent Score voting.
+* Changed presentation slightly for Allocated Score:
+  the average vote is now computed using the count of
+  *all* ballots in the election, including allocated
+  ballots.  (Previously the average was computing using
+  just the *remaining* ballots.)  This doesn't change
+  the outcome of the election, it's just a presentation
+  change.
+* Removed last traces of "STAR-PR", which I thought was
+  an alternate name for Allocated Score.
+* Doc changes.  Standardized on the spelling "multiwinner",
+  instead of "multi-winner".
+
+
+**2.0.3** - *2023/06/01*
 
 * Normalized nomenclature for `Method` objects.  Now,
   every method has an official correctly-spelled
   correctly-capitalized name, and exactly one "nickname".
   The nickname is always lowercase, and would return
   True for `isidentifier`.  These are used in the
   `starvote.method` map; a variant of these names is
@@ -805,27 +982,27 @@
   valid identifiers).
 * Improved `starvote.reference.monkey_patch`.  It's now
   data-driven and thus more reliable.
 * Added `starvote.reference.__all__`, in case you want
   to `from starvote.reference import *`.
 * Doc fixes.
 
-**2.0.2** - *2023/05/27*
+**2.0.2** - *2023/06/01*
 
 * Renamed the `tiebreaker` parameter `candidates` to `tie`.
 * Evicted some testing-only tiebreakers from the `starvote`
   module.  They're now in their own script, which only gets
   loaded when working with the test suite.
 
-**2.0.1** - *2023/05/27*
+**2.0.1** - *2023/06/01*
 
 * Changed the nickname of the reference version of
   Allocated Score Voting to "Allocated-R".
 
-**2.0** - *2023/05/27*
+**2.0** - *2023/06/01*
 
 A complete rewrite!  The 1.x code base was pretty smelly.
 This codebase is much, much cleaner--and I think I squashed
 one or two bugs too.
 
 `starvote` has an entirely new, functional API. `election`
 runs the election for you, and takes two required positional
@@ -835,15 +1012,15 @@
 
 You can also now pass in a handler for unbreakable ties.
 By default, unbreakable ties are now broken using a
 pre-chosen randomize list of candidates.  (`election` can
 still raise `UnbreakableTieError` exceptions if you prefer.)
 
 You can also call the voting method functions directly:
-`star`, `bloc_star`, `proportional_star`, and `reweighted_range`
+`star`, `bloc_star`, `proportional_star`, `reweighted_range`,
 are all functions, too.  These omit the `method` parameter
 but still require the `ballots` parameter.
 
 There's also a new text format for storing an election,
 *starvote format,* with the `.starvote` file extension.
 *starvote format* is a nice alternative to `.csv` files.
```

### Comparing `starvote-2.0.3/docs/clarifying_star_voting.md` & `starvote-2.0.4/docs/clarifying_star_voting.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/docs/formatting_fractions_in_columns_of_text.txt` & `starvote-2.0.4/docs/formatting_fractions_in_columns_of_text.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/pyproject.toml` & `starvote-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/starvote/__init__.py` & `starvote-2.0.4/starvote/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 ##
 ## TODO
 ##
 ## * write a unit test that checks the code examples
 ##   in README.md are up to date
 ##     * confirms "example.py" and the output in README.md matches
 ##     * confirms the "multi-winner elections" cmdline works
-##   (I keep breaking these.)
+##   (I keep breaking 'em.)
+##
+## * output
+##     * alternate output format idea:
+##         * make something more computer-readable.
+##         * maybe just super-regular HTML, with classes and names to make it easy?
+##     * allow displaying in floats
+##     * restore printing the preference matrix (it's lurking in 1.x versions)
 ##
 
 __doc__ = "An election tabulator for the STAR electoral system, and others"
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 __all__ = [
     'Allocated_Score_Voting', # Method
     'allocated', # Method (nickname)
     'allocated_score_voting', # function
     'Bloc_STAR_Voting', # Method
     'bloc', # Method (nickname)
@@ -28,16 +35,19 @@
     'Options', # class
     'predefined_permutation_tiebreaker', # tiebreaker class
     'parse_starvote', # function
     'on_demand_random_tiebreaker', # tiebreaker function
     'Reweighted_Range_Voting', # Method
     'rrv', # Method (nickname)
     'reweighted_range_voting', # function
+    'Sequentially_Spent_Score', # Method
+    'sss', # Method (nickname)
+    'sequentially_spent_score', # function
     'STAR_Voting', # Method
-    'star', # Method (name)
+    'star', # Method (nickname)
     'star_voting', # function
     'Tiebreaker', # class
     'tiebreakers', # maps string to tiebreakers
     'UnbreakableTieError', # exception class
     'UsageException', # exception class
     ]
 
@@ -615,16 +625,17 @@
                 spacer = ' ' * delta
                 average = f" (average {stripped}){spacer}"
             a = annotation(candidate)
             print(f"  {candidate:{candidate_width}} -- {score}{average}{a}".rstrip())
 
         self.print_result(first, second, tie, advance=advance)
 
-    def print_scores_and_averages(self, ballots, scores, first, second, tie, *, advance=False, no_preference=None):
-        ballot_count = len(ballots)
+    def print_scores_and_averages(self, ballots, scores, first, second, tie, *, advance=False, no_preference=None, ballot_count=None):
+        if ballot_count is None:
+            ballot_count = len(ballots)
         averages = {candidate: Fraction(score, ballot_count) for candidate, score in scores.items()}
         self.print_scores(scores, first, second, tie, advance=advance, averages=averages, no_preference=no_preference)
 
     def election_result(self, winners, tie, *, raise_tie=True):
         if not (winners or tie):
             raise ValueError("winners and tie are both false, exactly one must be true")
         if winners and tie:
@@ -757,15 +768,15 @@
     either the numerator or denominator of the
     Fraction constructor, and it normalizes the
     value internally--the resulting Fraction
     will have integers for the numerator and
     denominator.  Thanks, Sjoerd and Jeffrey!
     """
     assert isinstance(numerator, (int, Fraction))
-    assert isinstance(denominator, int)
+    assert isinstance(denominator, (int, Fraction))
 
     if denominator == 1:
         f = numerator
         is_fraction = isinstance(f, Fraction)
     else:
         f = Fraction(numerator, denominator)
         is_fraction = True
@@ -1495,15 +1506,16 @@
         maximum_score=maximum_score,
         print=print,
         seats=seats,
         tiebreaker=tiebreaker,
         verbosity=verbosity,
         )
 
-    hare_quota = _fraction_or_int(len(ballots), seats)
+    original_ballot_count = len(ballots)
+    hare_quota = _fraction_or_int(original_ballot_count, seats)
 
     options.initialize(ballots, messages=[f"Hare quota is {hare_quota}."])
 
     scores = _scoring_round(ballots)
     if len(scores) == seats:
         with options.heading(f"Round 1"):
             if options.verbosity:
@@ -1525,35 +1537,35 @@
 
     decorated_ballots = [[None, 1, dict(ballot), dict(ballot)] for ballot in ballots]
     # "ballots" is just column 3 of this list.  we need a list
     # of just the ballots to pass in to _scoring_round.
     # sometimes (but not always) we throw away ballots in the
     # allocation round, which means that sometimes (but not always)
     # we need to recalculate this list during the loop.
-    recalculate_ballots = True
+    recalculate_weighted_ballots = True
 
     candidates = None
 
     try:
         for polling_round in range(1, seats+1):
             with options.round_heading(f"Round {polling_round}"):
-                if recalculate_ballots:
-                    ballots = [t[INDEX_WEIGHTED_BALLOT] for t in decorated_ballots]
-                    recalculate_ballots = False
+                if recalculate_weighted_ballots:
+                    weighted_ballots = [t[INDEX_WEIGHTED_BALLOT] for t in decorated_ballots]
+                    recalculate_weighted_ballots = False
 
-                scores = _scoring_round(ballots, candidates)
+                scores = _scoring_round(weighted_ballots, candidates)
                 first, tie = _compute_first_from_scores(scores)
 
                 if candidates is None:
                     candidates = set(scores)
 
                 if options.verbosity:
-                    options.print_ballot_count_if_changed(ballots)
+                    options.print_ballot_count_if_changed(weighted_ballots)
                     options.print("The highest-scoring candidate wins a seat.")
-                    options.print_scores_and_averages(ballots, scores, first, None, tie, advance="wins a seat")
+                    options.print_scores_and_averages(weighted_ballots, scores, first, None, tie, advance="wins a seat", ballot_count=original_ballot_count)
 
                 if tie:
                     tie_winner = options.break_tie(f"{int_to_words(len(tie), flowery=False)}-way tie in Scoring Round", tie, 1)
                     first = tie_winner[0]
 
                 winners.append(first)
                 candidates.remove(first)
@@ -1606,16 +1618,16 @@
 
                             if options.verbosity:
                                 options.print(f"Allocating {allocation_count} ballot{pluralizer(allocation_count)} at score {score}.")
                             if allocation_count <= quota:
                                 del supporters[score_start:]
                                 quota = _fraction_or_int(quota - allocation_count)
                                 # deleted some ballots, so we have to
-                                # recalculate both ballots and decorated_ballots
-                                recalculate_ballots = True
+                                # recalculate both weighted_ballots and decorated_ballots
+                                recalculate_weighted_ballots = True
                                 if not quota:
                                     break
                                 continue
 
                             # this group has more supporters than we need to fill the quota.
                             # reduce every supporter's vote by the surplus, then keep them in play.
                             # since this fills the quota, we always exit the loop after this.
@@ -1675,30 +1687,29 @@
 
                                 for key, count in counts:
                                     starting_weight, weight = key
                                     options.print(f"{prefix}{count} ballot{pluralizer(count)} reweighted from {starting_weight} to {weight}.")
 
                             break
 
-                    if recalculate_ballots:
+                    if recalculate_weighted_ballots:
                         decorated_ballots = non_supporters + supporters
 
         _attempt_to_sort(winners)
         tie = None
     except UnbreakableTieError as e:
         winners = None
         tie = e
     return options.election_result(winners, tie)
 
 Allocated_Score_Voting = allocated = Method("Allocated Score Voting", allocated_score_voting, True)
 for _ in ('Allocated Score Voting', 'allocated'):
     methods[_] = Allocated_Score_Voting
 
 
-
 def reweighted_range_voting(ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
     seats,
     tiebreaker=_DEFAULT_TIEBREAKER,
     verbosity=_DEFAULT_VERBOSITY,
     ):
@@ -1831,14 +1842,210 @@
     return options.election_result(winners, tie)
 
 Reweighted_Range_Voting = rrv = Method("Reweighted Range Voting", reweighted_range_voting, True)
 for _ in ('Reweighted Range Voting', 'rrv'):
     methods[_] = Reweighted_Range_Voting
 
 
+def sequentially_spent_score(ballots, *,
+    maximum_score=_DEFAULT_MAXIMUM_SCORE,
+    print=_DEFAULT_PRINT,
+    seats,
+    tiebreaker=_DEFAULT_TIEBREAKER,
+    verbosity=_DEFAULT_VERBOSITY,
+    ):
+    """
+    Tabulates an election using Sequentially Spent Score:
+        https://electowiki.org/wiki/Sequentially_Spent_Score
+
+    Returns a list of results.
+
+    Takes one required positional parameter:
+    * "ballots" should be an iterable of ballot dicts.
+
+    Also accepts five optional keyword-only parameters:
+    * "maximum_score" specifies the maximum score allowed
+      per vote, default 5.
+    * "print" is a function called to print output.
+    * "seats" specifies the number of seats,
+      for multiwinner elections.
+    * "tiebreaker" specifies how to break ties;
+      should be a tiebreaker function or Tiebreaker
+      object.
+    * "verbosity" is an int specifying how much output
+      you want; 0 indicates no output, higher numbers
+      add more output.
+    """
+
+    options = Options(
+        Sequentially_Spent_Score,
+
+        maximum_score=maximum_score,
+        print=print,
+        seats=seats,
+        tiebreaker=tiebreaker,
+        verbosity=verbosity,
+        )
+
+    original_ballot_count = len(ballots)
+    hare_score_quota = _fraction_or_int(original_ballot_count * maximum_score, seats)
+    presentation_hare_score_quota = "".join(split_int_or_fraction_as_str(hare_score_quota))
+
+    options.initialize(ballots, messages=[f"Hare score quota is {presentation_hare_score_quota}."])
+
+    scores = _scoring_round(ballots)
+    if len(scores) == seats:
+        with options.heading(f"Round 1"):
+            if options.verbosity:
+                options.print(f"There are exactly {seats} candidates seeking {seats} seats.  Every candidate wins.")
+        winners = list(scores)
+        _attempt_to_sort(winners)
+        return winners
+
+    stars = maximum_score
+    weight = 1
+    # t = [weighted_ballot, ballot, stars, weight]
+
+    INDEX_WEIGHTED_BALLOT = 0
+    INDEX_BALLOT = 1
+    INDEX_STARS = 2
+    INDEX_WEIGHT = 3
+    decorated_ballots = [ [dict(b), dict(b), stars, weight] for b in ballots ]
+    weighted_ballots = [t[INDEX_WEIGHTED_BALLOT] for t in decorated_ballots]
+    winners = []
+    first = None
+    candidates = None
+
+    try:
+        for polling_round in range(1, seats+1):
+            with options.round_heading(f"Round {polling_round}"):
+
+                scores = _scoring_round(weighted_ballots, candidates)
+                first, tie = _compute_first_from_scores(scores)
+
+                if candidates is None:
+                    candidates = set(scores)
+
+                if options.verbosity:
+                    options.print_ballot_count_if_changed(ballots)
+                    options.print("The highest-scoring candidate wins a seat.")
+                    options.print_scores_and_averages(ballots, scores, first, None, tie, advance="wins a seat")
+
+                if tie:
+                    tie_winner = options.break_tie(f"{int_to_words(len(tie), flowery=False)}-way tie in Scoring Round", tie, 1)
+                    first = tie_winner[0]
+
+                winners.append(first)
+                candidates.remove(first)
+
+                if len(winners) == seats:
+                    # success!
+                    break
+
+                with options.subround_heading("Ballot allocation round"):
+                    winner_score = scores[first]
+                    if not winner_score:
+                        # all votes for candidate were zero.
+                        # nobody has to give back any stars.
+                        continue
+
+                    weight_reduction_ratio = min( _fraction_or_int(hare_score_quota, winner_score), 1)
+                    one_minus_weight_reduction_ratio = 1 - weight_reduction_ratio
+                    have_surplus = weight_reduction_ratio < 1
+
+                    if options.verbosity:
+                        counts = defaultdict(int)
+                        modified = 0
+                        if have_surplus:
+                            giving_back_surplus = "giving back surplus"
+                            # no need to normalize this for presentation via split_fraction_or_int,
+                            # one_minus_weight_reduction_ratio is guaranteed to be either 1 or a fraction < 1
+                            reduction = f" * {one_minus_weight_reduction_ratio}"
+                        else:
+                            giving_back_surplus = "no surplus to give back"
+                            reduction = ""
+
+                        presentation_winner_score = "".join(split_int_or_fraction_as_str(winner_score))
+                        options.print(f"Total score is {presentation_winner_score}, Hare score quota is {presentation_hare_score_quota}, {giving_back_surplus}.")
+                        options.print(f"Reducing each ballot's stars by their vote{reduction}.")
+
+                        remaining_decorated_ballots = []
+                        remaining_weighted_ballots = []
+
+                        allocated = 0
+                        for t in decorated_ballots:
+                            weighted_ballot, ballot, stars, weight = t
+
+                            score = weighted_ballot.get(first, 0)
+
+                            if score:
+                                starting_stars = stars
+                                star_reduction = score
+                                if have_surplus:
+                                    star_reduction = _fraction_or_int(star_reduction * weight_reduction_ratio)
+
+                                stars = max(stars - star_reduction, 0)
+                                if stars != starting_stars:
+                                    if not stars:
+                                        # remove, uh I mean "allocate", ballot
+                                        # (don't append to remaining_decorated_ballots)
+                                        allocated += 1
+                                        continue
+
+                                    t[INDEX_STARS] = stars
+
+                                    weight = _fraction_or_int(stars, maximum_score)
+                                    t[INDEX_WEIGHT] = weight
+
+                                    for c, s in ballot.items():
+                                        weighted_ballot[c] = s * weight
+
+                                    if options.verbosity:
+                                        key = (score, weight, starting_stars, stars)
+                                        counts[key] += 1
+                                        modified += 1
+
+                                remaining_decorated_ballots.append(t)
+                                remaining_weighted_ballots.append(weighted_ballot)
+
+                        if allocated:
+                            decorated_ballots = remaining_decorated_ballots
+                            weighted_ballots = remaining_weighted_ballots
+
+                        if options.verbosity:
+                            if allocated:
+                                options.print(f"Allocated {allocated} ballot{pluralizer(allocated)}.")
+
+                            # convert counts to list,
+                            counts = list(counts.items())
+                            if len(counts) == 1:
+                                prefix = ""
+                            else: # pragma: no cover
+                                options.print(f"Reweighted {modified} ballot{pluralizer(modified)}:")
+                                prefix = "   "
+                                # then sort by count then key, highest first.
+                                counts.sort(key=lambda t: (t[1], t[0]), reverse=True)
+
+                            for key, count in counts:
+                                score, weight, starting_stars, stars = key
+                                options.print(f"{prefix}{count} ballot{pluralizer(count)} voted {score}, stars reduced from {starting_stars} to {stars}, reweighted to {weight}.")
+
+
+        _attempt_to_sort(winners)
+        tie = None
+    except UnbreakableTieError as e:
+        winners = None
+        tie = e
+    return options.election_result(winners, tie)
+
+Sequentially_Spent_Score = sss = Method("Sequentially Spent Score", sequentially_spent_score, True)
+for _ in ('Sequentially Spent Score', 'sss'):
+    methods[_] = Sequentially_Spent_Score
+
+
 def election(method, ballots, *,
     maximum_score=_DEFAULT_MAXIMUM_SCORE,
     print=_DEFAULT_PRINT,
     seats=_DEFAULT_SEATS,
     tiebreaker=_DEFAULT_TIEBREAKER,
     verbosity=_DEFAULT_VERBOSITY,
     ):
@@ -1883,15 +2090,15 @@
         verbosity=verbosity,
 
         **extra_kwargs
         )
 
 
 
-def parse_starvote(starvote, *, path="<string>"):
+def parse_starvote(starvote, *, path=None):
     """
     Parses a custom election text format called "starvote format".
     Returns a kwargs dict usable for running an election, e.g.
         result = election(**parse_starvote(s))
 
     parse_starvote takes one required parameter: starvote, which
     must be a "starvote format" election string.  parse_starvote
@@ -2010,19 +2217,20 @@
         Chuck = 3
 
     (Why'd I write this?  I got tired of CSV files.)
     """
 
     exception_prefix_format = "Line {line_number}: " # deliberately not f-string
 
-    if path != "<string>":
+    if path:
         exception_prefix_format = f"File '{path}', " + exception_prefix_format
         current_directory = pathlib.Path(path).parent
     else:
         current_directory = pathlib.Path(os.getcwd())
+        path = "<string>"
 
 
     ballots = []
     kwargs = {}
     _sentinel = object()
 
     option_to_kwarg = {
@@ -2560,15 +2768,15 @@
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/starvote/reference.py` & `starvote-2.0.4/starvote/reference.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/README.md` & `starvote-2.0.4/test_elections/README.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/bad_syntax_ballot_pragma_as_last_line.txt` & `starvote-2.0.4/test_elections/bad_syntax_no_section.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-ValueError("'5 ballots: invalid as last line of a starvote format election")
+File 'test_elections/bad_syntax_no_section.starvote', Line 2: no section specified
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_change_section_in_list.txt` & `starvote-2.0.4/test_elections/bad_syntax_repeated_section.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_change_section_in_list.starvote', Line 6: you can't change sections inside a list
+File 'test_elections/bad_syntax_repeated_section.starvote', Line 6: section [options] specified twice
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_1.txt` & `starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_fussy_wrong_ballots_1.starvote', Line 7: ballots pragma must specify 2 or more repetitions
+File 'test_elections/bad_syntax_fussy_wrong_ballots_2.starvote', Line 7: ballot pragma must specify exactly 1 repetition
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_fussy_wrong_ballots_2.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_method.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_fussy_wrong_ballots_2.starvote', Line 7: ballot pragma must specify exactly 1 repetition
+File 'test_elections/bad_syntax_invalid_method.starvote', Line 3: invalid method 'bafflegab'
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_method.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_invalid_method.starvote', Line 3: invalid method 'bafflegab'
+File 'test_elections/bad_syntax_invalid_pragma.starvote', Line 3: unsupported pragma bafflegab
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_option.txt` & `starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_invalid_option.starvote', Line 3: unknown option 'bafflegab'
+File 'test_elections/bad_syntax_change_section_in_list.starvote', Line 6: you can't change sections inside a list
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_pragma.txt` & `starvote-2.0.4/test_elections/bad_syntax_malformed_section.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_invalid_pragma.starvote', Line 3: unsupported pragma bafflegab
+File 'test_elections/bad_syntax_malformed_section.starvote', Line 3: bad syntax '[option'
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_start_of_line_mode.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-ValueError("Line 3: bad syntax 'tiebreaker = [ Amy'")
+File 'test_elections/bad_syntax_invalid_tiebreaker.starvote', Line 3: invalid tiebreaker 'bafflegab'
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_1.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_starvote_path_2.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_invalid_tiebreaker.txt` & `starvote-2.0.4/test_elections/bad_syntax_repeated_option.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_invalid_tiebreaker.starvote', Line 3: invalid tiebreaker 'bafflegab'
+File 'test_elections/bad_syntax_repeated_option.starvote', Line 5: specified option 'method' twice
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_malformed_section.txt` & `starvote-2.0.4/test_elections/bad_syntax_no_equals.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_malformed_section.starvote', Line 3: bad syntax '[option'
+ValueError("Line 4: bad syntax 'bafflegab is confusing stuff!'")
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_no_ballots.txt` & `starvote-2.0.4/test_elections/bad_syntax_no_ballots.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_no_equals.txt` & `starvote-2.0.4/test_elections/bad_syntax_no_method.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-ValueError("Line 4: bad syntax 'bafflegab is confusing stuff!'")
+electoral system undefined, specify with -e|--electoral-system
+(or with method= in the [options] section of your starvote file)
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_no_method.txt` & `starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-electoral system undefined, specify with -e|--electoral-system
-(or with method= in the [options] section of your starvote file)
+File 'test_elections/bad_syntax_pragma_in_options.starvote', Line 4: unknown pragma 3 ballots
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_no_section.txt` & `starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_no_section.starvote', Line 2: no section specified
+File 'test_elections/bad_syntax_fussy_wrong_ballots_1.starvote', Line 7: ballots pragma must specify 2 or more repetitions
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_pragma_in_options.txt` & `starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_pragma_in_options.starvote', Line 4: unknown pragma 3 ballots
+File 'test_elections/bad_syntax_pragma_inside_list.starvote', Line 7: you can't use pragmas inside a list
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_pragma_inside_list.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_pragma_inside_list.starvote', Line 7: you can't use pragmas inside a list
+ValueError("Line 3: bad syntax 'tiebreaker = [ Amy'")
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_repeated_option.txt` & `starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_repeated_option.starvote', Line 5: specified option 'method' twice
+ValueError("'5 ballots: invalid as last line of a starvote format election")
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/bad_syntax_repeated_section.txt` & `starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-File 'test_elections/bad_syntax_repeated_section.starvote', Line 6: section [options] specified twice
+ValueError('tiebreaker list must not be empty')
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt` & `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv` & `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt` & `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.csv` & `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_best_akali_skins.txt` & `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_eurovision_song_contest_2023.txt` & `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt` & `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt` & `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt`

 * *Files 2% similar despite different names*

```diff
@@ -110,33 +110,33 @@
   This allocation overfills the remaining quota.  Returning fractional surplus.
   Allocating only 97.29% of these ballots.
   Keeping these ballots, but multiplying their weights by 31/1145.
   229 ballots reweighted from 3776/6685 to 117056/7654325.
 [Allocated Score Voting: Round 4]
   Tabulating 2550 remaining ballots.
   The highest-scoring candidate wins a seat.
-    Jacob Hornberger  -- 1404+   2591394/558765725  (average 130751611549/237475433125)  -- First place
-    Adam Kokesh       -- 1017+   1822363/7654325    (average   3893135444/9759264375)
-    Jo Jorgensen      --  912+ 303828914/558765725  (average 254949085057/712426299375)
-    Daniel Behrman    --  866+  74522901/558765725  (average  28468567103/83814858750)
-    Sam Robb          --  642+ 172269227/558765725  (average 358899864677/1424852598750)
-    John Monds        --  624+ 366095728/558765725  (average 174517954064/712426299375)
-    Arvin Vohra       --  362+ 643370509/1117531450 (average 135063251803/949901732500)
-    Sorinne Ardeleanu --  339+   1645444/3192947    (average   1084054477/8142014850)
-    Brian Ellison     --  285+   3885862/79823675   (average  22753633237/203550371250)
-    Mark Whitney      --  251+ 522234499/1117531450 (average  93674209483/949901732500)
-    Phil Gray         --  242+    236667/159647350  (average  38634895367/407100742500)
-    Kenneth Blevins   --  240+    838169/6385894    (average   1533452729/16284029700)
-    Jedidiah Hill     --  222+  89412069/111753145  (average   8299536753/94990173250)
-    Steve Richey      --  203+ 250700766/558765725  (average 113680142941/1424852598750)
-    James Ogle        --  200+  32696941/79823675   (average  15997431941/203550371250)
-    Erik Gerhardt     --  199+1032247577/1117531450 (average  74473668709/949901732500)
-    Keenan Dunham     --  196+1075144233/1117531450 (average 220111308433/2849705197500)
-    Rhett Smith       --  189+  28956584/558765725  (average 105635678609/1424852598750)
-    Louis Vanacore    --  183+ 251823242/558765725  (average 102505950917/1424852598750)
+    Jacob Hornberger  -- 1404+   2591394/558765725  (average 784509669294/1625449494025) -- First place
+    Adam Kokesh       -- 1017+   1822363/7654325    (average   7786270888/22266431425)
+    Jo Jorgensen      --  912+ 303828914/558765725  (average 509898170114/1625449494025)
+    Daniel Behrman    --  866+  74522901/558765725  (average 483965640751/1625449494025)
+    Sam Robb          --  642+ 172269227/558765725  (average 358899864677/1625449494025)
+    John Monds        --  624+ 366095728/558765725  (average 349035908128/1625449494025)
+    Arvin Vohra       --  362+ 643370509/1117531450 (average 405189755409/3250898988050)
+    Sorinne Ardeleanu --  339+   1645444/3192947    (average   1084054477/9288282823)
+    Brian Ellison     --  285+   3885862/79823675   (average  22753633237/232207070575)
+    Mark Whitney      --  251+ 522234499/1117531450 (average 281022628449/3250898988050)
+    Phil Gray         --  242+    236667/159647350  (average  38634895367/464414141150)
+    Kenneth Blevins   --  240+    838169/6385894    (average   1533452729/18576565646)
+    Jedidiah Hill     --  222+  89412069/111753145  (average  24898610259/325089898805)
+    Steve Richey      --  203+ 250700766/558765725  (average 113680142941/1625449494025)
+    James Ogle        --  200+  32696941/79823675   (average  15997431941/232207070575)
+    Erik Gerhardt     --  199+1032247577/1117531450 (average 223421006127/3250898988050)
+    Keenan Dunham     --  196+1075144233/1117531450 (average 220111308433/3250898988050)
+    Rhett Smith       --  189+  28956584/558765725  (average 105635678609/1625449494025)
+    Louis Vanacore    --  183+ 251823242/558765725  (average 102505950917/1625449494025)
   Jacob Hornberger wins a seat.
 [Allocated Score Voting: Round 4: Ballot allocation round]
   Allocating 581+4/5 ballots.
 [Allocated Score Voting: Round 4: Ballot allocation round: Round 1]
   Allocating 101 ballots at score 5.
 [Allocated Score Voting: Round 4: Ballot allocation round: Round 2]
   Remaining allocation quota is 2404/5.
@@ -180,32 +180,32 @@
   This allocation overfills the remaining quota.  Returning fractional surplus.
   Allocating only 43.38% of these ballots.
   Keeping these ballots, but multiplying their weights by 201/355.
   71 ballots reweighted from 3776/6685 to 758976/2373175.
 [Allocated Score Voting: Round 5]
   Tabulating 1999 remaining ballots.
   The highest-scoring candidate wins a seat.
-    Adam Kokesh       -- 376+ 7396779449/79344732950 (average 29841016368649/158610121167050) -- First place
-    Daniel Behrman    -- 374+    9942727/415417450   (average   155376069027/830419482550)
-    Sam Robb          -- 354+78061257357/79344732950 (average 28166096721657/158610121167050)
-    Jo Jorgensen      -- 343+57248246537/79344732950 (average 27272491648387/158610121167050)
-    John Monds        -- 191+25938757268/39672366475 (average  7603360753993/79305060583525)
-    Sorinne Ardeleanu -- 132+ 4476905049/79344732950 (average 10477981654449/158610121167050)
-    Brian Ellison     -- 117+ 3163925938/7934473295  (average   931497301453/15861012116705)
-    Arvin Vohra       -- 103+12570935257/39672366475 (average  4098824682182/79305060583525)
-    Kenneth Blevins   --  93+  746667503/11334961850 (average  1054898119553/22658588738150)
-    Phil Gray         --  90+20479941221/79344732950 (average  7161505906721/158610121167050)
-    Jedidiah Hill     --  78+46514107067/79344732950 (average  6235403277167/158610121167050)
-    Mark Whitney      --  72+  411932287/3173789318  (average   228924763183/6344404846682)
-    James Ogle        --  68+   47036982/39672366475 (average  2697767957282/79305060583525)
-    Steve Richey      --  62+36693850287/39672366475 (average  2496380571737/79305060583525)
-    Erik Gerhardt     --  61+ 2368624193/3173789318  (average   195969772591/6344404846682)
-    Keenan Dunham     --  59+ 8398712716/39672366475 (average  2349068334741/79305060583525)
-    Rhett Smith       --  58+ 5970470323/15868946590 (average   926369372543/31722024233410)
-    Louis Vanacore    --  51+ 8411482463/15868946590 (average   817727758553/31722024233410)
+    Adam Kokesh       -- 376+ 7396779449/79344732950 (average 29841016368649/230813828151550) -- First place
+    Daniel Behrman    -- 374+    9942727/415417450   (average   155376069027/1208449362050)
+    Sam Robb          -- 354+78061257357/79344732950 (average 28166096721657/230813828151550)
+    Jo Jorgensen      -- 343+57248246537/79344732950 (average 27272491648387/230813828151550)
+    John Monds        -- 191+25938757268/39672366475 (average  7603360753993/115406914075775)
+    Sorinne Ardeleanu -- 132+ 4476905049/79344732950 (average 10477981654449/230813828151550)
+    Brian Ellison     -- 117+ 3163925938/7934473295  (average   931497301453/23081382815155)
+    Arvin Vohra       -- 103+12570935257/39672366475 (average  4098824682182/115406914075775)
+    Kenneth Blevins   --  93+  746667503/11334961850 (average  1054898119553/32973404021650)
+    Phil Gray         --  90+20479941221/79344732950 (average  7161505906721/230813828151550)
+    Jedidiah Hill     --  78+46514107067/79344732950 (average  6235403277167/230813828151550)
+    Mark Whitney      --  72+  411932287/3173789318  (average   228924763183/9232553126062)
+    James Ogle        --  68+   47036982/39672366475 (average  2697767957282/115406914075775)
+    Steve Richey      --  62+36693850287/39672366475 (average  2496380571737/115406914075775)
+    Erik Gerhardt     --  61+ 2368624193/3173789318  (average   195969772591/9232553126062)
+    Keenan Dunham     --  59+ 8398712716/39672366475 (average  2349068334741/115406914075775)
+    Rhett Smith       --  58+ 5970470323/15868946590 (average   926369372543/46162765630310)
+    Louis Vanacore    --  51+ 8411482463/15868946590 (average   817727758553/46162765630310)
   Adam Kokesh wins a seat.
 [Allocated Score Voting: Winners]
   Adam Kokesh
   Jacob Hornberger
   Judge Jim Gray
   Justin Amash
   Vermin Supreme
```

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.csv` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_candidates.txt` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_presidential_poll_july_2020.txt` & `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt` & `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf` & `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt` & `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_fives_bloc_star.txt` & `starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_fives_star.txt` & `starvote-2.0.4/test_elections/test_election_all_fives_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_threes_bloc_star.txt` & `starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_threes_star.txt` & `starvote-2.0.4/test_elections/test_election_all_threes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_zeroes_bloc_star.txt` & `starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_all_zeroes_star.txt` & `starvote-2.0.4/test_elections/test_election_all_zeroes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.starvote` & `starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_bloc_star_and_electowiki.txt` & `starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote` & `starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt` & `starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_breakable_tie_for_second_in_score_round.txt` & `starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt` & `starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt` & `starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.starvote` & `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_1.txt` & `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.starvote` & `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_demonstrate_cloneproofness_2.txt` & `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_no_permuted_candidates_tiebreaker.txt` & `starvote-2.0.4/test_elections/bad_syntax_invalid_option.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-ValueError('tiebreaker list must not be empty')
+File 'test_elections/bad_syntax_invalid_option.starvote', Line 3: unknown option 'bafflegab'
 
 usage: starvote.py [options] <ballots_file>
 
 Tabulates an election based on votes in a CSV or starvote file.
 The parameters for the election can be inferred from the CSV filename,
 or explicitly specified via options.
 
 Options:
 
     -m|--method <method>
 
         Specifies the electoral system.
-        Supported methods are 'star', 'bloc', 'allocated', and 'rrv'.
+        Supported methods are 'star', 'bloc', 'allocated', 'rrv', and 'sss'.
 
     -r|--reference
 
         Adds the available reference implementations of methods.
         Continues even if any reference implementations are unavailable.
 
     -R|--force-reference
```

### Comparing `starvote-2.0.3/test_elections/test_election_only_two_candidates_rrv.txt` & `starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_only_two_candidates_star-pr.txt` & `starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-[Allocated Score Voting]
+[Sequentially Spent Score]
   Tabulating 5 ballots.
   Maximum score is 5.
   Want to fill 2 seats.
-  Hare quota is 5/2.
-[Allocated Score Voting: Initializing ordered permutation tiebreaker]
-  Permutation was defined in 'test_elections/test_election_only_two_candidates_star-pr.starvote'.
+  Hare score quota is 12+1/2.
+[Sequentially Spent Score: Initializing ordered permutation tiebreaker]
+  Permutation was defined in 'test_elections/test_election_only_two_candidates_sss.starvote'.
   Permuted list of candidates:
     1. Amy
     2. Becky
   Tiebreaker candidates will be selected from this list, preferring candidates with lower numbers.
-[Allocated Score Voting: Round 1]
+[Sequentially Spent Score: Round 1]
   There are exactly 2 candidates seeking 2 seats.  Every candidate wins.
```

### Comparing `starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.html` & `starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_reweighted_range_sample_election.txt` & `starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt` & `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt` & `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt` & `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 [Allocated Score Voting: Round 2: Ballot allocation round]
   Allocating 1 ballots.
 [Allocated Score Voting: Round 2: Ballot allocation round: Round 1]
   Allocating 1 ballot at score 10/3.
 [Allocated Score Voting: Round 3]
   Tabulating 2 remaining ballots.
   The highest-scoring candidate wins a seat.
-    Amy   -- 5+1/3 (average 2+2/3) -- First place
-    Brian -- 4     (average 2)
+    Amy   -- 5+1/3 (average 1+7/9) -- First place
+    Brian -- 4     (average 1+1/3)
   Amy wins a seat.
 [Allocated Score Voting: Winners]
   Amy
   Chuck
   Darcy
```

### Comparing `starvote-2.0.3/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt` & `starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt` & `starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_use_just_raise_tiebreaker.txt` & `starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/test_elections/test_election_use_no_description_tiebreaker.txt` & `starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/tests/harness.py` & `starvote-2.0.4/tests/harness.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/tests/run_tests.py` & `starvote-2.0.4/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/tools/is_ok` & `starvote-2.0.4/tools/is_ok`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/tools/remake_test_elections_output` & `starvote-2.0.4/tools/remake_test_elections_output`

 * *Files identical despite different names*

### Comparing `starvote-2.0.3/PKG-INFO` & `starvote-2.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,103 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 2.0.3
+Version: 2.0.4
 Summary: An election tabulator for the STAR electoral system, and others
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: numpy ; extra == "reference"
 Requires-Dist: pandas ; extra == "reference"
 Project-URL: Source, https://github.com/larryhastings/starvote/
 Provides-Extra: reference
 
 # starvote
 
-## A simple STAR Voting tabulator
+## A STAR Voting election tabulator
 
 ## Copyright 2023 by Larry Hastings
 
 [STAR voting](https://www.starvoting.org/) is a
-relatively-new [electoral system](https://en.wikipedia.org/wiki/Electoral_system).
-It's simple to vote and simple to tabulate.  While a completely fair and perfect
-electoral system is impossible, STAR Voting's approach makes reasonable tradeoffs
+relatively-new ["electoral system"](https://en.wikipedia.org/wiki/Electoral_system)--a
+method of running an election.  STAR Voting is simple--it's
+simple to vote, and simple to tabulate.  And while a completely
+fair and perfect electoral system is impossible,
+STAR Voting's approach makes sensible tradeoffs
 and avoids the worst pitfalls.  It's really great!
 
-This module, **starvote**, implements a simple STAR Voting tabulator.
+This module, **starvote**, implements a STAR Voting tabulator.
 It requires Python 3.7 or newer, but also supports CPython 3.6.
 (**starvote** relies on dictionaries preserving insertion order,
 which is guaranteed as of Python 3.7, but happened to work in CPython 3.6.)
 
 Features:
 
 * Supports four
   [electoral systems](https://en.wikipedia.org/wiki/Electoral_system):
 
   - [STAR Voting](https://www.starvoting.org/star), the snazzy
     new single-winner voting system.
   - [Bloc STAR Voting](https://www.starvoting.org/multi_winner),
-    a multi-winner variant of STAR voting that fills multiple
+    a multiwinner variant of STAR voting that fills multiple
     seats with the *most popular* candidates.
   - [Allocated Score Voting](https://electowiki.org/wiki/Allocated_Score),
     a [proportional representation](https://en.wikipedia.org/wiki/Proportional_representation)
     electoral system, and so far the only such system officially
     authorized to be a "Proportional STAR Voting" method.
   - [Reweighted Range Voting](https://rangevoting.org/RRV.html)
     (aka "RRV"), an alternative proportional representation
     electoral system.  RRV isn't a STAR variant, but like STAR
     it's a form of
     [score voting.](https://en.wikipedia.org/wiki/Score_voting)
     So the ballot and instructions to the voter are identical
     to a STAR-PR election.  The RRV algorithm is much simpler
     than Proportional STAR Voting, and its "never discard a voter"
     approach is appealing.
+  - [Sequentially Spent Score](https://electowiki.org/wiki/Sequentially_Spent_Score),
+    a third variety of score-based proportional representation
+    electoral system.
 
-* Implements the [Official Tiebreaker Protocol](https://www.starvoting.org/ties)
+* Implements the
+  [Official Tiebreaker Protocol](https://www.starvoting.org/ties)
   for STAR Voting and Bloc STAR Voting elections.
 
 * Provides a user-configurable final tiebreaker mechanism
   if the election (or one round in the election) ends in a tie.
 
   - The default tiebreaker mechanism randomly shuffles
     all the candidates in advance of running the election,
     then breaks the tie in favor of the candidate(s) that
     appear earliest in the list.
-  - Alternatively, you may choose to randomly pick a candidate
-    (or candidates) from the tied candidates, on demand.
+  - Alternatively, you can break ties by randomly picking
+    a candidate (or candidates) from the tied candidates,
+    on demand.
   - You can also implement your own custom tiebreaker.
-  - If you specify that there should be no tiebreaker, in
-    the event of an unbreakable tie the election will raise
-    an `UnbreakableTieError` exception.
+  - If you specify that there should be no tiebreaker,
+    and the election ends in an unbreakable tie, it will
+    raise an `UnbreakableTieError` exception.
 
 * All election tabulation calculations are performed using only integers
   and [fractions](https://docs.python.org/3/library/fractions.html).
-  This guarantees the calculations are 100% consistent and accurate
+  This guarantees results are 100% consistent and accurate
   across all platforms.  Floating-point rounding errors are
   impossible--because floats are never used!
 
 * Supports running elections specified in CSV files using
   [`https://star.vote/`](https://star.vote/) format.
 
-* Also supports running elections specified in a convenient custom
-  file format called *starvote format*.
+* Also supports running elections specified in
+  a convenient custom file format called *starvote format*.
 
-* *starvote* 2.0 passes its test suite with 100% coverage on
+* **starvote** 2.0.3 passes its test suite with 100% coverage on
   all supported versions.
 
-* *starvote* has no external dependencies.
+* **starvote** has no external dependencies.
 
 
 ## A quick STAR Voting primer
 
 When you vote using STAR Voting, your ballot looks something like this:
 
 ```
@@ -102,58 +109,67 @@
 
 To vote, give every candidate a score from 0 to 5.  5 means you like
 them the most, 0 means you like them the least.  (If you don't pick one
 of the scores, that's the same as a 0.)  If you give two candidates
 the same score, that means you like them equally--you don't have a
 preference between them.
 
-To figure out who won, you apply the **STAR** method: **S**core,
-**T**hen **A**utomatic **R**unoff.
+Tabulating the election is easy!  You apply the **STAR** method:
+**S**core, **T**hen **A**utomatic **R**unoff.
 
-In the first round, the score round, you add up the scores of all the
+In the first round, the *Scoring Round,* you add up the scores of all the
 candidates.  The top two scoring candidates automatically advance to
 the second round.
 
-In the second round, you examine every ballot to see which of the
-two remaining candidates they preferred.  If one has a higher score,
-that ballot prefers that candidate.  If the ballot scored both
-candidates the same, they have no preference.  The candidate that
-was preferred by more ballots wins the election.  It's that simple!
+In the second round, the *Automatic Runoff Round,* you examine every
+ballot to see which of the two remaining candidates they preferred.
+If one has a higher score, that ballot prefers that candidate.  If the
+ballot scored both candidates the same, they have no preference.
+The candidate preferred by more ballots wins the election.  It's that
+simple!
+
+And notice--you always examine every ballot.  STAR Voting never throws
+away ballots.  When you vote, your vote always matters,
+every step of the way.
 
 
 ## What's so good about STAR Voting?
 
 Electoral systems are a surprisingly deep topic.  They've been studied
-for hundreds of years, and there are many many different approaches.
+for hundreds of years, and there are many *many* different approaches.
 There are a number of desirable properties *and* undesirable properties
-that electoral systems can have.  And, bad news: it's impossible for
-there to be one best-possible voting system.  There are mutually
-exclusive desirable properties.  You can't make a one-size-fits-all
-system that avoids every problem.
+that electoral systems can have.  And here's the bad news: it's
+*impossible* for there to be one best-possible voting system.  There
+are mutually exclusive desirable properties, and there are desirable
+properties that bring with them downsides.  You just can't make a
+one-size-fits-all best system that avoids every problem--every electoral
+system has to be a compromise.  Wikipedia has
+[a comprehensive article](https://en.wikipedia.org/wiki/Comparison_of_electoral_systems)
+on the topic.
 
 STAR Voting avoid the worst problems of electoral systems.
 The remaining undesirable properties were chosen as the least-bad
 option.
 
-Here are some desirable properites STAR Voting displays:
+Here are some desirable properites STAR Voting has:
 
 * It's [monotonic.](https://en.wikipedia.org/wiki/Monotonicity_criterion)
   Giving a candidate a higher score can never hurt them, and
   giving a candidate a lower score can never help them.  (And yes,
   this is not always true of voting systems.  The increasingly popular
   [Instant Runoff Voting](https://en.wikipedia.org/wiki/Instant-runoff_voting)
   fails this; paradoxically, it's possible to *hurt* a candidate you
   prefer by giving them a *higher* score.)
 * It's [resolvable.](https://en.wikipedia.org/wiki/Resolvability_criterion)
   Ties are unlikely.
 * It complies with the [majority loser criterion.](https://en.wikipedia.org/wiki/Majority_loser_criterion)
   If a majority of candidates like one candidate the least, that candidate will
   never win a STAR Voting election.
 
-Here are some desirable properties STAR Voting doesn't have:
+But here are some desirable properties STAR Voting doesn't have:
 
 * It's not a [Condorcet method,](https://en.wikipedia.org/wiki/Condorcet_winner_criterion)
   which is a very particular property of an electoral system.
   Let's say you have an election with three candidates, A, B, and C.  You ask each voter
   to vote in three head-to-head races: "which do you like better, A or B?", "which do
   you like better, B or C?", and "which do you like better, A or C?"  If there's one
   candidate that wins in every such head-to-head vote in the election, they would be
@@ -175,62 +191,71 @@
   elected.  The STAR Voting team [wrote an essay on why they gave up on this criterion.](https://www.starvoting.org/pass_fail)
   The short version is: electoral systems that satisfy later-no-harm generally also
   exhibit
   [the spoiler effect,](https://en.wikipedia.org/wiki/Vote_splitting#%22Spoiler_effect%22)
   which is a worse property.  But achieving later-no-harm *and* avoiding the spoiler effect
   makes your electoral system even worse!
 
+(If there isn't a best-possible voting system, is there a worst-possible?  Maybe!
+If there *is* a worst electoral system, it's almost certainly
+[Plurality voting](https://en.wikipedia.org/wiki/Plurality_voting)...
+the predominant electoral system used here in the United States.  Sigh.)
+
 
 ## API
 
 ### `election`
 
-To use `starvote`, `import starvote`, then call the `election` method:
+To use `starvote`, first `import starvote`,
+then call its `election` function:
 
 ```Python
 def election(method, ballots, *,
     maximum_score=5,
     print=None,
     seats=1,
     verbosity=0,
     ):
 ```
 
-`election` tabulates an election based on your
-parameter and returns a `list` containing the
-winners. (Even for single-winner STAR Voting--in
+`election` tabulates an election based on the
+arguments you pass in and returns a `list` containing
+the winners. (Even for single-winner STAR Voting--in
 that case, the list will only contain one element.)
 
-`method` specifies which election system you want to use,
-via predefined `Method` objects. The allowed values are:
+`method` specifies which method (which "election system")
+you want to use in this election, via predefined `Method`
+objects. The supported values are:
 
 * `starvote.STAR_Voting`,
 * `starvote.Bloc_STAR_Voting`,
-* `starvote.Allocated_Score_Voting`, and
-* `starvote.Reweighted_Range_Voting`.
+* `starvote.Allocated_Score_Voting`,
+* `starvote.Reweighted_Range_Voting`, and
+* `starvote.Sequentially_Spent_Score`.
 
-Since those are a lot to
-type, `starvote` also provides nicknames, respectively:
+Since those are a lot to type, `starvote` also provides
+nicknames for these methods, respectively:
 
 * `starvote.star`,
 * `starvote.bloc`,
-* `starvote.allocated`, and
-* `starvote.rrv`.
+* `starvote.allocated`,
+* `starvote.rrv`, and
+* `starvote.sss`, and
 
 `ballots` should be an iterable containing individual ballots.
-Ballots are `dict` objects, mapping the candidate to that ballot's
-score for that candidate.  The candidate can be any Python value;
-the score must be an `int`.
+A ballot is a `dict` mapping the candidate to that ballot's
+score for that candidate.  The candidate can be any hashable
+Python value; the score must be an `int`.
 
-`maximum_score` specifies the maximum score allowed for any vote
-on any ballot.
+`maximum_score` specifies the maximum score allowed for
+any vote on any ballot.
 
 `seats` specifies how many seats the election should fill.
 STAR Voting is a single-winner method, so this should be
-`1` when using STAR Voting; for all the other methods,
+`1` when using STAR Voting; for the other methods,
 `seats` must be greater than or equal to `2`.
 
 `verbosity` specifies how much output you want.
 The current supported values are `0` (no output)
 and `1` (output); values higher than `1` are
 currently equivalent to `1`.
 
@@ -243,72 +268,79 @@
 
 ### Functions for specific electoral systems
 
 `starvote` also exports functions implementing each of
 the supported electoral systems:
 
 * `star_voting` implements single-winner STAR Voting.
-* `bloc_star_voting` implements multi-winner Bloc STAR Voting.
+* `bloc_star_voting` implements multiwinner Bloc STAR Voting.
 * `allocated_score_voting` implements Allocated Score Voting.
 * `reweighted_range_voting` implements Reweighted Range Voting.
+* `sequentially_spent_score` implements Sequentially Spent Score.
 
-These functions take much the same signature as `election`,
+These functions have much the same signature as `election`,
 with the following changes:
 
-* They don't take the `method` positional parameter;
-  the method is implicit in the function.  All four only
-  take one positional parameter, `ballots`, which is
-  required.
-* `star` doesn't take a `seats` parameter.  The other three
+* They don't have a `method` parameter; the method is implicit
+  in the function.  All four only take one positional parameter,
+  `ballots`, which is required.
+* `star` doesn't have a `seats` parameter.  The other three
   have a `seats` keyword-only parameter, and this parameter
-  is required--it doesn't have a default.  (A required
+  is required--it doesn't have a default.  (A *required*
   keyword-only parameter is pretty rare in Python!)
-* Note that these functions also always return a list,
-  even `star_voting`.
+* Note that, like `election`, these functions always
+  return a list, even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
 `starvote` ships a copy of the reference implementation
-of Allocated Score Voting.  Since this requires both NumPy
-and Pandas, it's not imported by default.  (I didn't want
+of Allocated Score Voting.  Since this requires both
+[NumPy](https://numpy.org/)
+and
+[Pandas](https://pandas.pydata.org/),
+it's not imported by default.  (I didn't want
 `starvote` to have any external dependencies.  The unit
 test suite runs correctly whether or not these external
 dependencies are installed.)
 
 You can import it with `import starvote.reference`;
 the directly-callable function is
 `starvote.reference.allocated_score_voting_reference`.
 You can also use the `Method` object
+`starvote.reference.Allocated_Score_Voting_reference`,
+with the nickname
+`starvote.reference.allocated_r`.
 
 If you want to integrate it into the `starvote` module,
 call`starvote.reference.monkey_patch()`.  This does
 three things:
 
-* Adds the function to the `starvote` module directly,
-  as `starvote.allocated_score_voting_reference`.
-* Adds it to `starvote.__all__` so that symbol
-  gets brought in by `from starvote import *`.
-*
+* Adds the function and `Method` objects to the `starvote`
+  module directly.
+
+  - Also adds them to `starvote.__all__` so they get
+    brought in by `from starvote import *`.
+
 * Adds the appropriate `Method` object
   to `starvote.methods`, using the name
   `'Allocated Score Voting (reference)'`
   and the nickname `allocated_r`.
 
 *Note:* the reference implementation doesn't support
 tiebreakers.  `allocated_score_voting_reference` *does*
 accept a `tiebreaker` argument, but currently it *must*
 be `None`.
 
 ### Ties
 
-The good news is, STAR Voting elections rarely result in a tie in the
-real world.  But ties can still happen.  The good news is, STAR Voting
-has a sensible, thorough protocol on how to break a tie.  The bad news is,
-not all ties are breakable--some ties genuinely represent the ambivalent
-will of the voters.
+STAR Voting elections rarely result in a tie in the real world.
+But ties can still happen.  The good news is, STAR Voting has a
+sensible, thorough protocol on how to break a tie.  The bad news is,
+not all ties are breakable--some ties genuinely represent the
+indecisive will of the voters.
 
 **starvote** gives you control over how to break ties in elections,
 through the `tiebreaker` parameter to `election` and the election-specific
 functions.  **starvote** also has two predefined tiebreaker functions,
 but you can substitute your own--or none at all.
 
 The default tiebreaker in **starvote** is
@@ -359,14 +391,22 @@
 
 If you pass in your own `candidates` list,
 you may also pass in a string for the
 `description` keyword-only parameter, which
 should be text describing the source of
 this ordered list of candidates.
 
+Note that, if you pass in your own
+`candidates` list, **starvote**'s tabulation
+of the election will be 100% deterministic
+and repeatable.  You can run that election
+a million times and you'll always get the
+same result.
+
+
 #### `on_demand_random_tiebreaker`
 
 If you prefer more unpredictability in your life,
 you can choose `on_demand_random_tiebreaker`
 to break ties.  `on_demand_random_tiebreaker` will
 simply pick a random candidate (or candidates)
 on demand, using Python's `random.sample` function.
@@ -562,17 +602,19 @@
 
 The `options` section specifies how to run the election.
 Assignment lines in the `options` section specify options;
 each name maps to a parameter to the `election` function.
 Here are all the supported names:
 
 ```
+    csv_path = <string>
     maximum score = <integer>
     method = <string>
     seats = <integer>
+    starvote_path = <string>
     tiebreaker = <string | list>
     verbosity = <integer>
 ```
 
 A *starvote format election* can specify each of these a maximum of once.
 
 An assignment line in the `options` section can also use
@@ -588,15 +630,16 @@
 
 * If you set a value to `[]`, it's set to an empty
   list, and the parser doesn't enable *list mode.*
 * You can't use pragmas or change sections while
   in *list mode.*
 * You can't nest lists.
 
-The only option that supports lists is `tiebreaker`.
+The only assignment that supports lists is the
+`tiebreaker` option in the `options` section.
 If `tiebreaker` is set to a string, this specifies
 the name of the tiebreaker in the `starvote.tiebreakers`
 dict to use for this election.  If `tiebreaker` is set
 to a string, `parse_starvote` looks up that string in
 the `options.tiebreakers` dict and uses the tiebreaker
 found there.  If `tiebreaker` is set
 to a list, this defines a pre-permuted list of candidates
@@ -626,14 +669,25 @@
 ```
     5 ballots:
 ```
 
 (You're explicitly permitted to have blank lines between the
 `ballots` pragma and the ballot it's repeating.)
 
+The `starvote_path` and `csv_path` options allow you to
+"import" another file into the current election.  They
+can specify relative or absolute paths; if relative,
+they will be resolved using the directory the *starvote
+format* file is in (if the *starvote format election* was
+loaded from a file) or the current directory.  Both settings
+will load ballots from the file specified; `starvote_path`
+will also load the options from the file specified, however
+any options set in the current election will override those
+options.
+
 #### Example
 
 Here's a sample starvote format election:
 
     [options]
 
     seats=3
@@ -705,66 +759,172 @@
 You may specify the text encoding using the
 `encoding` keyword-only parameter; the default
 encoding is `'utf-8'`.
 
 
 ### Command-line module
 
-The `starvote` module supports being run as a script (`python -m starvote`).
+The `starvote` module supports being run as a script
+(`python -m starvote`).
 Run it without arguments to see usage.
 
 To use, specify the path to a single file on the
 command-line.  `starvote` will read in the file,
 run the election, and print the result.
 
 The path may be a
 [CSV file.](https://en.wikipedia.org/wiki/Comma-separated_values)
 CSV files should end with the file extension `.csv`,
 and be in
 [`https://star.vote/`](https://star.vote/)
 format.  By default elections in CSV files are run
-using STAR Voting.
+using STAR Voting, for one seat, with `verbosity=1`
+and the default tiebreaker.
 
 Alternatively, the path may be a *starvote format* file.
-*starvote format* files should end with the file extension `.starvote`
-and contain a *starvote format election* in UTF-8 format.
+*starvote format* files should end with the file extension
+`.starvote` and contain a *starvote format election* in
+UTF-8 format.  *starvote format elections* explicitly
+specify all the parameters of the election.
 
 For example, you can run this from the root of the
 source-code repository:
 
 ```
 % python3 -m starvote test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
 ```
 
 to see how **starvote** handles ties during the automatic runoff round.
 
 
 ## Multiple-winner elections
 
-**starvote** also implements several multi-winner electoral systems:
-
-Simply instantiate your `Poll` object passing in the enum constant
-`starvote.Bloc_STAR`, `starvote.Proportional_STAR`,
-or `starvote.Reweighted_Range`
-for the `electoral_system` parameter, and the number of seats in
-the `seats` keyword-only parameter:
+**starvote** also implements several multiwinner electoral systems.
+All you need to do is pass in one of the multiwinner methods, such as
+`starvote.bloc`, `starvote.allocated`,
+or `starvote.rrv`, when you call `election`:
 
 ```Python
-poll = starvote.Poll(electoral_system=starvote.Bloc_STAR, seats=2)
+poll = election(starvote.bloc, ballots, seats=2)
 ```
 
 You can experiment with these with the command-line version of the
-module, too.  You can specify the electoral system with `-e`,
+module too.  Simply specify the method with `-m`,
 the number of seats with `-s`,
-and the maximum score with `-m`:
+and the maximum score with `-x`.
+These will override the settings from inside a *starvote format* file
+(and the default settings for CSV files).
+
+### Multiwinner vs proportional
+
+Here's a quick explanation about what "proportional voting" means,
+in the context of multiwinner elections.
+As with every other topic, you can read more about it
+[at Wikipedia.](https://en.wikipedia.org/wiki/Proportional_representation)
+
+A straight multiwinner election simply means you're electing
+2 or more candidates instead of one candidate.  The candidates
+that get the most votes--or however the election is tabulated--win.
+
+But electing only the most popular candidates can be a poor
+representation of the electorate.  Let's say you have a city
+election to fill five seats.  In this city, 60% of the voters
+vote only for party A, and 40% of the voters vote only for
+party B.  Bloc STAR Voting would very likely award all five
+seats to party A candidates.  Is that fair?  It seems like the
+["tyranny of the majority".](https://en.wikipedia.org/wiki/Tyranny_of_the_majority)
+
+There's an alternate approach to apportioning seats, used
+in political systems across the world, called "Proportional
+Representation".  The idea is, you have N seats, and you
+assign portions of them based on representing portions of
+the populace.  In the above example, you'd *want* to give
+three seats to party A and two seats to party B.  What
+system could do that?
+
+Often proportional representation is done based on voting
+for parties rather than voting for candidates.  This is
+called
+[Party-list proportional representation,](https://en.wikipedia.org/wiki/Party-list_proportional_representation)
+and it's used to elect governmental bodies across the world.
+
+But there are voting methods that permit voting directly for
+candidates and produces proportional representation.
+Allocated Score Voting, Reweighted Range Voting, and
+Sequentially Spent Score are three such methods.
+They all work something like this:
+
+* Each vote is a number, with higher numbers
+  indicating a stronger preference.
+* You run N rounds of the election to fill N seats,
+  each round electing one candidate.
+* When a candidate is elected, we may *allocate* ballots
+  to that candidate, which means we consider them used-up
+  and we remove them from the election.  If you vote
+  for candidate A1, and candidate A1 wins the first round,
+  your ballot might get "allocated" to candidate A1 and
+  ignored for the rest of the election.
+* Alternatively, we may *re-weigh* the
+  ballots of voters who voted for that candidate.
+  That means we reduce the voting power of those ballots.
+  If in the election, you voted for candidate A1, and A1
+  wins the first round, in the second round your vote
+  will count for less.  But if I gave A1 a score of 0,
+  my ballot would still be at full strength.
+
+The differences between the three is how they allocate
+vs. reweigh ballots. Allocated Score Voting and Sequentially
+Spent Score both allocate ballots, Reweighted Range Voting
+never does--with RRV every vote is counted in every round.
+Also, the three systems use different formulae to compute the
+new weight of a ballot after each round.  In Allocated Score
+and Sequentially Spent Score,
+the new weight is based on how many excess voters were needed
+to fill a quota (called a
+[Hare quota](https://en.wikipedia.org/wiki/Hare_quota));
+in Reweighted Range Voting, the new weight is based on the
+sum of the score(s) you contribute to the winning candidate(s).
+
+**starvote** ships a sample election that nicely demonstrates
+how direct-elected proportional representation elections can work:
+
+```
+test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+This election is like the example election I used in the description
+above.  It uses Reweighted Range Voting to fill three seats, and each
+vote has a maximum score of 10.
+60 of the voters prefer party A, and give high scores to candidates A1, A2, and A3;
+40 of the voters prefer party B, and give high scores to candidates B1 and B2.
+
+You can run the election in the `starvote` main directory with this command:
 
 ```
 % python3 -m starvote test_elections/test_election_reweighted_range_sample_election.starvote
 ```
 
+To see how the tabulation works using Allocated Score Voting, run this:
+
+```
+% python3 -m starvote -m allocated test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+You can also see how it changes with Sequentially Spent Score by running this:
+
+```
+% python3 -m starvote -m allocated test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
+And to see the tyrrany of the majority in action, this command will tabulate the election using Bloc STAR Voting:
+
+```
+% python3 -m starvote -m bloc test_elections/test_election_reweighted_range_sample_election.starvote
+```
+
 ### Warning
 
 I haven't found a single test corpus for Bloc STAR Voting.
 I'm following the rules as best I can, and the results I'm getting
 make sense.  But so far I can't confirm my implementation is
 correct--there's a very real possibility I got something wrong.
 
@@ -778,15 +938,16 @@
 ## Thanks
 
 Huge thanks to Tim Peters for his continuous input during the
 development of this library.  Although Tim didn't have any input
 on the library itself--if you don't like the library it's 100%
 my fault!--he tirelessly answered all my questions about voting
 during its development, and convinced me to change my approach
-several times.
+several times.  In particular, Tim's feedback pushed me to
+develop the `tiebreaker` plug-in interface.
 
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
@@ -804,15 +965,31 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
-**2.0.3** - *2023/05/27*
+**2.0.4** - *2023/06/05*
+
+* Added support for Sequentially Spent Score voting.
+* Changed presentation slightly for Allocated Score:
+  the average vote is now computed using the count of
+  *all* ballots in the election, including allocated
+  ballots.  (Previously the average was computing using
+  just the *remaining* ballots.)  This doesn't change
+  the outcome of the election, it's just a presentation
+  change.
+* Removed last traces of "STAR-PR", which I thought was
+  an alternate name for Allocated Score.
+* Doc changes.  Standardized on the spelling "multiwinner",
+  instead of "multi-winner".
+
+
+**2.0.3** - *2023/06/01*
 
 * Normalized nomenclature for `Method` objects.  Now,
   every method has an official correctly-spelled
   correctly-capitalized name, and exactly one "nickname".
   The nickname is always lowercase, and would return
   True for `isidentifier`.  These are used in the
   `starvote.method` map; a variant of these names is
@@ -820,27 +997,27 @@
   valid identifiers).
 * Improved `starvote.reference.monkey_patch`.  It's now
   data-driven and thus more reliable.
 * Added `starvote.reference.__all__`, in case you want
   to `from starvote.reference import *`.
 * Doc fixes.
 
-**2.0.2** - *2023/05/27*
+**2.0.2** - *2023/06/01*
 
 * Renamed the `tiebreaker` parameter `candidates` to `tie`.
 * Evicted some testing-only tiebreakers from the `starvote`
   module.  They're now in their own script, which only gets
   loaded when working with the test suite.
 
-**2.0.1** - *2023/05/27*
+**2.0.1** - *2023/06/01*
 
 * Changed the nickname of the reference version of
   Allocated Score Voting to "Allocated-R".
 
-**2.0** - *2023/05/27*
+**2.0** - *2023/06/01*
 
 A complete rewrite!  The 1.x code base was pretty smelly.
 This codebase is much, much cleaner--and I think I squashed
 one or two bugs too.
 
 `starvote` has an entirely new, functional API. `election`
 runs the election for you, and takes two required positional
@@ -850,15 +1027,15 @@
 
 You can also now pass in a handler for unbreakable ties.
 By default, unbreakable ties are now broken using a
 pre-chosen randomize list of candidates.  (`election` can
 still raise `UnbreakableTieError` exceptions if you prefer.)
 
 You can also call the voting method functions directly:
-`star`, `bloc_star`, `proportional_star`, and `reweighted_range`
+`star`, `bloc_star`, `proportional_star`, `reweighted_range`,
 are all functions, too.  These omit the `method` parameter
 but still require the `ballots` parameter.
 
 There's also a new text format for storing an election,
 *starvote format,* with the `.starvote` file extension.
 *starvote format* is a nice alternative to `.csv` files.
```


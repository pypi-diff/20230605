# Comparing `tmp/flat_api-0.8.1.tar.gz` & `tmp/flat_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flat_api-0.8.1.tar", last modified: Wed Mar 23 20:00:48 2022, max compression
+gzip compressed data, was "flat_api-1.0.0.tar", last modified: Mon Jun  5 17:15:23 2023, max compression
```

## Comparing `flat_api-0.8.1.tar` & `flat_api-1.0.0.tar`

### file list

```diff
@@ -1,252 +1,303 @@
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.158304 flat_api-0.8.1/
--rw-r--r--   0 gierschv   (501) staff       (20)    11357 2022-03-22 16:00:07.000000 flat_api-0.8.1/LICENSE
--rw-r--r--   0 gierschv   (501) staff       (20)    25052 2022-03-23 20:00:48.157807 flat_api-0.8.1/PKG-INFO
--rw-r--r--   0 gierschv   (501) staff       (20)    23973 2022-03-23 19:57:07.000000 flat_api-0.8.1/README.md
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.008458 flat_api-0.8.1/flat_api/
--rw-r--r--   0 gierschv   (501) staff       (20)     9991 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/__init__.py
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.014064 flat_api-0.8.1/flat_api/api/
--rw-r--r--   0 gierschv   (501) staff       (20)      463 2022-03-23 19:48:16.000000 flat_api-0.8.1/flat_api/api/__init__.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7114 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/account_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)   189723 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/class_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)    65970 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/collection_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)    17975 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/group_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)    79574 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/organization_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)   208155 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/score_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7455 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/task_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)    19360 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api/user_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)    27788 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/api_client.py
--rw-r--r--   0 gierschv   (501) staff       (20)    14407 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/configuration.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5379 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/exceptions.py
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.065759 flat_api-0.8.1/flat_api/models/
--rw-r--r--   0 gierschv   (501) staff       (20)     9221 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/__init__.py
--rw-r--r--   0 gierschv   (501) staff       (20)     9083 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/api_access_token.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5505 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/app_scopes.py
--rw-r--r--   0 gierschv   (501) staff       (20)    19341 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5874 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_canvas.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7374 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_copy.py
--rw-r--r--   0 gierschv   (501) staff       (20)    20361 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5210 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_creation_google_classroom.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5239 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_creation_microsoft_graph.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4902 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_lti.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5850 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_mfc.py
--rw-r--r--   0 gierschv   (501) staff       (20)    18315 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10042 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_comment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5323 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_comment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10287 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_history.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6051 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_history_attachment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4504 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)    11486 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6053 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_submission_update_comments.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4601 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/assignment_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)    11266 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_attachment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6332 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)    20368 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5779 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_canvas.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10855 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_clever.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6038 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_google_classroom.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6650 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_google_drive.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5085 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_issues.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6947 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_issues_sync.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6781 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_lti.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5886 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_mfc.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5042 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_details_microsoft_graph.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4405 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_roles.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4441 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6138 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/class_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)    14170 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6232 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_app.py
--rw-r--r--   0 gierschv   (501) staff       (20)     9566 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_capabilities.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6510 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6246 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_modification.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4400 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_privacy.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4565 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/collection_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7231 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/flat_error_response.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4715 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/flat_locales.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7608 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/google_classroom_coursework.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6843 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/google_classroom_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10403 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/group.py
--rw-r--r--   0 gierschv   (501) staff       (20)     9693 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/group_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4470 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/group_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4397 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/license_mode.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4571 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/license_sources.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4609 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/lms_name.py
--rw-r--r--   0 gierschv   (501) staff       (20)    11460 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/lti_credentials.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6191 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/lti_credentials_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)    23070 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/media_attachment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4503 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/media_score_sharing_mode.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7720 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/microsoft_graph_assignment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6789 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/microsoft_graph_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10276 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_invitation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6108 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_invitation_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4484 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_roles.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5394 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_user_access_token_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6021 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_user_signin_link.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5368 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/organization_user_signin_link_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)    14523 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/resource_collaborator.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10618 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/resource_collaborator_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     8777 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/resource_rights.py
--rw-r--r--   0 gierschv   (501) staff       (20)    17505 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comment.py
--rw-r--r--   0 gierschv   (501) staff       (20)    11725 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comment_context.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10008 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6312 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comment_moderation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     9054 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comment_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7513 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_comments_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)    14160 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6166 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation_builder_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)    13008 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation_builder_data_layout_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10575 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation_builder_data_score_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)     8454 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation_builder_data_score_data_instruments.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4475 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_creation_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)    32071 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5302 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_fork.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4632 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_license.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6592 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_likes_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)    14327 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_modification.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6572 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_plays_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4521 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_privacy.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10556 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_revision.py
--rw-r--r--   0 gierschv   (501) staff       (20)     9001 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_revision_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6077 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_revision_statistics.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5423 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_source.py
--rw-r--r--   0 gierschv   (501) staff       (20)    13555 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track.py
--rw-r--r--   0 gierschv   (501) staff       (20)     8154 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7350 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track_point.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4458 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4484 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7447 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_track_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     6572 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/score_views_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10067 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/task.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5044 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/task_export_options.py
--rw-r--r--   0 gierschv   (501) staff       (20)     5707 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/task_progress.py
--rw-r--r--   0 gierschv   (501) staff       (20)    10735 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_admin_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)    11776 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)    27245 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)    18404 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_details_admin.py
--rw-r--r--   0 gierschv   (501) staff       (20)     8046 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_details_admin_license.py
--rw-r--r--   0 gierschv   (501) staff       (20)    23806 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_public.py
--rw-r--r--   0 gierschv   (501) staff       (20)    16066 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/models/user_public_summary.py
--rw-r--r--   0 gierschv   (501) staff       (20)    13905 2022-03-23 20:00:08.000000 flat_api-0.8.1/flat_api/rest.py
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.009774 flat_api-0.8.1/flat_api.egg-info/
--rw-r--r--   0 gierschv   (501) staff       (20)    25052 2022-03-23 20:00:47.000000 flat_api-0.8.1/flat_api.egg-info/PKG-INFO
--rw-r--r--   0 gierschv   (501) staff       (20)     8665 2022-03-23 20:00:48.000000 flat_api-0.8.1/flat_api.egg-info/SOURCES.txt
--rw-r--r--   0 gierschv   (501) staff       (20)        1 2022-03-23 20:00:47.000000 flat_api-0.8.1/flat_api.egg-info/dependency_links.txt
--rw-r--r--   0 gierschv   (501) staff       (20)       48 2022-03-23 20:00:47.000000 flat_api-0.8.1/flat_api.egg-info/requires.txt
--rw-r--r--   0 gierschv   (501) staff       (20)        9 2022-03-23 20:00:47.000000 flat_api-0.8.1/flat_api.egg-info/top_level.txt
--rw-r--r--   0 gierschv   (501) staff       (20)       38 2022-03-23 20:00:48.158448 flat_api-0.8.1/setup.cfg
--rw-r--r--   0 gierschv   (501) staff       (20)     1996 2022-03-23 19:59:54.000000 flat_api-0.8.1/setup.py
-drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2022-03-23 20:00:48.157213 flat_api-0.8.1/test/
--rw-r--r--   0 gierschv   (501) staff       (20)        0 2022-03-23 19:48:16.000000 flat_api-0.8.1/test/__init__.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2441 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_account_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2482 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_api_access_token.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2440 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_app_scopes.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2446 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2496 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_canvas.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_copy.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2512 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2636 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_creation_google_classroom.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2628 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_creation_microsoft_graph.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_lti.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_mfc.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2528 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2586 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_comment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2652 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_comment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2586 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_history.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2668 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_history_attachment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2570 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2578 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2644 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_submission_update_comments.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_assignment_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7023 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2554 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_attachment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2514 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_canvas.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2514 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_clever.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2588 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_google_classroom.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2556 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_google_drive.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2514 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_issues.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2548 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_issues_sync.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2490 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_lti.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2490 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_mfc.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2580 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_details_microsoft_graph.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2448 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_roles.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2448 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2456 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_class_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2446 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection.py
--rw-r--r--   0 gierschv   (501) staff       (20)     3747 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_app.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2544 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_capabilities.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2512 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2544 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_modification.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2504 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_privacy.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_collection_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2506 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_flat_error_response.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2456 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_flat_locales.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2570 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_google_classroom_coursework.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2570 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_google_classroom_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2406 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_group.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2711 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_group_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_group_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2440 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_group_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2456 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_license_mode.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_license_sources.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2424 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_lms_name.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_lti_credentials.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2546 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_lti_credentials_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2488 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_media_attachment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2540 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_media_score_sharing_mode.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2562 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_microsoft_graph_assignment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2562 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_microsoft_graph_submission.py
--rw-r--r--   0 gierschv   (501) staff       (20)     4713 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2544 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_invitation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2610 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_invitation_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2504 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_roles.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2654 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_user_access_token_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2580 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_user_signin_link.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2646 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_organization_user_signin_link_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2528 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_resource_collaborator.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2594 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_resource_collaborator_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2480 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_resource_rights.py
--rw-r--r--   0 gierschv   (501) staff       (20)     7027 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comment.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2522 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comment_context.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2530 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comment_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2546 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comment_moderation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2514 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comment_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2522 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_comments_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2564 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation_builder_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2648 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation_builder_data_layout_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2640 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation_builder_data_score_data.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2730 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation_builder_data_score_data_instruments.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2506 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_creation_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2440 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_fork.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_license.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2498 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_likes_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2504 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_modification.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2498 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_plays_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_privacy.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2472 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_revision.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2538 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_revision_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2554 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_revision_statistics.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2456 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_source.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2448 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2514 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2490 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track_point.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2490 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track_state.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2482 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track_type.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2498 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_track_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2498 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_score_views_counts.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2398 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_task.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2389 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_task_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2506 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_task_export_options.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_task_progress.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2490 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_admin_update.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2683 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_api.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2464 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_creation.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2456 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_details.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2498 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_details_admin.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2556 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_details_admin_license.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2448 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_public.py
--rw-r--r--   0 gierschv   (501) staff       (20)     2506 2022-03-23 19:19:40.000000 flat_api-0.8.1/test/test_user_public_summary.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.864352 flat_api-1.0.0/
+-rw-r--r--   0 gierschv   (501) staff       (20)    11357 2022-03-22 16:00:07.000000 flat_api-1.0.0/LICENSE
+-rw-r--r--   0 gierschv   (501) staff       (20)    28925 2023-06-05 17:15:23.864451 flat_api-1.0.0/PKG-INFO
+-rw-r--r--   0 gierschv   (501) staff       (20)    27866 2023-06-05 17:14:21.000000 flat_api-1.0.0/README.md
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.808687 flat_api-1.0.0/flat_api/
+-rw-r--r--   0 gierschv   (501) staff       (20)     2313 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/__init__.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.811415 flat_api-1.0.0/flat_api/api/
+-rw-r--r--   0 gierschv   (501) staff       (20)      212 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/__init__.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     7523 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/account_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)   170985 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/class_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    58819 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/collection_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    63444 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/edu_resources_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18241 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/group_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    77065 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/organization_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)   183653 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/score_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     7514 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/task_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18587 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api/user_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    40684 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/api_client.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.811613 flat_api-1.0.0/flat_api/apis/
+-rw-r--r--   0 gierschv   (501) staff       (20)      856 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/apis/__init__.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18090 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/configuration.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     6693 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/exceptions.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.842276 flat_api-1.0.0/flat_api/model/
+-rw-r--r--   0 gierschv   (501) staff       (20)      342 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/model/__init__.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14807 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/api_access_token.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16295 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/app_scopes.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18483 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14687 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_copy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18801 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_copy_response.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15302 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_copy_response_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13574 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_copy_response_capabilities_can_publish_in_class_error.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18976 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14752 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_comment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13185 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_comment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16601 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_history.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13688 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_history_attachment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13886 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_history_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13767 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15918 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13490 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_submission_update_comments.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14048 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    17991 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/assignment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    24006 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13413 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_canvas.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13063 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_lti.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13416 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_mfc.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    21265 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13245 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_update_google_classroom.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13239 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_assignment_update_microsoft_graph.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16512 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_attachment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14630 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    20891 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13405 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_canvas.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15473 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_clever.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13463 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_google_classroom.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13661 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_google_drive.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13409 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_issues.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13831 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_issues_sync_inner.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13621 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_lti.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13419 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_mfc.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13123 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_details_microsoft_graph.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13857 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_grade_level.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13692 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_roles.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13720 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14568 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/class_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    17546 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13488 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_app.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15143 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13679 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13615 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_modification.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13837 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14444 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/collection_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14243 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_library.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16516 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14040 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13471 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_copy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14119 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13471 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_move.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13428 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18332 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_resource.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13683 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13167 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13661 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_resource_use_in_class.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13499 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/edu_skills_focused.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13978 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/flat_error_response.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14107 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/flat_locales.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14060 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/google_classroom_coursework.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13778 2023-06-05 17:14:13.000000 flat_api-1.0.0/flat_api/model/google_classroom_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15466 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/group.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14960 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/group_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13771 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/group_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13595 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/license_mode.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13880 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/license_sources.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14067 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/lms_name.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15538 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/lti_credentials.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13548 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/lti_credentials_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    20845 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/media_attachment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13657 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/media_score_sharing_mode.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14077 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/microsoft_graph_assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13737 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/microsoft_graph_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15150 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/organization_invitation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13645 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/organization_invitation_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13867 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/organization_roles.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13409 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/organization_user_access_token_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18055 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/resource_collaborator.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15568 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/resource_collaborator_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15626 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/resource_rights.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18368 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15273 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comment_context.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15476 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13596 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comment_moderation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14909 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14072 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_comments_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18376 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13995 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation_builder_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15888 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation_builder_data_layout_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15656 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation_builder_data_score_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14635 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation_builder_data_score_data_instruments_inner.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13853 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_creation_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    24849 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14155 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_fork.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14504 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_license.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13689 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_likes_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16684 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_modification.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13669 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_plays_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18472 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15331 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_revision.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15067 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_revision_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14168 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_revision_statistics.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13429 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_source.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16695 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14423 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13923 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track_point.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13415 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13806 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14200 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_track_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13669 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/score_views_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16331 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/task.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13113 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/task_export_options.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13342 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/task_progress.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13307 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/task_result.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14954 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_admin_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13683 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_azure_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14804 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_community_profile_links.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15441 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    22202 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    18172 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_details_admin.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    14335 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_details_admin_license.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    20097 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_public.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    16871 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_public_summary.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13389 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_signin_link.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    13276 2023-06-05 17:14:14.000000 flat_api-1.0.0/flat_api/model/user_signin_link_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    84105 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/model_utils.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.842471 flat_api-1.0.0/flat_api/models/
+-rw-r--r--   0 gierschv   (501) staff       (20)     9132 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/models/__init__.py
+-rw-r--r--   0 gierschv   (501) staff       (20)    15891 2023-06-05 17:14:15.000000 flat_api-1.0.0/flat_api/rest.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.809488 flat_api-1.0.0/flat_api.egg-info/
+-rw-r--r--   0 gierschv   (501) staff       (20)    28925 2023-06-05 17:15:23.000000 flat_api-1.0.0/flat_api.egg-info/PKG-INFO
+-rw-r--r--   0 gierschv   (501) staff       (20)    10447 2023-06-05 17:15:23.000000 flat_api-1.0.0/flat_api.egg-info/SOURCES.txt
+-rw-r--r--   0 gierschv   (501) staff       (20)        1 2023-06-05 17:15:23.000000 flat_api-1.0.0/flat_api.egg-info/dependency_links.txt
+-rw-r--r--   0 gierschv   (501) staff       (20)       48 2023-06-05 17:15:23.000000 flat_api-1.0.0/flat_api.egg-info/requires.txt
+-rw-r--r--   0 gierschv   (501) staff       (20)        9 2023-06-05 17:15:23.000000 flat_api-1.0.0/flat_api.egg-info/top_level.txt
+-rw-r--r--   0 gierschv   (501) staff       (20)      651 2023-06-05 17:04:33.000000 flat_api-1.0.0/pyproject.toml
+-rw-r--r--   0 gierschv   (501) staff       (20)       69 2023-06-05 17:15:23.864743 flat_api-1.0.0/setup.cfg
+-rw-r--r--   0 gierschv   (501) staff       (20)     2008 2023-06-05 17:14:41.000000 flat_api-1.0.0/setup.py
+drwxr-xr-x   0 gierschv   (501) staff       (20)        0 2023-06-05 17:15:23.864208 flat_api-1.0.0/test/
+-rw-r--r--   0 gierschv   (501) staff       (20)     2335 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_account_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2447 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_api_access_token.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2328 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_app_scopes.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2729 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2363 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_copy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2815 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_copy_response.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2783 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_copy_response_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2664 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_copy_response_capabilities_can_publish_in_class_error.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2952 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2455 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_comment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2512 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_comment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2829 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_history.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2526 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_history_attachment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2491 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_history_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2441 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2773 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2505 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_submission_update_comments.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2363 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2620 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_assignment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     6981 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3556 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2413 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_canvas.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2392 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_lti.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2392 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_mfc.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3040 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2520 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_update_google_classroom.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2513 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_assignment_update_microsoft_graph.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2560 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_attachment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2576 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3778 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2392 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_canvas.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2392 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_clever.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2456 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_google_classroom.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2428 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_google_drive.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2550 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_issues.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2457 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_issues_sync_inner.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_lti.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_mfc.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2449 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_details_microsoft_graph.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_grade_level.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2335 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_roles.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2335 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2562 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_class_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3132 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3638 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2356 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_app.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2419 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2506 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2534 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_modification.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2384 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2363 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_collection_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2335 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_library.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2834 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2427 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_capabilities.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_copy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2507 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_move.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2392 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2794 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_resource.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2385 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2415 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resource_use_in_class.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     4118 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_resources_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2378 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_edu_skills_focused.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2385 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_flat_error_response.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2342 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_flat_locales.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2441 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_google_classroom_coursework.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2441 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_google_classroom_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2299 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_group.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2607 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_group_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2432 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_group_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2328 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_group_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2342 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_license_mode.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2363 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_license_sources.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2314 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_lms_name.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2438 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_lti_credentials.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2495 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_lti_credentials_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2503 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_media_attachment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2414 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_media_score_sharing_mode.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2434 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_microsoft_graph_assignment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2434 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_microsoft_graph_submission.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     4602 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_organization_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2534 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_organization_invitation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2591 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_organization_invitation_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2384 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_organization_roles.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2596 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_organization_user_access_token_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2558 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_resource_collaborator.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2462 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_resource_collaborator_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2363 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_resource_rights.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     6923 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2609 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comment.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2399 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comment_context.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2530 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comment_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2420 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comment_moderation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2516 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comment_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2399 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_comments_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2687 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2805 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation_builder_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2507 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation_builder_data_layout_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2749 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation_builder_data_score_data.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2614 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation_builder_data_score_data_instruments_inner.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2385 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_creation_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     3461 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2328 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_fork.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2349 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_license.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2378 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_likes_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2690 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_modification.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2378 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_plays_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2349 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_privacy.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2496 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_revision.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2413 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_revision_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2427 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_revision_statistics.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2342 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_source.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2655 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2608 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track_point.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2371 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track_state.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2364 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track_type.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2594 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_track_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2378 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_score_views_counts.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2474 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_task.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2286 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_task_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2385 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_task_export_options.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2349 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_task_progress.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2335 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_task_result.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2486 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_admin_update.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2580 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_api.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2378 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_azure_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2442 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_community_profile_links.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2440 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_creation.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2896 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_details.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2721 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_details_admin.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2622 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_details_admin_license.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2686 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_public.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2587 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_public_summary.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2364 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_signin_link.py
+-rw-r--r--   0 gierschv   (501) staff       (20)     2421 2023-06-05 13:15:49.000000 flat_api-1.0.0/test/test_user_signin_link_creation.py
```

### Comparing `flat_api-0.8.1/LICENSE` & `flat_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flat_api-0.8.1/PKG-INFO` & `flat_api-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,33 @@
-Metadata-Version: 2.1
-Name: flat_api
-Version: 0.8.1
-Summary: Flat API Client
-Home-page: https://github.com/FlatIO/api-client-python
-Author: The Flat Team (https://flat.io)
-Author-email: developers@flat.io
-License: Apache
-Keywords: Flat API,MusicXML,Music Notation,MIDI
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Artistic Software
-Classifier: Topic :: Education
-Classifier: Topic :: Multimedia :: Sound/Audio
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Client for the Flat REST API
 
-[![Python package](https://github.com/FlatIO/api-client-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/FlatIO/api-client-python/actions/workflows/python-package.yml)
+[![Python package](https://github.com/FlatIO/api-client-python/actions/workflows/python.yml/badge.svg)](https://github.com/FlatIO/api-client-python/actions/workflows/python.yml)
 
 The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:
 - Creating and importing new music scores using MusicXML or MIDI files
 - Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI)
 - Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.
 
 You can find the API reference including code samples and our OpenAPI Specification at the following url: [https://flat.io/developers/api/reference](https://flat.io/developers/api/reference).
 
 To request some API credentials, please visit [https://flat.io/developers](https://flat.io/developers).
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python >= 3.7
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install flat_api
 ```
 
+or install from this repository
+
 ```sh
 pip install git+https://github.com/FlatIO/api-client-python.git
 ```
 
 Then import the package:
 ```python
 import flat_api
@@ -75,60 +48,58 @@
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from __future__ import print_function
-import time
-import flat_api
-from flat_api.rest import ApiException
 from pprint import pprint
+import flat_api
+from flat_api.api import account_api
 
-# Configure OAuth2 access token for authorization: OAuth2
-configuration = flat_api.Configuration()
-configuration.access_token = 'YOUR_ACCESS_TOKEN'
-
-# create an instance of the API class
-api_instance = flat_api.AccountApi(flat_api.ApiClient(configuration))
-only_id = False # bool | Only return the user id (optional) (default to False)
-
-try:
-    # Get current user profile
-    api_response = api_instance.get_authenticated_user(only_id=only_id)
-    pprint(api_response)
-except ApiException as e:
-    print("Exception when calling AccountApi->get_authenticated_user: %s\n" % e)
-
+configuration = flat_api.Configuration(
+    access_token = 'YOUR_ACCESS_TOKEN'
+)
+
+# Enter a context with an instance of the API client
+with flat_api.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = account_api.AccountApi(api_client)
+
+    try:
+        # Get current user account
+        api_response = api_instance.get_authenticated_user()
+        pprint(api_response)
+    except flat_api.ApiException as e:
+        print("Exception when calling AccountApi->get_authenticated_user: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.flat.io/v2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AccountApi* | [**get_authenticated_user**](docs/AccountApi.md#get_authenticated_user) | **GET** /me | Get current user profile
+*AccountApi* | [**get_authenticated_user**](docs/AccountApi.md#get_authenticated_user) | **GET** /me | Get current user account
 *ClassApi* | [**activate_class**](docs/ClassApi.md#activate_class) | **POST** /classes/{class}/activate | Activate the class
 *ClassApi* | [**add_class_user**](docs/ClassApi.md#add_class_user) | **PUT** /classes/{class}/users/{user} | Add a user to the class
 *ClassApi* | [**archive_assignment**](docs/ClassApi.md#archive_assignment) | **POST** /classes/{class}/assignments/{assignment}/archive | Archive the assignment
 *ClassApi* | [**archive_class**](docs/ClassApi.md#archive_class) | **POST** /classes/{class}/archive | Archive the class
 *ClassApi* | [**copy_assignment**](docs/ClassApi.md#copy_assignment) | **POST** /classes/{class}/assignments/{assignment}/copy | Copy an assignment
-*ClassApi* | [**create_assignment**](docs/ClassApi.md#create_assignment) | **POST** /classes/{class}/assignments | Assignment creation
 *ClassApi* | [**create_class**](docs/ClassApi.md#create_class) | **POST** /classes | Create a new class
+*ClassApi* | [**create_class_assignment**](docs/ClassApi.md#create_class_assignment) | **POST** /classes/{class}/assignments | Assignment creation
 *ClassApi* | [**create_submission**](docs/ClassApi.md#create_submission) | **PUT** /classes/{class}/assignments/{assignment}/submissions | Create or edit a submission
+*ClassApi* | [**create_test_student_account**](docs/ClassApi.md#create_test_student_account) | **POST** /classes/{class}/testStudent | Create a test student account
 *ClassApi* | [**delete_class_user**](docs/ClassApi.md#delete_class_user) | **DELETE** /classes/{class}/users/{user} | Remove a user from the class
-*ClassApi* | [**delete_submission**](docs/ClassApi.md#delete_submission) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission} | Delete a submission
+*ClassApi* | [**delete_submission**](docs/ClassApi.md#delete_submission) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission} | Reset a submission
 *ClassApi* | [**delete_submission_comment**](docs/ClassApi.md#delete_submission_comment) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission}/comments/{comment} | Delete a feedback comment to a submission
 *ClassApi* | [**edit_submission**](docs/ClassApi.md#edit_submission) | **PUT** /classes/{class}/assignments/{assignment}/submissions/{submission} | Edit a submission
 *ClassApi* | [**enroll_class**](docs/ClassApi.md#enroll_class) | **POST** /classes/enroll/{enrollmentCode} | Join a class
 *ClassApi* | [**export_submissions_reviews_as_csv**](docs/ClassApi.md#export_submissions_reviews_as_csv) | **GET** /classes/{class}/assignments/{assignment}/submissions/csv | CSV Grades exports
 *ClassApi* | [**export_submissions_reviews_as_excel**](docs/ClassApi.md#export_submissions_reviews_as_excel) | **GET** /classes/{class}/assignments/{assignment}/submissions/excel | Excel Grades exports
-*ClassApi* | [**fork_score**](docs/ClassApi.md#fork_score) | **POST** /scores/{score}/fork | Fork a score
 *ClassApi* | [**get_class**](docs/ClassApi.md#get_class) | **GET** /classes/{class} | Get the details of a single class
 *ClassApi* | [**get_score_submissions**](docs/ClassApi.md#get_score_submissions) | **GET** /scores/{score}/submissions | List submissions related to the score
 *ClassApi* | [**get_submission**](docs/ClassApi.md#get_submission) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission} | Get a student submission
 *ClassApi* | [**get_submission_comments**](docs/ClassApi.md#get_submission_comments) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission}/comments | List the feedback comments of a submission
 *ClassApi* | [**get_submission_history**](docs/ClassApi.md#get_submission_history) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission}/history | Get the history of the submission
 *ClassApi* | [**get_submissions**](docs/ClassApi.md#get_submissions) | **GET** /classes/{class}/assignments/{assignment}/submissions | List the students&#39; submissions
 *ClassApi* | [**list_assignments**](docs/ClassApi.md#list_assignments) | **GET** /classes/{class}/assignments | Assignments listing
@@ -144,14 +115,25 @@
 *CollectionApi* | [**delete_collection**](docs/CollectionApi.md#delete_collection) | **DELETE** /collections/{collection} | Delete the collection
 *CollectionApi* | [**delete_score_from_collection**](docs/CollectionApi.md#delete_score_from_collection) | **DELETE** /collections/{collection}/scores/{score} | Delete a score from the collection
 *CollectionApi* | [**edit_collection**](docs/CollectionApi.md#edit_collection) | **PUT** /collections/{collection} | Update a collection&#39;s metadata
 *CollectionApi* | [**get_collection**](docs/CollectionApi.md#get_collection) | **GET** /collections/{collection} | Get collection details
 *CollectionApi* | [**list_collection_scores**](docs/CollectionApi.md#list_collection_scores) | **GET** /collections/{collection}/scores | List the scores contained in a collection
 *CollectionApi* | [**list_collections**](docs/CollectionApi.md#list_collections) | **GET** /collections | List the collections
 *CollectionApi* | [**untrash_collection**](docs/CollectionApi.md#untrash_collection) | **POST** /collections/{collection}/untrash | Untrash a collection
+*EduResourcesApi* | [**copy_edu_resource**](docs/EduResourcesApi.md#copy_edu_resource) | **POST** /eduResources/{resource}/copy | Copy an education resource to a Resource Library
+*EduResourcesApi* | [**copy_edu_resource_to_demo_class**](docs/EduResourcesApi.md#copy_edu_resource_to_demo_class) | **POST** /eduResources/{resource}/copyToDemoClass | Copy an education assignment to a teacher demo class
+*EduResourcesApi* | [**create_edu_resource**](docs/EduResourcesApi.md#create_edu_resource) | **POST** /eduResources | Create a new education resource
+*EduResourcesApi* | [**delete_edu_resource**](docs/EduResourcesApi.md#delete_edu_resource) | **DELETE** /eduResources/{resource} | Delete an education resource
+*EduResourcesApi* | [**get_edu_resource**](docs/EduResourcesApi.md#get_edu_resource) | **GET** /eduResources/{resource} | Get an education resource
+*EduResourcesApi* | [**list_edu_libraries**](docs/EduResourcesApi.md#list_edu_libraries) | **GET** /eduResources/libraries | List the education libraries
+*EduResourcesApi* | [**list_edu_resources**](docs/EduResourcesApi.md#list_edu_resources) | **GET** /eduResources | List education resources in a library or folder
+*EduResourcesApi* | [**move_edu_resource**](docs/EduResourcesApi.md#move_edu_resource) | **POST** /eduResources/{resource}/move | Move an education resource
+*EduResourcesApi* | [**update_edu_resource**](docs/EduResourcesApi.md#update_edu_resource) | **PUT** /eduResources/{resource} | Update an education resource metadata
+*EduResourcesApi* | [**update_edu_resource_assignment**](docs/EduResourcesApi.md#update_edu_resource_assignment) | **PUT** /eduResources/{resource}/assignment | Update an education resource assignment
+*EduResourcesApi* | [**use_edu_resource_in_class**](docs/EduResourcesApi.md#use_edu_resource_in_class) | **POST** /eduResources/{resource}/useInClass | Use an education resource in a class
 *GroupApi* | [**get_group_details**](docs/GroupApi.md#get_group_details) | **GET** /groups/{group} | Get group information
 *GroupApi* | [**get_group_scores**](docs/GroupApi.md#get_group_scores) | **GET** /groups/{group}/scores | List group&#39;s scores
 *GroupApi* | [**list_group_users**](docs/GroupApi.md#list_group_users) | **GET** /groups/{group}/users | List group&#39;s users
 *OrganizationApi* | [**count_orga_users**](docs/OrganizationApi.md#count_orga_users) | **GET** /organizations/users/count | Count the organization users using the provided filters
 *OrganizationApi* | [**create_lti_credentials**](docs/OrganizationApi.md#create_lti_credentials) | **POST** /organizations/lti/credentials | Create a new couple of LTI 1.x credentials
 *OrganizationApi* | [**create_organization_invitation**](docs/OrganizationApi.md#create_organization_invitation) | **POST** /organizations/invitations | Create a new invitation to join the organization
 *OrganizationApi* | [**create_organization_user**](docs/OrganizationApi.md#create_organization_user) | **POST** /organizations/users | Create a new user account
@@ -201,52 +183,71 @@
 
 
 ## Documentation For Models
 
  - [ApiAccessToken](docs/ApiAccessToken.md)
  - [AppScopes](docs/AppScopes.md)
  - [Assignment](docs/Assignment.md)
- - [AssignmentCanvas](docs/AssignmentCanvas.md)
  - [AssignmentCopy](docs/AssignmentCopy.md)
- - [AssignmentCreation](docs/AssignmentCreation.md)
- - [AssignmentCreationGoogleClassroom](docs/AssignmentCreationGoogleClassroom.md)
- - [AssignmentCreationMicrosoftGraph](docs/AssignmentCreationMicrosoftGraph.md)
- - [AssignmentLti](docs/AssignmentLti.md)
- - [AssignmentMfc](docs/AssignmentMfc.md)
+ - [AssignmentCopyResponse](docs/AssignmentCopyResponse.md)
+ - [AssignmentCopyResponseCapabilities](docs/AssignmentCopyResponseCapabilities.md)
+ - [AssignmentCopyResponseCapabilitiesCanPublishInClassError](docs/AssignmentCopyResponseCapabilitiesCanPublishInClassError.md)
  - [AssignmentSubmission](docs/AssignmentSubmission.md)
  - [AssignmentSubmissionComment](docs/AssignmentSubmissionComment.md)
  - [AssignmentSubmissionCommentCreation](docs/AssignmentSubmissionCommentCreation.md)
  - [AssignmentSubmissionHistory](docs/AssignmentSubmissionHistory.md)
  - [AssignmentSubmissionHistoryAttachment](docs/AssignmentSubmissionHistoryAttachment.md)
+ - [AssignmentSubmissionHistoryState](docs/AssignmentSubmissionHistoryState.md)
  - [AssignmentSubmissionState](docs/AssignmentSubmissionState.md)
  - [AssignmentSubmissionUpdate](docs/AssignmentSubmissionUpdate.md)
  - [AssignmentSubmissionUpdateComments](docs/AssignmentSubmissionUpdateComments.md)
  - [AssignmentType](docs/AssignmentType.md)
+ - [AssignmentUpdate](docs/AssignmentUpdate.md)
+ - [ClassAssignment](docs/ClassAssignment.md)
+ - [ClassAssignmentCanvas](docs/ClassAssignmentCanvas.md)
+ - [ClassAssignmentLti](docs/ClassAssignmentLti.md)
+ - [ClassAssignmentMfc](docs/ClassAssignmentMfc.md)
+ - [ClassAssignmentUpdate](docs/ClassAssignmentUpdate.md)
+ - [ClassAssignmentUpdateGoogleClassroom](docs/ClassAssignmentUpdateGoogleClassroom.md)
+ - [ClassAssignmentUpdateMicrosoftGraph](docs/ClassAssignmentUpdateMicrosoftGraph.md)
  - [ClassAttachmentCreation](docs/ClassAttachmentCreation.md)
  - [ClassCreation](docs/ClassCreation.md)
  - [ClassDetails](docs/ClassDetails.md)
  - [ClassDetailsCanvas](docs/ClassDetailsCanvas.md)
  - [ClassDetailsClever](docs/ClassDetailsClever.md)
  - [ClassDetailsGoogleClassroom](docs/ClassDetailsGoogleClassroom.md)
  - [ClassDetailsGoogleDrive](docs/ClassDetailsGoogleDrive.md)
  - [ClassDetailsIssues](docs/ClassDetailsIssues.md)
- - [ClassDetailsIssuesSync](docs/ClassDetailsIssuesSync.md)
+ - [ClassDetailsIssuesSyncInner](docs/ClassDetailsIssuesSyncInner.md)
  - [ClassDetailsLti](docs/ClassDetailsLti.md)
  - [ClassDetailsMfc](docs/ClassDetailsMfc.md)
  - [ClassDetailsMicrosoftGraph](docs/ClassDetailsMicrosoftGraph.md)
+ - [ClassGradeLevel](docs/ClassGradeLevel.md)
  - [ClassRoles](docs/ClassRoles.md)
  - [ClassState](docs/ClassState.md)
  - [ClassUpdate](docs/ClassUpdate.md)
  - [Collection](docs/Collection.md)
  - [CollectionApp](docs/CollectionApp.md)
  - [CollectionCapabilities](docs/CollectionCapabilities.md)
  - [CollectionCreation](docs/CollectionCreation.md)
  - [CollectionModification](docs/CollectionModification.md)
  - [CollectionPrivacy](docs/CollectionPrivacy.md)
  - [CollectionType](docs/CollectionType.md)
+ - [EduLibrary](docs/EduLibrary.md)
+ - [EduResource](docs/EduResource.md)
+ - [EduResourceCapabilities](docs/EduResourceCapabilities.md)
+ - [EduResourceCopy](docs/EduResourceCopy.md)
+ - [EduResourceCreation](docs/EduResourceCreation.md)
+ - [EduResourceMove](docs/EduResourceMove.md)
+ - [EduResourcePrivacy](docs/EduResourcePrivacy.md)
+ - [EduResourceResource](docs/EduResourceResource.md)
+ - [EduResourceType](docs/EduResourceType.md)
+ - [EduResourceUpdate](docs/EduResourceUpdate.md)
+ - [EduResourceUseInClass](docs/EduResourceUseInClass.md)
+ - [EduSkillsFocused](docs/EduSkillsFocused.md)
  - [FlatErrorResponse](docs/FlatErrorResponse.md)
  - [FlatLocales](docs/FlatLocales.md)
  - [GoogleClassroomCoursework](docs/GoogleClassroomCoursework.md)
  - [GoogleClassroomSubmission](docs/GoogleClassroomSubmission.md)
  - [Group](docs/Group.md)
  - [GroupDetails](docs/GroupDetails.md)
  - [GroupType](docs/GroupType.md)
@@ -259,30 +260,28 @@
  - [MediaScoreSharingMode](docs/MediaScoreSharingMode.md)
  - [MicrosoftGraphAssignment](docs/MicrosoftGraphAssignment.md)
  - [MicrosoftGraphSubmission](docs/MicrosoftGraphSubmission.md)
  - [OrganizationInvitation](docs/OrganizationInvitation.md)
  - [OrganizationInvitationCreation](docs/OrganizationInvitationCreation.md)
  - [OrganizationRoles](docs/OrganizationRoles.md)
  - [OrganizationUserAccessTokenCreation](docs/OrganizationUserAccessTokenCreation.md)
- - [OrganizationUserSigninLink](docs/OrganizationUserSigninLink.md)
- - [OrganizationUserSigninLinkCreation](docs/OrganizationUserSigninLinkCreation.md)
  - [ResourceCollaborator](docs/ResourceCollaborator.md)
  - [ResourceCollaboratorCreation](docs/ResourceCollaboratorCreation.md)
  - [ResourceRights](docs/ResourceRights.md)
  - [ScoreComment](docs/ScoreComment.md)
  - [ScoreCommentContext](docs/ScoreCommentContext.md)
  - [ScoreCommentCreation](docs/ScoreCommentCreation.md)
  - [ScoreCommentModeration](docs/ScoreCommentModeration.md)
  - [ScoreCommentUpdate](docs/ScoreCommentUpdate.md)
  - [ScoreCommentsCounts](docs/ScoreCommentsCounts.md)
  - [ScoreCreation](docs/ScoreCreation.md)
  - [ScoreCreationBuilderData](docs/ScoreCreationBuilderData.md)
  - [ScoreCreationBuilderDataLayoutData](docs/ScoreCreationBuilderDataLayoutData.md)
  - [ScoreCreationBuilderDataScoreData](docs/ScoreCreationBuilderDataScoreData.md)
- - [ScoreCreationBuilderDataScoreDataInstruments](docs/ScoreCreationBuilderDataScoreDataInstruments.md)
+ - [ScoreCreationBuilderDataScoreDataInstrumentsInner](docs/ScoreCreationBuilderDataScoreDataInstrumentsInner.md)
  - [ScoreCreationType](docs/ScoreCreationType.md)
  - [ScoreDetails](docs/ScoreDetails.md)
  - [ScoreFork](docs/ScoreFork.md)
  - [ScoreLicense](docs/ScoreLicense.md)
  - [ScoreLikesCounts](docs/ScoreLikesCounts.md)
  - [ScoreModification](docs/ScoreModification.md)
  - [ScorePlaysCounts](docs/ScorePlaysCounts.md)
@@ -297,21 +296,26 @@
  - [ScoreTrackState](docs/ScoreTrackState.md)
  - [ScoreTrackType](docs/ScoreTrackType.md)
  - [ScoreTrackUpdate](docs/ScoreTrackUpdate.md)
  - [ScoreViewsCounts](docs/ScoreViewsCounts.md)
  - [Task](docs/Task.md)
  - [TaskExportOptions](docs/TaskExportOptions.md)
  - [TaskProgress](docs/TaskProgress.md)
+ - [TaskResult](docs/TaskResult.md)
  - [UserAdminUpdate](docs/UserAdminUpdate.md)
+ - [UserAzureDetails](docs/UserAzureDetails.md)
+ - [UserCommunityProfileLinks](docs/UserCommunityProfileLinks.md)
  - [UserCreation](docs/UserCreation.md)
  - [UserDetails](docs/UserDetails.md)
  - [UserDetailsAdmin](docs/UserDetailsAdmin.md)
  - [UserDetailsAdminLicense](docs/UserDetailsAdminLicense.md)
  - [UserPublic](docs/UserPublic.md)
  - [UserPublicSummary](docs/UserPublicSummary.md)
+ - [UserSigninLink](docs/UserSigninLink.md)
+ - [UserSigninLinkCreation](docs/UserSigninLinkCreation.md)
 
 
 ## Documentation For Authorization
 
 
 ## OAuth2
 
@@ -324,14 +328,16 @@
  - **account.education_profile**: Provides access to the basic person's education profile and public organization information. 
  - **scores.readonly**: Allows read-only access to all a user's scores. You won't need this scope to read public scores. 
  - **scores.social**: Allow to post comments and like scores 
  - **scores**: Full, permissive scope to access all of a user's scores. 
  - **collections.readonly**: Allow read-only access to a user's collections.
  - **collections.add_scores**: Allow to add scores to a user's collections.
  - **collections**: Full, permissive scope to access all of a user's collections.
+ - **edu.resources**: Read-write access to the resource library.
+ - **edu.resources.readonly**: Read-only access to the resource library.
  - **edu.classes**: Full, permissive scope to manage the classes.
  - **edu.classes.readonly**: Read-only access to the classes.
  - **edu.assignments**: Read-write access to the assignments and submissions.
  - **edu.assignments.readonly**: Read-only access to the assignments and submissions.
  - **edu.admin**: Full, permissive scope to manage all the admin of an organization.
  - **edu.admin.lti**: Access and manage the LTI Credentials for an organization.
  - **edu.admin.lti.readonly**: Read-only access to the LTI Credentials of an organization.
@@ -341,9 +347,26 @@
 
 
 ## Author
 
 developers@flat.io
 
 
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in flat_api.apis and flat_api.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from flat_api.api.default_api import DefaultApi`
+- `from flat_api.model.pet import Pet`
 
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import flat_api
+from flat_api.apis import *
+from flat_api.models import *
+```
```

### Comparing `flat_api-0.8.1/flat_api/api/account_api.py` & `flat_api-1.0.0/flat_api/api/task_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,174 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import re  # noqa: F401
+import sys  # noqa: F401
 
-# python 2 and python 3 compatibility library
-import six
-
-from flat_api.api_client import ApiClient
-from flat_api.exceptions import (  # noqa: F401
-    ApiTypeError,
-    ApiValueError
+from flat_api.api_client import ApiClient, Endpoint as _Endpoint
+from flat_api.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
 )
+from flat_api.model.flat_error_response import FlatErrorResponse
+from flat_api.model.task import Task
 
 
-class AccountApi(object):
+class TaskApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.get_task_endpoint = _Endpoint(
+            settings={
+                'response_type': (Task,),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/tasks/{task}',
+                'operation_id': 'get_task',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'task',
+                ],
+                'required': [
+                    'task',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'task':
+                        (str,),
+                },
+                'attribute_map': {
+                    'task': 'task',
+                },
+                'location_map': {
+                    'task': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
 
-    def get_authenticated_user(self, **kwargs):  # noqa: E501
-        """Get current user profile  # noqa: E501
+    def get_task(
+        self,
+        task,
+        **kwargs
+    ):
+        """Get a task details  # noqa: E501
 
-        Get details about the current authenticated User.   # noqa: E501
+        This method can be used to follow a task progression, for example while a score is being exported.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_authenticated_user(async_req=True)
-        >>> result = thread.get()
 
-        :param async_req bool: execute request asynchronously
-        :param bool only_id: Only return the user id
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: UserDetails
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_authenticated_user_with_http_info(**kwargs)  # noqa: E501
-
-    def get_authenticated_user_with_http_info(self, **kwargs):  # noqa: E501
-        """Get current user profile  # noqa: E501
-
-        Get details about the current authenticated User.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_authenticated_user_with_http_info(async_req=True)
+        >>> thread = api.get_task(task, async_req=True)
         >>> result = thread.get()
 
-        :param async_req bool: execute request asynchronously
-        :param bool only_id: Only return the user id
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(UserDetails, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
+        Args:
+            task (str): Unique identifier for the task
 
-        local_var_params = locals()
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Task
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['task'] = \
+            task
+        return self.get_task_endpoint.call_with_http_info(**kwargs)
 
-        all_params = [
-            'only_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_authenticated_user" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'only_id' in local_var_params and local_var_params['only_id'] is not None:  # noqa: E501
-            query_params.append(('onlyId', local_var_params['only_id']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['OAuth2']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/me', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='UserDetails',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `flat_api-0.8.1/flat_api/api/user_api.py` & `flat_api-1.0.0/flat_api/api/user_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,388 +1,454 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import re  # noqa: F401
+import sys  # noqa: F401
 
-# python 2 and python 3 compatibility library
-import six
-
-from flat_api.api_client import ApiClient
-from flat_api.exceptions import (  # noqa: F401
-    ApiTypeError,
-    ApiValueError
+from flat_api.api_client import ApiClient, Endpoint as _Endpoint
+from flat_api.model_utils import (  # noqa: F401
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_and_convert_types
 )
+from flat_api.model.flat_error_response import FlatErrorResponse
+from flat_api.model.score_details import ScoreDetails
+from flat_api.model.user_public import UserPublic
 
 
 class UserApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.ger_user_likes_endpoint = _Endpoint(
+            settings={
+                'response_type': ([ScoreDetails],),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/users/{user}/likes',
+                'operation_id': 'ger_user_likes',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'user',
+                    'ids',
+                ],
+                'required': [
+                    'user',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'user':
+                        (str,),
+                    'ids':
+                        (bool,),
+                },
+                'attribute_map': {
+                    'user': 'user',
+                    'ids': 'ids',
+                },
+                'location_map': {
+                    'user': 'path',
+                    'ids': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_user_endpoint = _Endpoint(
+            settings={
+                'response_type': (UserPublic,),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/users/{user}',
+                'operation_id': 'get_user',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'user',
+                ],
+                'required': [
+                    'user',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'user':
+                        (str,),
+                },
+                'attribute_map': {
+                    'user': 'user',
+                },
+                'location_map': {
+                    'user': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_user_scores_endpoint = _Endpoint(
+            settings={
+                'response_type': ([ScoreDetails],),
+                'auth': [
+                    'OAuth2'
+                ],
+                'endpoint_path': '/users/{user}/scores',
+                'operation_id': 'get_user_scores',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'user',
+                    'parent',
+                ],
+                'required': [
+                    'user',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'user':
+                        (str,),
+                    'parent':
+                        (str,),
+                },
+                'attribute_map': {
+                    'user': 'user',
+                    'parent': 'parent',
+                },
+                'location_map': {
+                    'user': 'path',
+                    'parent': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
 
-    def ger_user_likes(self, user, **kwargs):  # noqa: E501
+    def ger_user_likes(
+        self,
+        user,
+        **kwargs
+    ):
         """List liked scores  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
+
         >>> thread = api.ger_user_likes(user, async_req=True)
         >>> result = thread.get()
 
-        :param async_req bool: execute request asynchronously
-        :param str user: Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user.  (required)
-        :param bool ids: Return only the identifiers of the scores
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: list[ScoreDetails]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.ger_user_likes_with_http_info(user, **kwargs)  # noqa: E501
+        Args:
+            user (str): Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user. 
 
-    def ger_user_likes_with_http_info(self, user, **kwargs):  # noqa: E501
-        """List liked scores  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.ger_user_likes_with_http_info(user, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str user: Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user.  (required)
-        :param bool ids: Return only the identifiers of the scores
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(list[ScoreDetails], status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
+        Keyword Args:
+            ids (bool): Return only the identifiers of the scores. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [ScoreDetails]
+                If the method is called asynchronously, returns the request
+                thread.
         """
-
-        local_var_params = locals()
-
-        all_params = [
-            'user',
-            'ids'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method ger_user_likes" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'user' is set
-        if self.api_client.client_side_validation and ('user' not in local_var_params or  # noqa: E501
-                                                        local_var_params['user'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `user` when calling `ger_user_likes`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'user' in local_var_params:
-            path_params['user'] = local_var_params['user']  # noqa: E501
-
-        query_params = []
-        if 'ids' in local_var_params and local_var_params['ids'] is not None:  # noqa: E501
-            query_params.append(('ids', local_var_params['ids']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['OAuth2']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/users/{user}/likes', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[ScoreDetails]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def get_user(self, user, **kwargs):  # noqa: E501
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['user'] = \
+            user
+        return self.ger_user_likes_endpoint.call_with_http_info(**kwargs)
+
+    def get_user(
+        self,
+        user,
+        **kwargs
+    ):
         """Get a public user profile  # noqa: E501
 
         Get a profile of a Flat or Flat for Education User.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
+
         >>> thread = api.get_user(user, async_req=True)
         >>> result = thread.get()
 
-        :param async_req bool: execute request asynchronously
-        :param str user: This route parameter is the unique identifier of the user. You can specify an email instead of an unique identifier. If you are executing this request authenticated, you can use `me` as a value instead of the current User unique identifier to work on the current authenticated user.  (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: UserPublic
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_user_with_http_info(user, **kwargs)  # noqa: E501
-
-    def get_user_with_http_info(self, user, **kwargs):  # noqa: E501
-        """Get a public user profile  # noqa: E501
-
-        Get a profile of a Flat or Flat for Education User.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_user_with_http_info(user, async_req=True)
-        >>> result = thread.get()
+        Args:
+            user (str): This route parameter is the unique identifier of the user. You can specify an email instead of an unique identifier. If you are executing this request authenticated, you can use `me` as a value instead of the current User unique identifier to work on the current authenticated user. 
 
-        :param async_req bool: execute request asynchronously
-        :param str user: This route parameter is the unique identifier of the user. You can specify an email instead of an unique identifier. If you are executing this request authenticated, you can use `me` as a value instead of the current User unique identifier to work on the current authenticated user.  (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(UserPublic, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            UserPublic
+                If the method is called asynchronously, returns the request
+                thread.
         """
-
-        local_var_params = locals()
-
-        all_params = [
-            'user'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_user" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'user' is set
-        if self.api_client.client_side_validation and ('user' not in local_var_params or  # noqa: E501
-                                                        local_var_params['user'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `user` when calling `get_user`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'user' in local_var_params:
-            path_params['user'] = local_var_params['user']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['OAuth2']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/users/{user}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='UserPublic',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def get_user_scores(self, user, **kwargs):  # noqa: E501
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['user'] = \
+            user
+        return self.get_user_endpoint.call_with_http_info(**kwargs)
+
+    def get_user_scores(
+        self,
+        user,
+        **kwargs
+    ):
         """List user's scores  # noqa: E501
 
         Get the list of public scores owned by a User.  **DEPRECATED**: Please note that the current behavior will be deprecrated on **2019-01-01**. This method will no longer list private and shared scores, but only public scores of a Flat account. If you want to access to private scores, please use the [Collections API](#tag/Collection) instead.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
+
         >>> thread = api.get_user_scores(user, async_req=True)
         >>> result = thread.get()
 
-        :param async_req bool: execute request asynchronously
-        :param str user: Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user.  (required)
-        :param str parent: Filter the score forked from the score id `parent`
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: list[ScoreDetails]
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_user_scores_with_http_info(user, **kwargs)  # noqa: E501
-
-    def get_user_scores_with_http_info(self, user, **kwargs):  # noqa: E501
-        """List user's scores  # noqa: E501
-
-        Get the list of public scores owned by a User.  **DEPRECATED**: Please note that the current behavior will be deprecrated on **2019-01-01**. This method will no longer list private and shared scores, but only public scores of a Flat account. If you want to access to private scores, please use the [Collections API](#tag/Collection) instead.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_user_scores_with_http_info(user, async_req=True)
-        >>> result = thread.get()
+        Args:
+            user (str): Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user. 
 
-        :param async_req bool: execute request asynchronously
-        :param str user: Unique identifier of a Flat user. If you authenticated, you can use `me` to refer to the current user.  (required)
-        :param str parent: Filter the score forked from the score id `parent`
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(list[ScoreDetails], status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
+        Keyword Args:
+            parent (str): Filter the score forked from the score id `parent`. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [ScoreDetails]
+                If the method is called asynchronously, returns the request
+                thread.
         """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['user'] = \
+            user
+        return self.get_user_scores_endpoint.call_with_http_info(**kwargs)
 
-        local_var_params = locals()
-
-        all_params = [
-            'user',
-            'parent'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_user_scores" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'user' is set
-        if self.api_client.client_side_validation and ('user' not in local_var_params or  # noqa: E501
-                                                        local_var_params['user'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `user` when calling `get_user_scores`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'user' in local_var_params:
-            path_params['user'] = local_var_params['user']  # noqa: E501
-
-        query_params = []
-        if 'parent' in local_var_params and local_var_params['parent'] is not None:  # noqa: E501
-            query_params.append(('parent', local_var_params['parent']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['OAuth2']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/users/{user}/scores', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[ScoreDetails]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
```

### Comparing `flat_api-0.8.1/flat_api/api_client.py` & `flat_api-1.0.0/flat_api/api_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-# coding: utf-8
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
-from __future__ import absolute_import
 
-import atexit
-import datetime
-from dateutil.parser import parse
 import json
+import atexit
 import mimetypes
 from multiprocessing.pool import ThreadPool
+import io
 import os
 import re
-import tempfile
+import typing
+from urllib.parse import quote
+from urllib3.fields import RequestField
 
-# python 2 and python 3 compatibility library
-import six
-from six.moves.urllib.parse import quote
 
-from flat_api.configuration import Configuration
-import flat_api.models
 from flat_api import rest
-from flat_api.exceptions import ApiValueError, ApiException
+from flat_api.configuration import Configuration
+from flat_api.exceptions import ApiTypeError, ApiValueError, ApiException
+from flat_api.model_utils import (
+    ModelNormal,
+    ModelSimple,
+    ModelComposed,
+    check_allowed_values,
+    check_validations,
+    date,
+    datetime,
+    deserialize_file,
+    file_type,
+    model_to_dict,
+    none_type,
+    validate_and_convert_types
+)
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -49,25 +58,14 @@
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
     :param pool_threads: The number of threads to use for async requests
         to the API. More threads means more concurrent API requests.
     """
 
-    PRIMITIVE_TYPES = (float, bool, bytes, six.text_type) + six.integer_types
-    NATIVE_TYPES_MAPPING = {
-        'int': int,
-        'long': int if six.PY3 else long,  # noqa: F821
-        'float': float,
-        'str': str,
-        'bool': bool,
-        'date': datetime.date,
-        'datetime': datetime.datetime,
-        'object': object,
-    }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
                  cookie=None, pool_threads=1):
         if configuration is None:
             configuration = Configuration.get_default_copy()
         self.configuration = configuration
@@ -76,15 +74,14 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'flat_api/1.0.0'
-        self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -115,19 +112,34 @@
     def user_agent(self, value):
         self.default_headers['User-Agent'] = value
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
-            self, resource_path, method, path_params=None,
-            query_params=None, header_params=None, body=None, post_params=None,
-            files=None, response_type=None, auth_settings=None,
-            _return_http_data_only=None, collection_formats=None,
-            _preload_content=True, _request_timeout=None, _host=None):
+        self,
+        resource_path: str,
+        method: str,
+        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        body: typing.Optional[typing.Any] = None,
+        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
+        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
+        auth_settings: typing.Optional[typing.List[str]] = None,
+        _return_http_data_only: typing.Optional[bool] = None,
+        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
+        _preload_content: bool = True,
+        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
+        _host: typing.Optional[str] = None,
+        _check_type: typing.Optional[bool] = None,
+        _content_type: typing.Optional[str] = None,
+        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
+    ):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -158,22 +170,27 @@
         # post parameters
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
             post_params.extend(self.files_parameters(files))
-
-        # auth setting
-        self.update_params_for_auth(header_params, query_params, auth_settings)
+            if header_params['Content-Type'].startswith("multipart"):
+                post_params = self.parameters_to_multipart(post_params,
+                                                           (dict))
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
+        # auth setting
+        self.update_params_for_auth(header_params, query_params,
+                                    auth_settings, resource_path, method, body,
+                                    request_auths=_request_auths)
+
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
         else:
             # use server/host defined in path or operation instead
             url = _host + resource_path
 
@@ -181,210 +198,251 @@
             # perform request and return response
             response_data = self.request(
                 method, url, query_params=query_params, headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout)
         except ApiException as e:
-            e.body = e.body.decode('utf-8') if six.PY3 else e.body
+            e.body = e.body.decode('utf-8')
             raise e
 
-        content_type = response_data.getheader('content-type')
-
         self.last_response = response_data
 
         return_data = response_data
 
         if not _preload_content:
+            return (return_data)
             return return_data
 
-        if six.PY3 and response_type not in ["file", "bytes"]:
-            match = None
-            if content_type is not None:
-                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
-            encoding = match.group(1) if match else "utf-8"
-            response_data.data = response_data.data.decode(encoding)
-
         # deserialize response data
         if response_type:
-            return_data = self.deserialize(response_data, response_type)
+            if response_type != (file_type,):
+                encoding = "utf-8"
+                content_type = response_data.getheader('content-type')
+                if content_type is not None:
+                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
+                    if match:
+                        encoding = match.group(1)
+                response_data.data = response_data.data.decode(encoding)
+
+            return_data = self.deserialize(
+                response_data,
+                response_type,
+                _check_type
+            )
         else:
             return_data = None
 
         if _return_http_data_only:
             return (return_data)
         else:
             return (return_data, response_data.status,
                     response_data.getheaders())
 
-    def sanitize_for_serialization(self, obj):
-        """Builds a JSON POST object.
+    def parameters_to_multipart(self, params, collection_types):
+        """Get parameters as list of tuples, formatting as json if value is collection_types
+
+        :param params: Parameters as list of two-tuples
+        :param dict collection_types: Parameter collection types
+        :return: Parameters as list of tuple or urllib3.fields.RequestField
+        """
+        new_params = []
+        if collection_types is None:
+            collection_types = (dict)
+        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+            if isinstance(
+                     v, collection_types): # v is instance of collection_type, formatting as application/json
+                v = json.dumps(v, ensure_ascii=False).encode("utf-8")
+                field = RequestField(k, v)
+                field.make_multipart(content_type="application/json; charset=utf-8")
+                new_params.append(field)
+            else:
+                new_params.append((k, v))
+        return new_params
 
+    @classmethod
+    def sanitize_for_serialization(cls, obj):
+        """Prepares data for transmission before it is sent with the rest client
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
-
+        If obj is io.IOBase, return the bytes
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
-        if obj is None:
-            return None
-        elif isinstance(obj, self.PRIMITIVE_TYPES):
+        if isinstance(obj, (ModelNormal, ModelComposed)):
+            return {
+                key: cls.sanitize_for_serialization(val) for key,
+                val in model_to_dict(
+                    obj,
+                    serialize=True).items()}
+        elif isinstance(obj, io.IOBase):
+            return cls.get_file_data_and_close_file(obj)
+        elif isinstance(obj, (str, int, float, none_type, bool)):
             return obj
-        elif isinstance(obj, list):
-            return [self.sanitize_for_serialization(sub_obj)
-                    for sub_obj in obj]
-        elif isinstance(obj, tuple):
-            return tuple(self.sanitize_for_serialization(sub_obj)
-                         for sub_obj in obj)
-        elif isinstance(obj, (datetime.datetime, datetime.date)):
+        elif isinstance(obj, (datetime, date)):
             return obj.isoformat()
-
+        elif isinstance(obj, ModelSimple):
+            return cls.sanitize_for_serialization(obj.value)
+        elif isinstance(obj, (list, tuple)):
+            return [cls.sanitize_for_serialization(item) for item in obj]
         if isinstance(obj, dict):
-            obj_dict = obj
-        else:
-            # Convert model obj to dict except
-            # attributes `openapi_types`, `attribute_map`
-            # and attributes which value is not None.
-            # Convert attribute name to json key in
-            # model definition for request.
-            obj_dict = {obj.attribute_map[attr]: getattr(obj, attr)
-                        for attr, _ in six.iteritems(obj.openapi_types)
-                        if getattr(obj, attr) is not None}
-
-        return {key: self.sanitize_for_serialization(val)
-                for key, val in six.iteritems(obj_dict)}
+            return {key: cls.sanitize_for_serialization(val) for key, val in obj.items()}
+        raise ApiValueError(
+            'Unable to prepare type {} for serialization'.format(
+                obj.__class__.__name__))
 
-    def deserialize(self, response, response_type):
+    def deserialize(self, response, response_type, _check_type):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
-        :param response_type: class literal for
-            deserialized object, or string of class name.
+        :param response_type: For the response, a tuple containing:
+            valid classes
+            a list containing valid classes (for list schemas)
+            a dict containing a tuple of valid classes as the value
+            Example values:
+            (str,)
+            (Pet,)
+            (float, none_type)
+            ([int, none_type],)
+            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
+        :param _check_type: boolean, whether to check the types of the data
+            received from the server
+        :type _check_type: bool
 
         :return: deserialized object.
         """
         # handle file downloading
         # save response body into a tmp file and return the instance
-        if response_type == "file":
-            return self.__deserialize_file(response)
+        if response_type == (file_type,):
+            content_disposition = response.getheader("Content-Disposition")
+            return deserialize_file(response.data, self.configuration,
+                                    content_disposition=content_disposition)
 
         # fetch data from response object
         try:
-            data = json.loads(response.data)
+            received_data = json.loads(response.data)
         except ValueError:
-            data = response.data
-
-        return self.__deserialize(data, response_type)
-
-    def __deserialize(self, data, klass):
-        """Deserializes dict, list, str into an object.
-
-        :param data: dict, list or str.
-        :param klass: class literal, or string of class name.
-
-        :return: object.
-        """
-        if data is None:
-            return None
+            received_data = response.data
 
-        if type(klass) == str:
-            if klass.startswith('list['):
-                sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
-                return [self.__deserialize(sub_data, sub_kls)
-                        for sub_data in data]
-
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
-                return {k: self.__deserialize(v, sub_kls)
-                        for k, v in six.iteritems(data)}
-
-            # convert str to class
-            if klass in self.NATIVE_TYPES_MAPPING:
-                klass = self.NATIVE_TYPES_MAPPING[klass]
-            else:
-                klass = getattr(flat_api.models, klass)
-
-        if klass in self.PRIMITIVE_TYPES:
-            return self.__deserialize_primitive(data, klass)
-        elif klass == object:
-            return self.__deserialize_object(data)
-        elif klass == datetime.date:
-            return self.__deserialize_date(data)
-        elif klass == datetime.datetime:
-            return self.__deserialize_datetime(data)
-        else:
-            return self.__deserialize_model(data, klass)
-
-    def call_api(self, resource_path, method,
-                 path_params=None, query_params=None, header_params=None,
-                 body=None, post_params=None, files=None,
-                 response_type=None, auth_settings=None, async_req=None,
-                 _return_http_data_only=None, collection_formats=None,
-                 _preload_content=True, _request_timeout=None, _host=None):
+        # store our data under the key of 'received_data' so users have some
+        # context if they are deserializing a string and the data type is wrong
+        deserialized_data = validate_and_convert_types(
+            received_data,
+            response_type,
+            ['received_data'],
+            True,
+            _check_type,
+            configuration=self.configuration
+        )
+        return deserialized_data
+
+    def call_api(
+        self,
+        resource_path: str,
+        method: str,
+        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
+        body: typing.Optional[typing.Any] = None,
+        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
+        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
+        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
+        auth_settings: typing.Optional[typing.List[str]] = None,
+        async_req: typing.Optional[bool] = None,
+        _return_http_data_only: typing.Optional[bool] = None,
+        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
+        _preload_content: bool = True,
+        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
+        _host: typing.Optional[str] = None,
+        _check_type: typing.Optional[bool] = None,
+        _request_auths: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
+    ):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
         :param header_params: Header parameters to be
             placed in the request header.
         :param body: Request body.
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
-        :param response: Response data type.
-        :param files dict: key -> filename, value -> filepath,
-            for `multipart/form-data`.
+        :param response_type: For the response, a tuple containing:
+            valid classes
+            a list containing valid classes (for list schemas)
+            a dict containing a tuple of valid classes as the value
+            Example values:
+            (str,)
+            (Pet,)
+            (float, none_type)
+            ([int, none_type],)
+            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
+        :param files: key -> field name, value -> a list of open file
+            objects for `multipart/form-data`.
+        :type files: dict
         :param async_req bool: execute request asynchronously
+        :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
+        :type _return_http_data_only: bool, optional
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
+        :type collection_formats: dict, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
+        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
+        :param _check_type: boolean describing if the data back from the server
+            should have its type checked.
+        :type _check_type: bool, optional
+        :param _request_auths: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auths: list, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
                                    response_type, auth_settings,
                                    _return_http_data_only, collection_formats,
-                                   _preload_content, _request_timeout, _host)
+                                   _preload_content, _request_timeout, _host,
+                                   _check_type, _request_auths=_request_auths)
 
         return self.pool.apply_async(self.__call_api, (resource_path,
                                                        method, path_params,
                                                        query_params,
                                                        header_params, body,
                                                        post_params, files,
                                                        response_type,
                                                        auth_settings,
                                                        _return_http_data_only,
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
-                                                       _host))
+                                                       _host, _check_type, None, _request_auths))
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(url,
@@ -398,16 +456,18 @@
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          headers=headers)
         elif method == "OPTIONS":
             return self.rest_client.OPTIONS(url,
                                             query_params=query_params,
                                             headers=headers,
+                                            post_params=post_params,
                                             _preload_content=_preload_content,
-                                            _request_timeout=_request_timeout)
+                                            _request_timeout=_request_timeout,
+                                            body=body)
         elif method == "POST":
             return self.rest_client.POST(url,
                                          query_params=query_params,
                                          headers=headers,
                                          post_params=post_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
@@ -447,15 +507,15 @@
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
         new_params = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in six.iteritems(params) if isinstance(params, dict) else params:  # noqa: E501
+        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, value) for value in v)
                 else:
                     if collection_format == 'ssv':
                         delimiter = ' '
@@ -467,35 +527,52 @@
                         delimiter = ','
                     new_params.append(
                         (k, delimiter.join(str(value) for value in v)))
             else:
                 new_params.append((k, v))
         return new_params
 
-    def files_parameters(self, files=None):
+    @staticmethod
+    def get_file_data_and_close_file(file_instance: io.IOBase) -> bytes:
+        file_data = file_instance.read()
+        file_instance.close()
+        return file_data
+
+    def files_parameters(self,
+                         files: typing.Optional[typing.Dict[str,
+                                                            typing.List[io.IOBase]]] = None):
         """Builds form parameters.
 
-        :param files: File parameters.
-        :return: Form parameters with files.
+        :param files: None or a dict with key=param_name and
+            value is a list of open file objects
+        :return: List of tuples of form parameters with file data
         """
-        params = []
+        if files is None:
+            return []
 
-        if files:
-            for k, v in six.iteritems(files):
-                if not v:
+        params = []
+        for param_name, file_instances in files.items():
+            if file_instances is None:
+                # if the file field is nullable, skip None values
+                continue
+            for file_instance in file_instances:
+                if file_instance is None:
+                    # if the file field is nullable, skip None values
                     continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (mimetypes.guess_type(filename)[0] or
-                                    'application/octet-stream')
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])]))
+                if file_instance.closed is True:
+                    raise ApiValueError(
+                        "Cannot read a closed file. The passed in file_type "
+                        "for %s must be open." % param_name
+                    )
+                filename = os.path.basename(file_instance.name)
+                filedata = self.get_file_data_and_close_file(file_instance)
+                mimetype = (mimetypes.guess_type(filename)[0] or
+                            'application/octet-stream')
+                params.append(
+                    tuple([param_name, tuple([filename, filedata, mimetype])]))
 
         return params
 
     def select_header_accept(self, accepts):
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
@@ -507,161 +584,314 @@
         accepts = [x.lower() for x in accepts]
 
         if 'application/json' in accepts:
             return 'application/json'
         else:
             return ', '.join(accepts)
 
-    def select_header_content_type(self, content_types):
+    def select_header_content_type(self, content_types, method=None, body=None):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
+        :param method: http method (e.g. POST, PATCH).
+        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
-            return 'application/json'
+            return None
 
         content_types = [x.lower() for x in content_types]
 
+        if (method == 'PATCH' and
+                'application/json-patch+json' in content_types and
+                isinstance(body, list)):
+            return 'application/json-patch+json'
+
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, querys, auth_settings):
+    def update_params_for_auth(self, headers, queries, auth_settings,
+                               resource_path, method, body, request_auths=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
+        :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
+        :param resource_path: A string representation of the HTTP request resource path.
+        :param method: A string representation of the HTTP request method.
+        :param body: A object representing the body of the HTTP request.
+            The object type is the return value of _encoder.default().
+        :param request_auths: if set, the provided settings will
+            override the token in the configuration.
         """
         if not auth_settings:
             return
 
+        if request_auths:
+            for auth_setting in request_auths:
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting)
+            return
+
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                if auth_setting['in'] == 'cookie':
-                    headers['Cookie'] = auth_setting['value']
-                elif auth_setting['in'] == 'header':
-                    headers[auth_setting['key']] = auth_setting['value']
-                elif auth_setting['in'] == 'query':
-                    querys.append((auth_setting['key'], auth_setting['value']))
-                else:
-                    raise ApiValueError(
-                        'Authentication token must be in `query` or `header`'
-                    )
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting)
 
-    def __deserialize_file(self, response):
-        """Deserializes body to file
+    def _apply_auth_params(self, headers, queries, resource_path, method, body, auth_setting):
+        if auth_setting['in'] == 'cookie':
+            headers['Cookie'] = auth_setting['key'] + "=" + auth_setting['value']
+        elif auth_setting['in'] == 'header':
+            if auth_setting['type'] != 'http-signature':
+                headers[auth_setting['key']] = auth_setting['value']
+        elif auth_setting['in'] == 'query':
+            queries.append((auth_setting['key'], auth_setting['value']))
+        else:
+            raise ApiValueError(
+                'Authentication token must be in `query` or `header`'
+            )
 
-        Saves response body into a file in a temporary folder,
-        using the filename from the `Content-Disposition` header if provided.
 
-        :param response:  RESTResponse.
-        :return: file path.
-        """
-        fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
-        os.close(fd)
-        os.remove(path)
+class Endpoint(object):
+    def __init__(self, settings=None, params_map=None, root_map=None,
+                 headers_map=None, api_client=None, callable=None):
+        """Creates an endpoint
+
+        Args:
+            settings (dict): see below key value pairs
+                'response_type' (tuple/None): response type
+                'auth' (list): a list of auth type keys
+                'endpoint_path' (str): the endpoint path
+                'operation_id' (str): endpoint string identifier
+                'http_method' (str): POST/PUT/PATCH/GET etc
+                'servers' (list): list of str servers that this endpoint is at
+            params_map (dict): see below key value pairs
+                'all' (list): list of str endpoint parameter names
+                'required' (list): list of required parameter names
+                'nullable' (list): list of nullable parameter names
+                'enum' (list): list of parameters with enum values
+                'validation' (list): list of parameters with validations
+            root_map
+                'validations' (dict): the dict mapping endpoint parameter tuple
+                    paths to their validation dictionaries
+                'allowed_values' (dict): the dict mapping endpoint parameter
+                    tuple paths to their allowed_values (enum) dictionaries
+                'openapi_types' (dict): param_name to openapi type
+                'attribute_map' (dict): param_name to camelCase name
+                'location_map' (dict): param_name to  'body', 'file', 'form',
+                    'header', 'path', 'query'
+                collection_format_map (dict): param_name to `csv` etc.
+            headers_map (dict): see below key value pairs
+                'accept' (list): list of Accept header strings
+                'content_type' (list): list of Content-Type header strings
+            api_client (ApiClient) api client instance
+            callable (function): the function which is invoked when the
+                Endpoint is called
+        """
+        self.settings = settings
+        self.params_map = params_map
+        self.params_map['all'].extend([
+            'async_req',
+            '_host_index',
+            '_preload_content',
+            '_request_timeout',
+            '_return_http_data_only',
+            '_check_input_type',
+            '_check_return_type',
+            '_content_type',
+            '_spec_property_naming',
+            '_request_auths'
+        ])
+        self.params_map['nullable'].extend(['_request_timeout'])
+        self.validations = root_map['validations']
+        self.allowed_values = root_map['allowed_values']
+        self.openapi_types = root_map['openapi_types']
+        extra_types = {
+            'async_req': (bool,),
+            '_host_index': (none_type, int),
+            '_preload_content': (bool,),
+            '_request_timeout': (none_type, float, (float,), [float], int, (int,), [int]),
+            '_return_http_data_only': (bool,),
+            '_check_input_type': (bool,),
+            '_check_return_type': (bool,),
+            '_spec_property_naming': (bool,),
+            '_content_type': (none_type, str),
+            '_request_auths': (none_type, list)
+        }
+        self.openapi_types.update(extra_types)
+        self.attribute_map = root_map['attribute_map']
+        self.location_map = root_map['location_map']
+        self.collection_format_map = root_map['collection_format_map']
+        self.headers_map = headers_map
+        self.api_client = api_client
+        self.callable = callable
+
+    def __validate_inputs(self, kwargs):
+        for param in self.params_map['enum']:
+            if param in kwargs:
+                check_allowed_values(
+                    self.allowed_values,
+                    (param,),
+                    kwargs[param]
+                )
 
-        content_disposition = response.getheader("Content-Disposition")
-        if content_disposition:
-            filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                                 content_disposition).group(1)
-            path = os.path.join(os.path.dirname(path), filename)
+        for param in self.params_map['validation']:
+            if param in kwargs:
+                check_validations(
+                    self.validations,
+                    (param,),
+                    kwargs[param],
+                    configuration=self.api_client.configuration
+                )
 
-        with open(path, "wb") as f:
-            f.write(response.data)
+        if kwargs['_check_input_type'] is False:
+            return
 
-        return path
+        for key, value in kwargs.items():
+            fixed_val = validate_and_convert_types(
+                value,
+                self.openapi_types[key],
+                [key],
+                kwargs['_spec_property_naming'],
+                kwargs['_check_input_type'],
+                configuration=self.api_client.configuration
+            )
+            kwargs[key] = fixed_val
 
-    def __deserialize_primitive(self, data, klass):
-        """Deserializes string to primitive type.
+    def __gather_params(self, kwargs):
+        params = {
+            'body': None,
+            'collection_format': {},
+            'file': {},
+            'form': [],
+            'header': {},
+            'path': {},
+            'query': []
+        }
+
+        for param_name, param_value in kwargs.items():
+            param_location = self.location_map.get(param_name)
+            if param_location is None:
+                continue
+            if param_location:
+                if param_location == 'body':
+                    params['body'] = param_value
+                    continue
+                base_name = self.attribute_map[param_name]
+                if (param_location == 'form' and
+                        self.openapi_types[param_name] == (file_type,)):
+                    params['file'][base_name] = [param_value]
+                elif (param_location == 'form' and
+                        self.openapi_types[param_name] == ([file_type],)):
+                    # param_value is already a list
+                    params['file'][base_name] = param_value
+                elif param_location in {'form', 'query'}:
+                    param_value_full = (base_name, param_value)
+                    params[param_location].append(param_value_full)
+                if param_location not in {'form', 'query'}:
+                    params[param_location][base_name] = param_value
+                collection_format = self.collection_format_map.get(param_name)
+                if collection_format:
+                    params['collection_format'][base_name] = collection_format
 
-        :param data: str.
-        :param klass: class literal.
+        return params
 
-        :return: int, long, float, str, bool.
-        """
-        try:
-            return klass(data)
-        except UnicodeEncodeError:
-            return six.text_type(data)
-        except TypeError:
-            return data
+    def __call__(self, *args, **kwargs):
+        """ This method is invoked when endpoints are called
+        Example:
 
-    def __deserialize_object(self, value):
-        """Return an original value.
+        api_instance = AccountApi()
+        api_instance.get_authenticated_user  # this is an instance of the class Endpoint
+        api_instance.get_authenticated_user()  # this invokes api_instance.get_authenticated_user.__call__()
+        which then invokes the callable functions stored in that endpoint at
+        api_instance.get_authenticated_user.callable or self.callable in this class
 
-        :return: object.
         """
-        return value
+        return self.callable(self, *args, **kwargs)
 
-    def __deserialize_date(self, string):
-        """Deserializes string to date.
+    def call_with_http_info(self, **kwargs):
 
-        :param string: str.
-        :return: date.
-        """
         try:
-            return parse(string).date()
-        except ImportError:
-            return string
-        except ValueError:
-            raise rest.ApiException(
-                status=0,
-                reason="Failed to parse `{0}` as date object".format(string)
+            index = self.api_client.configuration.server_operation_index.get(
+                self.settings['operation_id'], self.api_client.configuration.server_index
+            ) if kwargs['_host_index'] is None else kwargs['_host_index']
+            server_variables = self.api_client.configuration.server_operation_variables.get(
+                self.settings['operation_id'], self.api_client.configuration.server_variables
             )
+            _host = self.api_client.configuration.get_host_from_settings(
+                index, variables=server_variables, servers=self.settings['servers']
+            )
+        except IndexError:
+            if self.settings['servers']:
+                raise ApiValueError(
+                    "Invalid host index. Must be 0 <= index < %s" %
+                    len(self.settings['servers'])
+                )
+            _host = None
 
-    def __deserialize_datetime(self, string):
-        """Deserializes string to datetime.
-
-        The string should be in iso8601 datetime format.
+        for key, value in kwargs.items():
+            if key not in self.params_map['all']:
+                raise ApiTypeError(
+                    "Got an unexpected parameter '%s'"
+                    " to method `%s`" %
+                    (key, self.settings['operation_id'])
+                )
+            # only throw this nullable ApiValueError if _check_input_type
+            # is False, if _check_input_type==True we catch this case
+            # in self.__validate_inputs
+            if (key not in self.params_map['nullable'] and value is None
+                    and kwargs['_check_input_type'] is False):
+                raise ApiValueError(
+                    "Value may not be None for non-nullable parameter `%s`"
+                    " when calling `%s`" %
+                    (key, self.settings['operation_id'])
+                )
 
-        :param string: str.
-        :return: datetime.
-        """
-        try:
-            return parse(string)
-        except ImportError:
-            return string
-        except ValueError:
-            raise rest.ApiException(
-                status=0,
-                reason=(
-                    "Failed to parse `{0}` as datetime object"
-                    .format(string)
+        for key in self.params_map['required']:
+            if key not in kwargs.keys():
+                raise ApiValueError(
+                    "Missing the required parameter `%s` when calling "
+                    "`%s`" % (key, self.settings['operation_id'])
                 )
-            )
 
-    def __deserialize_model(self, data, klass):
-        """Deserializes list or dict to model.
+        self.__validate_inputs(kwargs)
+
+        params = self.__gather_params(kwargs)
 
-        :param data: dict, list.
-        :param klass: class literal.
-        :return: model object.
-        """
-        has_discriminator = False
-        if (hasattr(klass, 'get_real_child_model')
-                and klass.discriminator_value_class_map):
-            has_discriminator = True
-
-        if not klass.openapi_types and has_discriminator is False:
-            return data
-
-        kwargs = {}
-        if (data is not None and
-                klass.openapi_types is not None and
-                isinstance(data, (list, dict))):
-            for attr, attr_type in six.iteritems(klass.openapi_types):
-                if klass.attribute_map[attr] in data:
-                    value = data[klass.attribute_map[attr]]
-                    kwargs[attr] = self.__deserialize(value, attr_type)
-
-        instance = klass(**kwargs)
-
-        if has_discriminator:
-            klass_name = instance.get_real_child_model(data)
-            if klass_name:
-                instance = self.__deserialize(data, klass_name)
-        return instance
+        accept_headers_list = self.headers_map['accept']
+        if accept_headers_list:
+            params['header']['Accept'] = self.api_client.select_header_accept(
+                accept_headers_list)
+
+        if kwargs.get('_content_type'):
+            params['header']['Content-Type'] = kwargs['_content_type']
+        else:
+            content_type_headers_list = self.headers_map['content_type']
+            if content_type_headers_list:
+                if params['body'] != "":
+                    content_types_list = self.api_client.select_header_content_type(
+                        content_type_headers_list, self.settings['http_method'],
+                        params['body'])
+                    if content_types_list:
+                        params['header']['Content-Type'] = content_types_list
+
+        return self.api_client.call_api(
+            self.settings['endpoint_path'], self.settings['http_method'],
+            params['path'],
+            params['query'],
+            params['header'],
+            body=params['body'],
+            post_params=params['form'],
+            files=params['file'],
+            response_type=self.settings['response_type'],
+            auth_settings=self.settings['auth'],
+            async_req=kwargs['async_req'],
+            _check_type=kwargs['_check_return_type'],
+            _return_http_data_only=kwargs['_return_http_data_only'],
+            _preload_content=kwargs['_preload_content'],
+            _request_timeout=kwargs['_request_timeout'],
+            _host=_host,
+            _request_auths=kwargs['_request_auths'],
+            collection_formats=params['collection_format'])
```

### Comparing `flat_api-0.8.1/flat_api/configuration.py` & `flat_api-1.0.0/flat_api/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-import six
-from six.moves import http_client as httplib
+from http import client as http_client
+from flat_api.exceptions import ApiValueError
+
 
+JSON_SCHEMA_VALIDATION_KEYWORDS = {
+    'multipleOf', 'maximum', 'exclusiveMaximum',
+    'minimum', 'exclusiveMinimum', 'maxLength',
+    'minLength', 'pattern', 'maxItems', 'minItems'
+}
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
@@ -46,34 +48,72 @@
          implementation.
       2. The client was generated using an older version of the OpenAPI document
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
+    :param server_index: Index to servers configuration.
+    :param server_variables: Mapping with string values to replace variables in
+      templated server configuration. The validation of enums is performed for
+      variables with defined enum values before.
+    :param server_operation_index: Mapping from operation ID to an index to server
+      configuration.
+    :param server_operation_variables: Mapping from operation ID to a mapping with
+      string values to replace variables in templated server configuration.
+      The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format
 
     :Example:
     """
 
     _default = None
 
-    def __init__(self, host="https://api.flat.io/v2",
+    def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
+                 access_token=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
+                 disabled_client_side_validations="",
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self.host = host
+        self._base_path = "https://api.flat.io/v2" if host is None else host
         """Default Base url
         """
+        self.server_index = 0 if server_index is None and host is None else server_index
+        self.server_operation_index = server_operation_index or {}
+        """Default server index
+        """
+        self.server_variables = server_variables or {}
+        self.server_operation_variables = server_operation_variables or {}
+        """Default server variables
+        """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
+        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -86,17 +126,15 @@
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
-        self.access_token = None
-        """access token for OAuth/Bearer
-        """
+        self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("flat_api")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -115,15 +153,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -139,26 +177,32 @@
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
+        self.no_proxy = None
+        """bypass proxy for host in the no_proxy list.
+        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
-        # Disable client side validation
+        # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
+        self.socket_options = None
+
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
                 setattr(result, k, copy.deepcopy(v, memo))
@@ -167,14 +211,21 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
@@ -221,15 +272,15 @@
         """
         self.__logger_file = value
         if self.__logger_file:
             # If set logging file,
             # then add file handler and remove stream handler.
             self.logger_file_handler = logging.FileHandler(self.__logger_file)
             self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.addHandler(self.logger_file_handler)
 
     @property
     def debug(self):
         """Debug status
 
         :param value: The debug status, True or False.
@@ -243,25 +294,25 @@
 
         :param value: The debug status, True or False.
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -278,23 +329,24 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
-    def get_api_key_with_prefix(self, identifier):
+    def get_api_key_with_prefix(self, identifier, alias=None):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
+        :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier)
+        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
@@ -332,57 +384,72 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.17.0\n"\
-               "SDK Package Version: 0.7.0".\
+               "Version of the API: 2.18.0\n"\
+               "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
                 'url': "https://api.flat.io/v2",
                 'description': "No description provided",
             }
         ]
 
-    def get_host_from_settings(self, index, variables=None):
+    def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
+        :param servers: an array of host settings or None
         :return: URL based on host settings
         """
+        if index is None:
+            return self._base_path
+
         variables = {} if variables is None else variables
-        servers = self.get_host_settings()
+        servers = self.get_host_settings() if servers is None else servers
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
                 "Invalid index {0} when selecting the host settings. "
                 "Must be less than {1}".format(index, len(servers)))
 
         url = server['url']
 
         # go through variables and replace placeholders
-        for variable_name, variable in server['variables'].items():
+        for variable_name, variable in server.get('variables', {}).items():
             used_value = variables.get(
                 variable_name, variable['default_value'])
 
             if 'enum_values' in variable \
                     and used_value not in variable['enum_values']:
                 raise ValueError(
                     "The variable `{0}` in the host URL has invalid value "
                     "{1}. Must be {2}.".format(
                         variable_name, variables[variable_name],
                         variable['enum_values']))
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
+
+    @property
+    def host(self):
+        """Return generated host."""
+        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
+
+    @host.setter
+    def host(self, value):
+        """Fix base path."""
+        self._base_path = value
+        self.server_index = None
```

### Comparing `flat_api-0.8.1/flat_api/models/score_creation.py` & `flat_api-1.0.0/flat_api/model/resource_rights.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,347 +1,276 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-import pprint
 import re  # noqa: F401
+import sys  # noqa: F401
 
-import six
+from flat_api.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from flat_api.exceptions import ApiAttributeError
 
-from flat_api.configuration import Configuration
 
 
-class ScoreCreation(object):
+class ResourceRights(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
-    """
     Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
     """
-    openapi_types = {
-        'data_encoding': 'str',
-        'title': 'str',
-        'privacy': 'ScorePrivacy',
-        'builder_data': 'ScoreCreationBuilderData',
-        'filename': 'str',
-        'source': 'ScoreSource',
-        'collection': 'str',
-        'data': 'str',
-        'google_drive_folder': 'str'
-    }
 
-    attribute_map = {
-        'data_encoding': 'dataEncoding',
-        'title': 'title',
-        'privacy': 'privacy',
-        'builder_data': 'builderData',
-        'filename': 'filename',
-        'source': 'source',
-        'collection': 'collection',
-        'data': 'data',
-        'google_drive_folder': 'googleDriveFolder'
+    allowed_values = {
     }
 
-    def __init__(self, data_encoding=None, title=None, privacy=None, builder_data=None, filename=None, source=None, collection=None, data=None, google_drive_folder=None, local_vars_configuration=None):  # noqa: E501
-        """ScoreCreation - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._data_encoding = None
-        self._title = None
-        self._privacy = None
-        self._builder_data = None
-        self._filename = None
-        self._source = None
-        self._collection = None
-        self._data = None
-        self._google_drive_folder = None
-        self.discriminator = None
-
-        if data_encoding is not None:
-            self.data_encoding = data_encoding
-        if title is not None:
-            self.title = title
-        if privacy is not None:
-            self.privacy = privacy
-        if builder_data is not None:
-            self.builder_data = builder_data
-        if filename is not None:
-            self.filename = filename
-        if source is not None:
-            self.source = source
-        if collection is not None:
-            self.collection = collection
-        if data is not None:
-            self.data = data
-        if google_drive_folder is not None:
-            self.google_drive_folder = google_drive_folder
-
-    @property
-    def data_encoding(self):
-        """Gets the data_encoding of this ScoreCreation.  # noqa: E501
-
-        The optional encoding of the score data. This property must match the encoding used for the `data` property.  # noqa: E501
-
-        :return: The data_encoding of this ScoreCreation.  # noqa: E501
-        :rtype: str
-        """
-        return self._data_encoding
-
-    @data_encoding.setter
-    def data_encoding(self, data_encoding):
-        """Sets the data_encoding of this ScoreCreation.
-
-        The optional encoding of the score data. This property must match the encoding used for the `data` property.  # noqa: E501
-
-        :param data_encoding: The data_encoding of this ScoreCreation.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["base64"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and data_encoding not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `data_encoding` ({0}), must be one of {1}"  # noqa: E501
-                .format(data_encoding, allowed_values)
-            )
-
-        self._data_encoding = data_encoding
-
-    @property
-    def title(self):
-        """Gets the title of this ScoreCreation.  # noqa: E501
-
-        The title of the new score. If the title is too long, the API may trim this one.  If this title is not specified, the API will try to (in this order):   - Use the title contained in the file (e.g. [`movement-title`](https://usermanuals.musicxml.com/MusicXML/Content/EL-MusicXML-movement-title.htm) or [`credit-words`](https://usermanuals.musicxml.com/MusicXML/Content/EL-MusicXML-credit-words.htm) for [MusicXML](http://www.musicxml.com/) files).   - Use the name of the file for files from a specified `source` (e.g. Google Drive) or the one in the `filename` property   - Set a default title (e.g. \"New Music Score\")   # noqa: E501
-
-        :return: The title of this ScoreCreation.  # noqa: E501
-        :rtype: str
-        """
-        return self._title
-
-    @title.setter
-    def title(self, title):
-        """Sets the title of this ScoreCreation.
-
-        The title of the new score. If the title is too long, the API may trim this one.  If this title is not specified, the API will try to (in this order):   - Use the title contained in the file (e.g. [`movement-title`](https://usermanuals.musicxml.com/MusicXML/Content/EL-MusicXML-movement-title.htm) or [`credit-words`](https://usermanuals.musicxml.com/MusicXML/Content/EL-MusicXML-credit-words.htm) for [MusicXML](http://www.musicxml.com/) files).   - Use the name of the file for files from a specified `source` (e.g. Google Drive) or the one in the `filename` property   - Set a default title (e.g. \"New Music Score\")   # noqa: E501
-
-        :param title: The title of this ScoreCreation.  # noqa: E501
-        :type: str
-        """
-
-        self._title = title
-
-    @property
-    def privacy(self):
-        """Gets the privacy of this ScoreCreation.  # noqa: E501
-
-
-        :return: The privacy of this ScoreCreation.  # noqa: E501
-        :rtype: ScorePrivacy
-        """
-        return self._privacy
-
-    @privacy.setter
-    def privacy(self, privacy):
-        """Sets the privacy of this ScoreCreation.
-
-
-        :param privacy: The privacy of this ScoreCreation.  # noqa: E501
-        :type: ScorePrivacy
-        """
-
-        self._privacy = privacy
-
-    @property
-    def builder_data(self):
-        """Gets the builder_data of this ScoreCreation.  # noqa: E501
-
-
-        :return: The builder_data of this ScoreCreation.  # noqa: E501
-        :rtype: ScoreCreationBuilderData
-        """
-        return self._builder_data
-
-    @builder_data.setter
-    def builder_data(self, builder_data):
-        """Sets the builder_data of this ScoreCreation.
-
-
-        :param builder_data: The builder_data of this ScoreCreation.  # noqa: E501
-        :type: ScoreCreationBuilderData
-        """
-
-        self._builder_data = builder_data
-
-    @property
-    def filename(self):
-        """Gets the filename of this ScoreCreation.  # noqa: E501
-
-        If this is an imported file, its filename  # noqa: E501
-
-        :return: The filename of this ScoreCreation.  # noqa: E501
-        :rtype: str
-        """
-        return self._filename
-
-    @filename.setter
-    def filename(self, filename):
-        """Sets the filename of this ScoreCreation.
-
-        If this is an imported file, its filename  # noqa: E501
-
-        :param filename: The filename of this ScoreCreation.  # noqa: E501
-        :type: str
-        """
-
-        self._filename = filename
-
-    @property
-    def source(self):
-        """Gets the source of this ScoreCreation.  # noqa: E501
-
-
-        :return: The source of this ScoreCreation.  # noqa: E501
-        :rtype: ScoreSource
-        """
-        return self._source
-
-    @source.setter
-    def source(self, source):
-        """Sets the source of this ScoreCreation.
-
-
-        :param source: The source of this ScoreCreation.  # noqa: E501
-        :type: ScoreSource
-        """
-
-        self._source = source
-
-    @property
-    def collection(self):
-        """Gets the collection of this ScoreCreation.  # noqa: E501
-
-        Unique identifier of a collection where the score will be created. If no collection identifier is provided, the score will be stored in the `root` directory.   # noqa: E501
-
-        :return: The collection of this ScoreCreation.  # noqa: E501
-        :rtype: str
-        """
-        return self._collection
-
-    @collection.setter
-    def collection(self, collection):
-        """Sets the collection of this ScoreCreation.
-
-        Unique identifier of a collection where the score will be created. If no collection identifier is provided, the score will be stored in the `root` directory.   # noqa: E501
+    validations = {
+    }
 
-        :param collection: The collection of this ScoreCreation.  # noqa: E501
-        :type: str
+    @cached_property
+    def additional_properties_type():
         """
-
-        self._collection = collection
-
-    @property
-    def data(self):
-        """Gets the data of this ScoreCreation.  # noqa: E501
-
-        The data of the score file. It must be a MusicXML 3 file (`vnd.recordare.musicxml` or `vnd.recordare.musicxml+xml`), a MIDI file (`audio/midi`) or a Flat.json (aka Adagio.json) file. Binary payloads (`vnd.recordare.musicxml` and `audio/midi`) can be encoded in Base64, in this case the `dataEncoding` property must match the encoding used for the API request.   # noqa: E501
-
-        :return: The data of this ScoreCreation.  # noqa: E501
-        :rtype: str
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
         """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this ScoreCreation.
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-        The data of the score file. It must be a MusicXML 3 file (`vnd.recordare.musicxml` or `vnd.recordare.musicxml+xml`), a MIDI file (`audio/midi`) or a Flat.json (aka Adagio.json) file. Binary payloads (`vnd.recordare.musicxml` and `audio/midi`) can be encoded in Base64, in this case the `dataEncoding` property must match the encoding used for the API request.   # noqa: E501
+    _nullable = False
 
-        :param data: The data of this ScoreCreation.  # noqa: E501
-        :type: str
+    @cached_property
+    def openapi_types():
         """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
 
-        self._data = data
-
-    @property
-    def google_drive_folder(self):
-        """Gets the google_drive_folder of this ScoreCreation.  # noqa: E501
-
-        If the user uses Google Drive and this properties is specified, the file will be created in this directory. The currently user creating the file must be granted to write in this directory.   # noqa: E501
-
-        :return: The google_drive_folder of this ScoreCreation.  # noqa: E501
-        :rtype: str
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
         """
-        return self._google_drive_folder
+        return {
+            'acl_read': (bool,),  # noqa: E501
+            'acl_write': (bool,),  # noqa: E501
+            'acl_admin': (bool,),  # noqa: E501
+            'is_collaborator': (bool,),  # noqa: E501
+        }
 
-    @google_drive_folder.setter
-    def google_drive_folder(self, google_drive_folder):
-        """Sets the google_drive_folder of this ScoreCreation.
+    @cached_property
+    def discriminator():
+        return None
 
-        If the user uses Google Drive and this properties is specified, the file will be created in this directory. The currently user creating the file must be granted to write in this directory.   # noqa: E501
 
-        :param google_drive_folder: The google_drive_folder of this ScoreCreation.  # noqa: E501
-        :type: str
-        """
+    attribute_map = {
+        'acl_read': 'aclRead',  # noqa: E501
+        'acl_write': 'aclWrite',  # noqa: E501
+        'acl_admin': 'aclAdmin',  # noqa: E501
+        'is_collaborator': 'isCollaborator',  # noqa: E501
+    }
 
-        self._google_drive_folder = google_drive_folder
+    read_only_vars = {
+    }
 
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, ScoreCreation):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, ScoreCreation):
-            return True
+    _composed_schemas = {}
 
-        return self.to_dict() != other.to_dict()
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ResourceRights - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            acl_read (bool): `True` if the current user can read the current document . [optional] if omitted the server will use the default value of False  # noqa: E501
+            acl_write (bool): `True` if the current user can modify the current document.  If this is a right of a Collection, the capabilities of the associated user can be lower than this permission, check out the `capabilities` property as the end-user to have the complete possibilities with the collection. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            acl_admin (bool): `True` if the current user can manage the current document (i.e. share, delete)  If this is a right of a Collection, the capabilities of the associated user can be lower than this permission, check out the `capabilities` property as the end-user to have the complete possibilities with the collection. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            is_collaborator (bool): `True` if the current user is a collaborator of the current document (direct or via group). . [optional] if omitted the server will use the default value of False  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ResourceRights - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            acl_read (bool): `True` if the current user can read the current document . [optional] if omitted the server will use the default value of False  # noqa: E501
+            acl_write (bool): `True` if the current user can modify the current document.  If this is a right of a Collection, the capabilities of the associated user can be lower than this permission, check out the `capabilities` property as the end-user to have the complete possibilities with the collection. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            acl_admin (bool): `True` if the current user can manage the current document (i.e. share, delete)  If this is a right of a Collection, the capabilities of the associated user can be lower than this permission, check out the `capabilities` property as the end-user to have the complete possibilities with the collection. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            is_collaborator (bool): `True` if the current user is a collaborator of the current document (direct or via group). . [optional] if omitted the server will use the default value of False  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `flat_api-0.8.1/flat_api/models/user_details.py` & `flat_api-1.0.0/flat_api/model/score_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,848 +1,416 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-import pprint
 import re  # noqa: F401
+import sys  # noqa: F401
 
-import six
-
-from flat_api.configuration import Configuration
+from flat_api.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from flat_api.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from flat_api.model.resource_collaborator import ResourceCollaborator
+    from flat_api.model.resource_rights import ResourceRights
+    from flat_api.model.score_comments_counts import ScoreCommentsCounts
+    from flat_api.model.score_creation_type import ScoreCreationType
+    from flat_api.model.score_license import ScoreLicense
+    from flat_api.model.score_likes_counts import ScoreLikesCounts
+    from flat_api.model.score_plays_counts import ScorePlaysCounts
+    from flat_api.model.score_privacy import ScorePrivacy
+    from flat_api.model.score_views_counts import ScoreViewsCounts
+    from flat_api.model.user_public_summary import UserPublicSummary
+    globals()['ResourceCollaborator'] = ResourceCollaborator
+    globals()['ResourceRights'] = ResourceRights
+    globals()['ScoreCommentsCounts'] = ScoreCommentsCounts
+    globals()['ScoreCreationType'] = ScoreCreationType
+    globals()['ScoreLicense'] = ScoreLicense
+    globals()['ScoreLikesCounts'] = ScoreLikesCounts
+    globals()['ScorePlaysCounts'] = ScorePlaysCounts
+    globals()['ScorePrivacy'] = ScorePrivacy
+    globals()['ScoreViewsCounts'] = ScoreViewsCounts
+    globals()['UserPublicSummary'] = UserPublicSummary
 
 
-class UserDetails(object):
+class ScoreDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
-    """
     Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
     """
-    openapi_types = {
-        'username': 'str',
-        'class_role': 'ClassRoles',
-        'private_profile': 'bool',
-        'followers_count': 'int',
-        'firstname': 'str',
-        'is_power_user': 'bool',
-        'locale': 'FlatLocales',
-        'instruments': 'list[str]',
-        'html_url': 'str',
-        'liked_scores_count': 'int',
-        'printable_name': 'str',
-        'bio': 'str',
-        'picture_file': 'str',
-        'id': 'str',
-        'cover_picture_file': 'str',
-        'picture': 'str',
-        'name': 'str',
-        'is_flat_team': 'bool',
-        'organization_role': 'OrganizationRoles',
-        'profile_theme': 'str',
-        'cover_picture': 'str',
-        'owned_public_scores_count': 'int',
-        'lastname': 'str',
-        'following_count': 'int',
-        'organization': 'str',
-        'type': 'str',
-        'registration_date': 'datetime'
-    }
 
-    attribute_map = {
-        'username': 'username',
-        'class_role': 'classRole',
-        'private_profile': 'privateProfile',
-        'followers_count': 'followersCount',
-        'firstname': 'firstname',
-        'is_power_user': 'isPowerUser',
-        'locale': 'locale',
-        'instruments': 'instruments',
-        'html_url': 'htmlUrl',
-        'liked_scores_count': 'likedScoresCount',
-        'printable_name': 'printableName',
-        'bio': 'bio',
-        'picture_file': 'pictureFile',
-        'id': 'id',
-        'cover_picture_file': 'coverPictureFile',
-        'picture': 'picture',
-        'name': 'name',
-        'is_flat_team': 'isFlatTeam',
-        'organization_role': 'organizationRole',
-        'profile_theme': 'profileTheme',
-        'cover_picture': 'coverPicture',
-        'owned_public_scores_count': 'ownedPublicScoresCount',
-        'lastname': 'lastname',
-        'following_count': 'followingCount',
-        'organization': 'organization',
-        'type': 'type',
-        'registration_date': 'registrationDate'
+    allowed_values = {
     }
 
-    def __init__(self, username=None, class_role=None, private_profile=None, followers_count=None, firstname=None, is_power_user=None, locale=None, instruments=None, html_url=None, liked_scores_count=None, printable_name=None, bio=None, picture_file=None, id=None, cover_picture_file=None, picture=None, name=None, is_flat_team=None, organization_role=None, profile_theme=None, cover_picture=None, owned_public_scores_count=None, lastname=None, following_count=None, organization=None, type=None, registration_date=None, local_vars_configuration=None):  # noqa: E501
-        """UserDetails - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._username = None
-        self._class_role = None
-        self._private_profile = None
-        self._followers_count = None
-        self._firstname = None
-        self._is_power_user = None
-        self._locale = None
-        self._instruments = None
-        self._html_url = None
-        self._liked_scores_count = None
-        self._printable_name = None
-        self._bio = None
-        self._picture_file = None
-        self._id = None
-        self._cover_picture_file = None
-        self._picture = None
-        self._name = None
-        self._is_flat_team = None
-        self._organization_role = None
-        self._profile_theme = None
-        self._cover_picture = None
-        self._owned_public_scores_count = None
-        self._lastname = None
-        self._following_count = None
-        self._organization = None
-        self._type = None
-        self._registration_date = None
-        self.discriminator = None
-
-        if username is not None:
-            self.username = username
-        if class_role is not None:
-            self.class_role = class_role
-        if private_profile is not None:
-            self.private_profile = private_profile
-        if followers_count is not None:
-            self.followers_count = followers_count
-        if firstname is not None:
-            self.firstname = firstname
-        if is_power_user is not None:
-            self.is_power_user = is_power_user
-        if locale is not None:
-            self.locale = locale
-        if instruments is not None:
-            self.instruments = instruments
-        if html_url is not None:
-            self.html_url = html_url
-        if liked_scores_count is not None:
-            self.liked_scores_count = liked_scores_count
-        if printable_name is not None:
-            self.printable_name = printable_name
-        if bio is not None:
-            self.bio = bio
-        self.picture_file = picture_file
-        if id is not None:
-            self.id = id
-        self.cover_picture_file = cover_picture_file
-        self.picture = picture
-        if name is not None:
-            self.name = name
-        if is_flat_team is not None:
-            self.is_flat_team = is_flat_team
-        if organization_role is not None:
-            self.organization_role = organization_role
-        if profile_theme is not None:
-            self.profile_theme = profile_theme
-        if cover_picture is not None:
-            self.cover_picture = cover_picture
-        if owned_public_scores_count is not None:
-            self.owned_public_scores_count = owned_public_scores_count
-        if lastname is not None:
-            self.lastname = lastname
-        if following_count is not None:
-            self.following_count = following_count
-        if organization is not None:
-            self.organization = organization
-        if type is not None:
-            self.type = type
-        if registration_date is not None:
-            self.registration_date = registration_date
-
-    @property
-    def username(self):
-        """Gets the username of this UserDetails.  # noqa: E501
-
-        The user name (unique for the organization)  # noqa: E501
-
-        :return: The username of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._username
-
-    @username.setter
-    def username(self, username):
-        """Sets the username of this UserDetails.
-
-        The user name (unique for the organization)  # noqa: E501
-
-        :param username: The username of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._username = username
-
-    @property
-    def class_role(self):
-        """Gets the class_role of this UserDetails.  # noqa: E501
-
-
-        :return: The class_role of this UserDetails.  # noqa: E501
-        :rtype: ClassRoles
-        """
-        return self._class_role
-
-    @class_role.setter
-    def class_role(self, class_role):
-        """Sets the class_role of this UserDetails.
-
-
-        :param class_role: The class_role of this UserDetails.  # noqa: E501
-        :type: ClassRoles
-        """
-
-        self._class_role = class_role
-
-    @property
-    def private_profile(self):
-        """Gets the private_profile of this UserDetails.  # noqa: E501
-
-        Tell either this user profile is private or not (individual accounts only)  # noqa: E501
-
-        :return: The private_profile of this UserDetails.  # noqa: E501
-        :rtype: bool
-        """
-        return self._private_profile
-
-    @private_profile.setter
-    def private_profile(self, private_profile):
-        """Sets the private_profile of this UserDetails.
-
-        Tell either this user profile is private or not (individual accounts only)  # noqa: E501
-
-        :param private_profile: The private_profile of this UserDetails.  # noqa: E501
-        :type: bool
-        """
-
-        self._private_profile = private_profile
-
-    @property
-    def followers_count(self):
-        """Gets the followers_count of this UserDetails.  # noqa: E501
-
-        Number of followers the user have  # noqa: E501
-
-        :return: The followers_count of this UserDetails.  # noqa: E501
-        :rtype: int
-        """
-        return self._followers_count
-
-    @followers_count.setter
-    def followers_count(self, followers_count):
-        """Sets the followers_count of this UserDetails.
-
-        Number of followers the user have  # noqa: E501
-
-        :param followers_count: The followers_count of this UserDetails.  # noqa: E501
-        :type: int
-        """
-
-        self._followers_count = followers_count
-
-    @property
-    def firstname(self):
-        """Gets the firstname of this UserDetails.  # noqa: E501
-
-        Firstname of the user (for education users)  # noqa: E501
-
-        :return: The firstname of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._firstname
-
-    @firstname.setter
-    def firstname(self, firstname):
-        """Sets the firstname of this UserDetails.
-
-        Firstname of the user (for education users)  # noqa: E501
-
-        :param firstname: The firstname of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._firstname = firstname
-
-    @property
-    def is_power_user(self):
-        """Gets the is_power_user of this UserDetails.  # noqa: E501
-
-        User license status. 'true' if user is an individual Power user  # noqa: E501
-
-        :return: The is_power_user of this UserDetails.  # noqa: E501
-        :rtype: bool
-        """
-        return self._is_power_user
-
-    @is_power_user.setter
-    def is_power_user(self, is_power_user):
-        """Sets the is_power_user of this UserDetails.
-
-        User license status. 'true' if user is an individual Power user  # noqa: E501
-
-        :param is_power_user: The is_power_user of this UserDetails.  # noqa: E501
-        :type: bool
-        """
-
-        self._is_power_user = is_power_user
-
-    @property
-    def locale(self):
-        """Gets the locale of this UserDetails.  # noqa: E501
-
-
-        :return: The locale of this UserDetails.  # noqa: E501
-        :rtype: FlatLocales
-        """
-        return self._locale
-
-    @locale.setter
-    def locale(self, locale):
-        """Sets the locale of this UserDetails.
-
-
-        :param locale: The locale of this UserDetails.  # noqa: E501
-        :type: FlatLocales
-        """
-
-        self._locale = locale
-
-    @property
-    def instruments(self):
-        """Gets the instruments of this UserDetails.  # noqa: E501
-
-        An array of the instrument identifiers. The format of the strings is `{instrument-group}.{instrument-id}`.   # noqa: E501
-
-        :return: The instruments of this UserDetails.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._instruments
-
-    @instruments.setter
-    def instruments(self, instruments):
-        """Sets the instruments of this UserDetails.
-
-        An array of the instrument identifiers. The format of the strings is `{instrument-group}.{instrument-id}`.   # noqa: E501
-
-        :param instruments: The instruments of this UserDetails.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._instruments = instruments
-
-    @property
-    def html_url(self):
-        """Gets the html_url of this UserDetails.  # noqa: E501
-
-        Link to user profile (for Indiv. users only)  # noqa: E501
-
-        :return: The html_url of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._html_url
-
-    @html_url.setter
-    def html_url(self, html_url):
-        """Sets the html_url of this UserDetails.
-
-        Link to user profile (for Indiv. users only)  # noqa: E501
-
-        :param html_url: The html_url of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._html_url = html_url
-
-    @property
-    def liked_scores_count(self):
-        """Gets the liked_scores_count of this UserDetails.  # noqa: E501
-
-        Number of the scores liked by the user  # noqa: E501
-
-        :return: The liked_scores_count of this UserDetails.  # noqa: E501
-        :rtype: int
-        """
-        return self._liked_scores_count
-
-    @liked_scores_count.setter
-    def liked_scores_count(self, liked_scores_count):
-        """Sets the liked_scores_count of this UserDetails.
-
-        Number of the scores liked by the user  # noqa: E501
-
-        :param liked_scores_count: The liked_scores_count of this UserDetails.  # noqa: E501
-        :type: int
-        """
-
-        self._liked_scores_count = liked_scores_count
-
-    @property
-    def printable_name(self):
-        """Gets the printable_name of this UserDetails.  # noqa: E501
-
-        The name that can be directly printed (name, firstname & lastname, or username)  # noqa: E501
-
-        :return: The printable_name of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._printable_name
-
-    @printable_name.setter
-    def printable_name(self, printable_name):
-        """Sets the printable_name of this UserDetails.
-
-        The name that can be directly printed (name, firstname & lastname, or username)  # noqa: E501
-
-        :param printable_name: The printable_name of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._printable_name = printable_name
-
-    @property
-    def bio(self):
-        """Gets the bio of this UserDetails.  # noqa: E501
-
-        User's biography  # noqa: E501
-
-        :return: The bio of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._bio
-
-    @bio.setter
-    def bio(self, bio):
-        """Sets the bio of this UserDetails.
-
-        User's biography  # noqa: E501
-
-        :param bio: The bio of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._bio = bio
-
-    @property
-    def picture_file(self):
-        """Gets the picture_file of this UserDetails.  # noqa: E501
-
-        The ID of the user profile picture  # noqa: E501
-
-        :return: The picture_file of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._picture_file
-
-    @picture_file.setter
-    def picture_file(self, picture_file):
-        """Sets the picture_file of this UserDetails.
-
-        The ID of the user profile picture  # noqa: E501
-
-        :param picture_file: The picture_file of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._picture_file = picture_file
-
-    @property
-    def id(self):
-        """Gets the id of this UserDetails.  # noqa: E501
-
-        Identifier of the user  # noqa: E501
-
-        :return: The id of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this UserDetails.
-
-        Identifier of the user  # noqa: E501
-
-        :param id: The id of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._id = id
-
-    @property
-    def cover_picture_file(self):
-        """Gets the cover_picture_file of this UserDetails.  # noqa: E501
-
-        The ID of the user profile cover picture  # noqa: E501
-
-        :return: The cover_picture_file of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._cover_picture_file
-
-    @cover_picture_file.setter
-    def cover_picture_file(self, cover_picture_file):
-        """Sets the cover_picture_file of this UserDetails.
-
-        The ID of the user profile cover picture  # noqa: E501
-
-        :param cover_picture_file: The cover_picture_file of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._cover_picture_file = cover_picture_file
-
-    @property
-    def picture(self):
-        """Gets the picture of this UserDetails.  # noqa: E501
-
-        The URL of the picture to display  # noqa: E501
-
-        :return: The picture of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._picture
-
-    @picture.setter
-    def picture(self, picture):
-        """Sets the picture of this UserDetails.
-
-        The URL of the picture to display  # noqa: E501
-
-        :param picture: The picture of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._picture = picture
-
-    @property
-    def name(self):
-        """Gets the name of this UserDetails.  # noqa: E501
-
-        A displayable name for the user (for consumer users)  # noqa: E501
-
-        :return: The name of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this UserDetails.
-
-        A displayable name for the user (for consumer users)  # noqa: E501
-
-        :param name: The name of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._name = name
-
-    @property
-    def is_flat_team(self):
-        """Gets the is_flat_team of this UserDetails.  # noqa: E501
-
-        Will be 'true' if user is part of the Flat Team  # noqa: E501
-
-        :return: The is_flat_team of this UserDetails.  # noqa: E501
-        :rtype: bool
-        """
-        return self._is_flat_team
-
-    @is_flat_team.setter
-    def is_flat_team(self, is_flat_team):
-        """Sets the is_flat_team of this UserDetails.
-
-        Will be 'true' if user is part of the Flat Team  # noqa: E501
-
-        :param is_flat_team: The is_flat_team of this UserDetails.  # noqa: E501
-        :type: bool
-        """
-
-        self._is_flat_team = is_flat_team
-
-    @property
-    def organization_role(self):
-        """Gets the organization_role of this UserDetails.  # noqa: E501
-
-
-        :return: The organization_role of this UserDetails.  # noqa: E501
-        :rtype: OrganizationRoles
-        """
-        return self._organization_role
-
-    @organization_role.setter
-    def organization_role(self, organization_role):
-        """Sets the organization_role of this UserDetails.
-
-
-        :param organization_role: The organization_role of this UserDetails.  # noqa: E501
-        :type: OrganizationRoles
-        """
-
-        self._organization_role = organization_role
-
-    @property
-    def profile_theme(self):
-        """Gets the profile_theme of this UserDetails.  # noqa: E501
-
-        Theme (background) for the profile  # noqa: E501
-
-        :return: The profile_theme of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._profile_theme
-
-    @profile_theme.setter
-    def profile_theme(self, profile_theme):
-        """Sets the profile_theme of this UserDetails.
-
-        Theme (background) for the profile  # noqa: E501
-
-        :param profile_theme: The profile_theme of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._profile_theme = profile_theme
-
-    @property
-    def cover_picture(self):
-        """Gets the cover_picture of this UserDetails.  # noqa: E501
-
-        Cover picture (backgroud) for the profile  # noqa: E501
-
-        :return: The cover_picture of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._cover_picture
-
-    @cover_picture.setter
-    def cover_picture(self, cover_picture):
-        """Sets the cover_picture of this UserDetails.
-
-        Cover picture (backgroud) for the profile  # noqa: E501
-
-        :param cover_picture: The cover_picture of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._cover_picture = cover_picture
-
-    @property
-    def owned_public_scores_count(self):
-        """Gets the owned_public_scores_count of this UserDetails.  # noqa: E501
-
-        Number of public scores the user have  # noqa: E501
-
-        :return: The owned_public_scores_count of this UserDetails.  # noqa: E501
-        :rtype: int
-        """
-        return self._owned_public_scores_count
-
-    @owned_public_scores_count.setter
-    def owned_public_scores_count(self, owned_public_scores_count):
-        """Sets the owned_public_scores_count of this UserDetails.
-
-        Number of public scores the user have  # noqa: E501
-
-        :param owned_public_scores_count: The owned_public_scores_count of this UserDetails.  # noqa: E501
-        :type: int
-        """
-
-        self._owned_public_scores_count = owned_public_scores_count
-
-    @property
-    def lastname(self):
-        """Gets the lastname of this UserDetails.  # noqa: E501
-
-        Lastname of the user (for education users)  # noqa: E501
-
-        :return: The lastname of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._lastname
-
-    @lastname.setter
-    def lastname(self, lastname):
-        """Sets the lastname of this UserDetails.
-
-        Lastname of the user (for education users)  # noqa: E501
-
-        :param lastname: The lastname of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._lastname = lastname
-
-    @property
-    def following_count(self):
-        """Gets the following_count of this UserDetails.  # noqa: E501
-
-        Number of people the user follow  # noqa: E501
-
-        :return: The following_count of this UserDetails.  # noqa: E501
-        :rtype: int
-        """
-        return self._following_count
-
-    @following_count.setter
-    def following_count(self, following_count):
-        """Sets the following_count of this UserDetails.
-
-        Number of people the user follow  # noqa: E501
-
-        :param following_count: The following_count of this UserDetails.  # noqa: E501
-        :type: int
-        """
-
-        self._following_count = following_count
-
-    @property
-    def organization(self):
-        """Gets the organization of this UserDetails.  # noqa: E501
-
-        Organization ID (for Edu users only)  # noqa: E501
-
-        :return: The organization of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._organization
-
-    @organization.setter
-    def organization(self, organization):
-        """Sets the organization of this UserDetails.
-
-        Organization ID (for Edu users only)  # noqa: E501
-
-        :param organization: The organization of this UserDetails.  # noqa: E501
-        :type: str
-        """
-
-        self._organization = organization
-
-    @property
-    def type(self):
-        """Gets the type of this UserDetails.  # noqa: E501
-
-        The type of account  # noqa: E501
-
-        :return: The type of this UserDetails.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this UserDetails.
-
-        The type of account  # noqa: E501
+    validations = {
+    }
 
-        :param type: The type of this UserDetails.  # noqa: E501
-        :type: str
+    @cached_property
+    def additional_properties_type():
         """
-        allowed_values = ["user", "guest"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
-
-        self._type = type
-
-    @property
-    def registration_date(self):
-        """Gets the registration_date of this UserDetails.  # noqa: E501
-
-        Date the user signed up  # noqa: E501
-
-        :return: The registration_date of this UserDetails.  # noqa: E501
-        :rtype: datetime
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
         """
-        return self._registration_date
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    @registration_date.setter
-    def registration_date(self, registration_date):
-        """Sets the registration_date of this UserDetails.
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (str,),  # noqa: E501
+            'sharing_key': (str,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'privacy': (ScorePrivacy,),  # noqa: E501
+            'user': (UserPublicSummary,),  # noqa: E501
+            'html_url': (str,),  # noqa: E501
+            'subtitle': (str,),  # noqa: E501
+            'lyricist': (str,),  # noqa: E501
+            'arranger': (str,),  # noqa: E501
+            'composer': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'tags': ([str],),  # noqa: E501
+            'creation_type': (ScoreCreationType,),  # noqa: E501
+            'license': (ScoreLicense,),  # noqa: E501
+            'license_text': (str,),  # noqa: E501
+            'duration_time': (float,),  # noqa: E501
+            'number_measures': (int,),  # noqa: E501
+            'main_tempo_qpm': (float,),  # noqa: E501
+            'rights': (ResourceRights,),  # noqa: E501
+            'collaborators': ([ResourceCollaborator],),  # noqa: E501
+            'creation_date': (datetime,),  # noqa: E501
+            'modification_date': (datetime,),  # noqa: E501
+            'publication_date': (datetime,),  # noqa: E501
+            'organization': (str,),  # noqa: E501
+            'parent_score': (str,),  # noqa: E501
+            'instruments': ([str],),  # noqa: E501
+            'samples': ([str],),  # noqa: E501
+            'google_drive_file_id': (str,),  # noqa: E501
+            'likes': (ScoreLikesCounts,),  # noqa: E501
+            'comments': (ScoreCommentsCounts,),  # noqa: E501
+            'views': (ScoreViewsCounts,),  # noqa: E501
+            'plays': (ScorePlaysCounts,),  # noqa: E501
+            'collections': ([str],),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
 
-        Date the user signed up  # noqa: E501
 
-        :param registration_date: The registration_date of this UserDetails.  # noqa: E501
-        :type: datetime
-        """
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'sharing_key': 'sharingKey',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'privacy': 'privacy',  # noqa: E501
+        'user': 'user',  # noqa: E501
+        'html_url': 'htmlUrl',  # noqa: E501
+        'subtitle': 'subtitle',  # noqa: E501
+        'lyricist': 'lyricist',  # noqa: E501
+        'arranger': 'arranger',  # noqa: E501
+        'composer': 'composer',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
+        'creation_type': 'creationType',  # noqa: E501
+        'license': 'license',  # noqa: E501
+        'license_text': 'licenseText',  # noqa: E501
+        'duration_time': 'durationTime',  # noqa: E501
+        'number_measures': 'numberMeasures',  # noqa: E501
+        'main_tempo_qpm': 'mainTempoQpm',  # noqa: E501
+        'rights': 'rights',  # noqa: E501
+        'collaborators': 'collaborators',  # noqa: E501
+        'creation_date': 'creationDate',  # noqa: E501
+        'modification_date': 'modificationDate',  # noqa: E501
+        'publication_date': 'publicationDate',  # noqa: E501
+        'organization': 'organization',  # noqa: E501
+        'parent_score': 'parentScore',  # noqa: E501
+        'instruments': 'instruments',  # noqa: E501
+        'samples': 'samples',  # noqa: E501
+        'google_drive_file_id': 'googleDriveFileId',  # noqa: E501
+        'likes': 'likes',  # noqa: E501
+        'comments': 'comments',  # noqa: E501
+        'views': 'views',  # noqa: E501
+        'plays': 'plays',  # noqa: E501
+        'collections': 'collections',  # noqa: E501
+    }
 
-        self._registration_date = registration_date
+    read_only_vars = {
+    }
 
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, UserDetails):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, UserDetails):
-            return True
+    _composed_schemas = {}
 
-        return self.to_dict() != other.to_dict()
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ScoreDetails - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (str): The unique identifier of the score. [optional]  # noqa: E501
+            sharing_key (str): The private sharing key of the score (available when the `privacy` mode is set to `privateLink`). [optional]  # noqa: E501
+            title (str): The title of the score. [optional]  # noqa: E501
+            privacy (ScorePrivacy): [optional]  # noqa: E501
+            user (UserPublicSummary): [optional]  # noqa: E501
+            html_url (str): The url where the score can be viewed in a web browser. [optional]  # noqa: E501
+            subtitle (str): Subtitle of the score. [optional]  # noqa: E501
+            lyricist (str): Lyricist of the score. [optional]  # noqa: E501
+            arranger (str): Arranger of the score. [optional]  # noqa: E501
+            composer (str): Composer of the score. [optional]  # noqa: E501
+            description (str): Description of the creation. [optional]  # noqa: E501
+            tags ([str]): Tags describing the score. [optional]  # noqa: E501
+            creation_type (ScoreCreationType): [optional]  # noqa: E501
+            license (ScoreLicense): [optional]  # noqa: E501
+            license_text (str): Additional license text written on the exported/printed score. [optional]  # noqa: E501
+            duration_time (float): In seconds, an approximative duration of the score. [optional]  # noqa: E501
+            number_measures (int): The number of measures in the score. [optional]  # noqa: E501
+            main_tempo_qpm (float): The main tempo of the score (in QPM). [optional]  # noqa: E501
+            rights (ResourceRights): [optional]  # noqa: E501
+            collaborators ([ResourceCollaborator]): The list of the collaborators of the score. [optional]  # noqa: E501
+            creation_date (datetime): The date when the score was created. [optional]  # noqa: E501
+            modification_date (datetime): The date of the last revision of the score. [optional]  # noqa: E501
+            publication_date (datetime): The date when the score was published on Flat. [optional]  # noqa: E501
+            organization (str): If the score has been created in an organization, the identifier of this organization. This property is especially used with the score privacy `organizationPublic`. . [optional]  # noqa: E501
+            parent_score (str): If the score has been forked, the unique identifier of the parent score. . [optional]  # noqa: E501
+            instruments ([str]): An array of the instrument identifiers used in the last version of the score. This is mainly used to display a list of the instruments in the Flat's UI or instruments icons. The format of the strings is `{instrument-group}.{instrument-id}`. . [optional]  # noqa: E501
+            samples ([str]): An array of the audio samples identifiers used the different score parts. The format of the strings is `{instrument-group}.{sample-id}`. . [optional]  # noqa: E501
+            google_drive_file_id (str): If the user uses Google Drive and the score exists on Google Drive, this field will contain the unique identifier of the Flat score on Google Drive. You can access the document using the url: `https://drive.google.com/open?id={googleDriveFileId}` . [optional]  # noqa: E501
+            likes (ScoreLikesCounts): [optional]  # noqa: E501
+            comments (ScoreCommentsCounts): [optional]  # noqa: E501
+            views (ScoreViewsCounts): [optional]  # noqa: E501
+            plays (ScorePlaysCounts): [optional]  # noqa: E501
+            collections ([str]): The List of parent collections, which includes all the collections this score is included. Please note that you might not have access to all of them.. [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ScoreDetails - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            id (str): The unique identifier of the score. [optional]  # noqa: E501
+            sharing_key (str): The private sharing key of the score (available when the `privacy` mode is set to `privateLink`). [optional]  # noqa: E501
+            title (str): The title of the score. [optional]  # noqa: E501
+            privacy (ScorePrivacy): [optional]  # noqa: E501
+            user (UserPublicSummary): [optional]  # noqa: E501
+            html_url (str): The url where the score can be viewed in a web browser. [optional]  # noqa: E501
+            subtitle (str): Subtitle of the score. [optional]  # noqa: E501
+            lyricist (str): Lyricist of the score. [optional]  # noqa: E501
+            arranger (str): Arranger of the score. [optional]  # noqa: E501
+            composer (str): Composer of the score. [optional]  # noqa: E501
+            description (str): Description of the creation. [optional]  # noqa: E501
+            tags ([str]): Tags describing the score. [optional]  # noqa: E501
+            creation_type (ScoreCreationType): [optional]  # noqa: E501
+            license (ScoreLicense): [optional]  # noqa: E501
+            license_text (str): Additional license text written on the exported/printed score. [optional]  # noqa: E501
+            duration_time (float): In seconds, an approximative duration of the score. [optional]  # noqa: E501
+            number_measures (int): The number of measures in the score. [optional]  # noqa: E501
+            main_tempo_qpm (float): The main tempo of the score (in QPM). [optional]  # noqa: E501
+            rights (ResourceRights): [optional]  # noqa: E501
+            collaborators ([ResourceCollaborator]): The list of the collaborators of the score. [optional]  # noqa: E501
+            creation_date (datetime): The date when the score was created. [optional]  # noqa: E501
+            modification_date (datetime): The date of the last revision of the score. [optional]  # noqa: E501
+            publication_date (datetime): The date when the score was published on Flat. [optional]  # noqa: E501
+            organization (str): If the score has been created in an organization, the identifier of this organization. This property is especially used with the score privacy `organizationPublic`. . [optional]  # noqa: E501
+            parent_score (str): If the score has been forked, the unique identifier of the parent score. . [optional]  # noqa: E501
+            instruments ([str]): An array of the instrument identifiers used in the last version of the score. This is mainly used to display a list of the instruments in the Flat's UI or instruments icons. The format of the strings is `{instrument-group}.{instrument-id}`. . [optional]  # noqa: E501
+            samples ([str]): An array of the audio samples identifiers used the different score parts. The format of the strings is `{instrument-group}.{sample-id}`. . [optional]  # noqa: E501
+            google_drive_file_id (str): If the user uses Google Drive and the score exists on Google Drive, this field will contain the unique identifier of the Flat score on Google Drive. You can access the document using the url: `https://drive.google.com/open?id={googleDriveFileId}` . [optional]  # noqa: E501
+            likes (ScoreLikesCounts): [optional]  # noqa: E501
+            comments (ScoreCommentsCounts): [optional]  # noqa: E501
+            views (ScoreViewsCounts): [optional]  # noqa: E501
+            plays (ScorePlaysCounts): [optional]  # noqa: E501
+            collections ([str]): The List of parent collections, which includes all the collections this score is included. Please note that you might not have access to all of them.. [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            for arg in args:
+                if isinstance(arg, dict):
+                    kwargs.update(arg)
+                else:
+                    raise ApiTypeError(
+                        "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                            args,
+                            self.__class__.__name__,
+                        ),
+                        path_to_item=_path_to_item,
+                        valid_classes=(self.__class__,),
+                    )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `flat_api-0.8.1/flat_api/rest.py` & `flat_api-1.0.0/flat_api/rest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    The version of the OpenAPI document: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import io
 import json
 import logging
 import re
 import ssl
-
-import certifi
-# python 2 and python 3 compatibility library
-import six
-from six.moves.urllib.parse import urlencode
+from urllib.parse import urlencode
+from urllib.parse import urlparse
+from urllib.request import proxy_bypass_environment
 import urllib3
+import ipaddress
 
-from flat_api.exceptions import ApiException, ApiValueError
+from flat_api.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
 
@@ -59,53 +54,50 @@
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        # ca_certs
-        if configuration.ssl_ca_cert:
-            ca_certs = configuration.ssl_ca_cert
-        else:
-            # if not set certificate file, use Mozilla's root certificates.
-            ca_certs = certifi.where()
-
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
-        if configuration.proxy:
+        if configuration.proxy and not should_bypass_proxies(
+                configuration.host, no_proxy=configuration.no_proxy or ''):
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
                 **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
@@ -138,30 +130,31 @@
             )
 
         post_params = post_params or {}
         headers = headers or {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif (isinstance(_request_timeout, tuple) and
                   len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
                     connect=_request_timeout[0], read=_request_timeout[1])
 
-        if 'Content-Type' not in headers:
-            headers['Content-Type'] = 'application/json'
-
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
+                if (method != 'DELETE') and ('Content-Type' not in headers):
+                    headers['Content-Type'] = 'application/json'
                 if query_params:
                     url += '?' + urlencode(query_params)
-                if re.search('json', headers['Content-Type'], re.IGNORECASE):
+                if ('Content-Type' not in headers) or (re.search('json',
+                                                                 headers['Content-Type'], re.IGNORECASE)):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
@@ -218,14 +211,26 @@
         if _preload_content:
             r = RESTResponse(r)
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
             raise ApiException(http_resp=r)
 
         return r
 
     def GET(self, url, headers=None, query_params=None, _preload_content=True,
             _request_timeout=None):
         return self.request("GET", url,
@@ -286,7 +291,63 @@
         return self.request("PATCH", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
+
+# end of class RESTClientObject
+
+
+def is_ipv4(target):
+    """ Test if IPv4 address or not
+    """
+    try:
+        chk = ipaddress.IPv4Address(target)
+        return True
+    except ipaddress.AddressValueError:
+        return False
+
+
+def in_ipv4net(target, net):
+    """ Test if target belongs to given IPv4 network
+    """
+    try:
+        nw = ipaddress.IPv4Network(net)
+        ip = ipaddress.IPv4Address(target)
+        if ip in nw:
+            return True
+        return False
+    except ipaddress.AddressValueError:
+        return False
+    except ipaddress.NetmaskValueError:
+        return False
+
+
+def should_bypass_proxies(url, no_proxy=None):
+    """ Yet another requests.should_bypass_proxies
+    Test if proxies should not be used for a particular url.
+    """
+
+    parsed = urlparse(url)
+
+    # special cases
+    if parsed.hostname in [None, '']:
+        return True
+
+    # special cases
+    if no_proxy in [None, '']:
+        return False
+    if no_proxy == '*':
+        return True
+
+    no_proxy = no_proxy.lower().replace(' ', '');
+    entries = (
+        host for host in no_proxy.split(',') if host
+    )
+
+    if is_ipv4(parsed.hostname):
+        for item in entries:
+            if in_ipv4net(parsed.hostname, item):
+                return True
+    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy})
```

### Comparing `flat_api-0.8.1/flat_api.egg-info/PKG-INFO` & `flat_api-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: flat-api
-Version: 0.8.1
+Name: flat_api
+Version: 1.0.0
 Summary: Flat API Client
 Home-page: https://github.com/FlatIO/api-client-python
 Author: The Flat Team (https://flat.io)
 Author-email: developers@flat.io
 License: Apache
 Keywords: Flat API,MusicXML,Music Notation,MIDI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
@@ -25,36 +24,38 @@
 Classifier: Topic :: Education
 Classifier: Topic :: Multimedia :: Sound/Audio
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Client for the Flat REST API
 
-[![Python package](https://github.com/FlatIO/api-client-python/actions/workflows/python-package.yml/badge.svg)](https://github.com/FlatIO/api-client-python/actions/workflows/python-package.yml)
+[![Python package](https://github.com/FlatIO/api-client-python/actions/workflows/python.yml/badge.svg)](https://github.com/FlatIO/api-client-python/actions/workflows/python.yml)
 
 The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:
 - Creating and importing new music scores using MusicXML or MIDI files
 - Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI)
 - Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.
 
 You can find the API reference including code samples and our OpenAPI Specification at the following url: [https://flat.io/developers/api/reference](https://flat.io/developers/api/reference).
 
 To request some API credentials, please visit [https://flat.io/developers](https://flat.io/developers).
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python >= 3.7
 
 ## Installation & Usage
 ### pip install
 
 ```sh
 pip install flat_api
 ```
 
+or install from this repository
+
 ```sh
 pip install git+https://github.com/FlatIO/api-client-python.git
 ```
 
 Then import the package:
 ```python
 import flat_api
@@ -75,60 +76,58 @@
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from __future__ import print_function
-import time
-import flat_api
-from flat_api.rest import ApiException
 from pprint import pprint
+import flat_api
+from flat_api.api import account_api
 
-# Configure OAuth2 access token for authorization: OAuth2
-configuration = flat_api.Configuration()
-configuration.access_token = 'YOUR_ACCESS_TOKEN'
-
-# create an instance of the API class
-api_instance = flat_api.AccountApi(flat_api.ApiClient(configuration))
-only_id = False # bool | Only return the user id (optional) (default to False)
-
-try:
-    # Get current user profile
-    api_response = api_instance.get_authenticated_user(only_id=only_id)
-    pprint(api_response)
-except ApiException as e:
-    print("Exception when calling AccountApi->get_authenticated_user: %s\n" % e)
-
+configuration = flat_api.Configuration(
+    access_token = 'YOUR_ACCESS_TOKEN'
+)
+
+# Enter a context with an instance of the API client
+with flat_api.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = account_api.AccountApi(api_client)
+
+    try:
+        # Get current user account
+        api_response = api_instance.get_authenticated_user()
+        pprint(api_response)
+    except flat_api.ApiException as e:
+        print("Exception when calling AccountApi->get_authenticated_user: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.flat.io/v2*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AccountApi* | [**get_authenticated_user**](docs/AccountApi.md#get_authenticated_user) | **GET** /me | Get current user profile
+*AccountApi* | [**get_authenticated_user**](docs/AccountApi.md#get_authenticated_user) | **GET** /me | Get current user account
 *ClassApi* | [**activate_class**](docs/ClassApi.md#activate_class) | **POST** /classes/{class}/activate | Activate the class
 *ClassApi* | [**add_class_user**](docs/ClassApi.md#add_class_user) | **PUT** /classes/{class}/users/{user} | Add a user to the class
 *ClassApi* | [**archive_assignment**](docs/ClassApi.md#archive_assignment) | **POST** /classes/{class}/assignments/{assignment}/archive | Archive the assignment
 *ClassApi* | [**archive_class**](docs/ClassApi.md#archive_class) | **POST** /classes/{class}/archive | Archive the class
 *ClassApi* | [**copy_assignment**](docs/ClassApi.md#copy_assignment) | **POST** /classes/{class}/assignments/{assignment}/copy | Copy an assignment
-*ClassApi* | [**create_assignment**](docs/ClassApi.md#create_assignment) | **POST** /classes/{class}/assignments | Assignment creation
 *ClassApi* | [**create_class**](docs/ClassApi.md#create_class) | **POST** /classes | Create a new class
+*ClassApi* | [**create_class_assignment**](docs/ClassApi.md#create_class_assignment) | **POST** /classes/{class}/assignments | Assignment creation
 *ClassApi* | [**create_submission**](docs/ClassApi.md#create_submission) | **PUT** /classes/{class}/assignments/{assignment}/submissions | Create or edit a submission
+*ClassApi* | [**create_test_student_account**](docs/ClassApi.md#create_test_student_account) | **POST** /classes/{class}/testStudent | Create a test student account
 *ClassApi* | [**delete_class_user**](docs/ClassApi.md#delete_class_user) | **DELETE** /classes/{class}/users/{user} | Remove a user from the class
-*ClassApi* | [**delete_submission**](docs/ClassApi.md#delete_submission) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission} | Delete a submission
+*ClassApi* | [**delete_submission**](docs/ClassApi.md#delete_submission) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission} | Reset a submission
 *ClassApi* | [**delete_submission_comment**](docs/ClassApi.md#delete_submission_comment) | **DELETE** /classes/{class}/assignments/{assignment}/submissions/{submission}/comments/{comment} | Delete a feedback comment to a submission
 *ClassApi* | [**edit_submission**](docs/ClassApi.md#edit_submission) | **PUT** /classes/{class}/assignments/{assignment}/submissions/{submission} | Edit a submission
 *ClassApi* | [**enroll_class**](docs/ClassApi.md#enroll_class) | **POST** /classes/enroll/{enrollmentCode} | Join a class
 *ClassApi* | [**export_submissions_reviews_as_csv**](docs/ClassApi.md#export_submissions_reviews_as_csv) | **GET** /classes/{class}/assignments/{assignment}/submissions/csv | CSV Grades exports
 *ClassApi* | [**export_submissions_reviews_as_excel**](docs/ClassApi.md#export_submissions_reviews_as_excel) | **GET** /classes/{class}/assignments/{assignment}/submissions/excel | Excel Grades exports
-*ClassApi* | [**fork_score**](docs/ClassApi.md#fork_score) | **POST** /scores/{score}/fork | Fork a score
 *ClassApi* | [**get_class**](docs/ClassApi.md#get_class) | **GET** /classes/{class} | Get the details of a single class
 *ClassApi* | [**get_score_submissions**](docs/ClassApi.md#get_score_submissions) | **GET** /scores/{score}/submissions | List submissions related to the score
 *ClassApi* | [**get_submission**](docs/ClassApi.md#get_submission) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission} | Get a student submission
 *ClassApi* | [**get_submission_comments**](docs/ClassApi.md#get_submission_comments) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission}/comments | List the feedback comments of a submission
 *ClassApi* | [**get_submission_history**](docs/ClassApi.md#get_submission_history) | **GET** /classes/{class}/assignments/{assignment}/submissions/{submission}/history | Get the history of the submission
 *ClassApi* | [**get_submissions**](docs/ClassApi.md#get_submissions) | **GET** /classes/{class}/assignments/{assignment}/submissions | List the students&#39; submissions
 *ClassApi* | [**list_assignments**](docs/ClassApi.md#list_assignments) | **GET** /classes/{class}/assignments | Assignments listing
@@ -144,14 +143,25 @@
 *CollectionApi* | [**delete_collection**](docs/CollectionApi.md#delete_collection) | **DELETE** /collections/{collection} | Delete the collection
 *CollectionApi* | [**delete_score_from_collection**](docs/CollectionApi.md#delete_score_from_collection) | **DELETE** /collections/{collection}/scores/{score} | Delete a score from the collection
 *CollectionApi* | [**edit_collection**](docs/CollectionApi.md#edit_collection) | **PUT** /collections/{collection} | Update a collection&#39;s metadata
 *CollectionApi* | [**get_collection**](docs/CollectionApi.md#get_collection) | **GET** /collections/{collection} | Get collection details
 *CollectionApi* | [**list_collection_scores**](docs/CollectionApi.md#list_collection_scores) | **GET** /collections/{collection}/scores | List the scores contained in a collection
 *CollectionApi* | [**list_collections**](docs/CollectionApi.md#list_collections) | **GET** /collections | List the collections
 *CollectionApi* | [**untrash_collection**](docs/CollectionApi.md#untrash_collection) | **POST** /collections/{collection}/untrash | Untrash a collection
+*EduResourcesApi* | [**copy_edu_resource**](docs/EduResourcesApi.md#copy_edu_resource) | **POST** /eduResources/{resource}/copy | Copy an education resource to a Resource Library
+*EduResourcesApi* | [**copy_edu_resource_to_demo_class**](docs/EduResourcesApi.md#copy_edu_resource_to_demo_class) | **POST** /eduResources/{resource}/copyToDemoClass | Copy an education assignment to a teacher demo class
+*EduResourcesApi* | [**create_edu_resource**](docs/EduResourcesApi.md#create_edu_resource) | **POST** /eduResources | Create a new education resource
+*EduResourcesApi* | [**delete_edu_resource**](docs/EduResourcesApi.md#delete_edu_resource) | **DELETE** /eduResources/{resource} | Delete an education resource
+*EduResourcesApi* | [**get_edu_resource**](docs/EduResourcesApi.md#get_edu_resource) | **GET** /eduResources/{resource} | Get an education resource
+*EduResourcesApi* | [**list_edu_libraries**](docs/EduResourcesApi.md#list_edu_libraries) | **GET** /eduResources/libraries | List the education libraries
+*EduResourcesApi* | [**list_edu_resources**](docs/EduResourcesApi.md#list_edu_resources) | **GET** /eduResources | List education resources in a library or folder
+*EduResourcesApi* | [**move_edu_resource**](docs/EduResourcesApi.md#move_edu_resource) | **POST** /eduResources/{resource}/move | Move an education resource
+*EduResourcesApi* | [**update_edu_resource**](docs/EduResourcesApi.md#update_edu_resource) | **PUT** /eduResources/{resource} | Update an education resource metadata
+*EduResourcesApi* | [**update_edu_resource_assignment**](docs/EduResourcesApi.md#update_edu_resource_assignment) | **PUT** /eduResources/{resource}/assignment | Update an education resource assignment
+*EduResourcesApi* | [**use_edu_resource_in_class**](docs/EduResourcesApi.md#use_edu_resource_in_class) | **POST** /eduResources/{resource}/useInClass | Use an education resource in a class
 *GroupApi* | [**get_group_details**](docs/GroupApi.md#get_group_details) | **GET** /groups/{group} | Get group information
 *GroupApi* | [**get_group_scores**](docs/GroupApi.md#get_group_scores) | **GET** /groups/{group}/scores | List group&#39;s scores
 *GroupApi* | [**list_group_users**](docs/GroupApi.md#list_group_users) | **GET** /groups/{group}/users | List group&#39;s users
 *OrganizationApi* | [**count_orga_users**](docs/OrganizationApi.md#count_orga_users) | **GET** /organizations/users/count | Count the organization users using the provided filters
 *OrganizationApi* | [**create_lti_credentials**](docs/OrganizationApi.md#create_lti_credentials) | **POST** /organizations/lti/credentials | Create a new couple of LTI 1.x credentials
 *OrganizationApi* | [**create_organization_invitation**](docs/OrganizationApi.md#create_organization_invitation) | **POST** /organizations/invitations | Create a new invitation to join the organization
 *OrganizationApi* | [**create_organization_user**](docs/OrganizationApi.md#create_organization_user) | **POST** /organizations/users | Create a new user account
@@ -201,52 +211,71 @@
 
 
 ## Documentation For Models
 
  - [ApiAccessToken](docs/ApiAccessToken.md)
  - [AppScopes](docs/AppScopes.md)
  - [Assignment](docs/Assignment.md)
- - [AssignmentCanvas](docs/AssignmentCanvas.md)
  - [AssignmentCopy](docs/AssignmentCopy.md)
- - [AssignmentCreation](docs/AssignmentCreation.md)
- - [AssignmentCreationGoogleClassroom](docs/AssignmentCreationGoogleClassroom.md)
- - [AssignmentCreationMicrosoftGraph](docs/AssignmentCreationMicrosoftGraph.md)
- - [AssignmentLti](docs/AssignmentLti.md)
- - [AssignmentMfc](docs/AssignmentMfc.md)
+ - [AssignmentCopyResponse](docs/AssignmentCopyResponse.md)
+ - [AssignmentCopyResponseCapabilities](docs/AssignmentCopyResponseCapabilities.md)
+ - [AssignmentCopyResponseCapabilitiesCanPublishInClassError](docs/AssignmentCopyResponseCapabilitiesCanPublishInClassError.md)
  - [AssignmentSubmission](docs/AssignmentSubmission.md)
  - [AssignmentSubmissionComment](docs/AssignmentSubmissionComment.md)
  - [AssignmentSubmissionCommentCreation](docs/AssignmentSubmissionCommentCreation.md)
  - [AssignmentSubmissionHistory](docs/AssignmentSubmissionHistory.md)
  - [AssignmentSubmissionHistoryAttachment](docs/AssignmentSubmissionHistoryAttachment.md)
+ - [AssignmentSubmissionHistoryState](docs/AssignmentSubmissionHistoryState.md)
  - [AssignmentSubmissionState](docs/AssignmentSubmissionState.md)
  - [AssignmentSubmissionUpdate](docs/AssignmentSubmissionUpdate.md)
  - [AssignmentSubmissionUpdateComments](docs/AssignmentSubmissionUpdateComments.md)
  - [AssignmentType](docs/AssignmentType.md)
+ - [AssignmentUpdate](docs/AssignmentUpdate.md)
+ - [ClassAssignment](docs/ClassAssignment.md)
+ - [ClassAssignmentCanvas](docs/ClassAssignmentCanvas.md)
+ - [ClassAssignmentLti](docs/ClassAssignmentLti.md)
+ - [ClassAssignmentMfc](docs/ClassAssignmentMfc.md)
+ - [ClassAssignmentUpdate](docs/ClassAssignmentUpdate.md)
+ - [ClassAssignmentUpdateGoogleClassroom](docs/ClassAssignmentUpdateGoogleClassroom.md)
+ - [ClassAssignmentUpdateMicrosoftGraph](docs/ClassAssignmentUpdateMicrosoftGraph.md)
  - [ClassAttachmentCreation](docs/ClassAttachmentCreation.md)
  - [ClassCreation](docs/ClassCreation.md)
  - [ClassDetails](docs/ClassDetails.md)
  - [ClassDetailsCanvas](docs/ClassDetailsCanvas.md)
  - [ClassDetailsClever](docs/ClassDetailsClever.md)
  - [ClassDetailsGoogleClassroom](docs/ClassDetailsGoogleClassroom.md)
  - [ClassDetailsGoogleDrive](docs/ClassDetailsGoogleDrive.md)
  - [ClassDetailsIssues](docs/ClassDetailsIssues.md)
- - [ClassDetailsIssuesSync](docs/ClassDetailsIssuesSync.md)
+ - [ClassDetailsIssuesSyncInner](docs/ClassDetailsIssuesSyncInner.md)
  - [ClassDetailsLti](docs/ClassDetailsLti.md)
  - [ClassDetailsMfc](docs/ClassDetailsMfc.md)
  - [ClassDetailsMicrosoftGraph](docs/ClassDetailsMicrosoftGraph.md)
+ - [ClassGradeLevel](docs/ClassGradeLevel.md)
  - [ClassRoles](docs/ClassRoles.md)
  - [ClassState](docs/ClassState.md)
  - [ClassUpdate](docs/ClassUpdate.md)
  - [Collection](docs/Collection.md)
  - [CollectionApp](docs/CollectionApp.md)
  - [CollectionCapabilities](docs/CollectionCapabilities.md)
  - [CollectionCreation](docs/CollectionCreation.md)
  - [CollectionModification](docs/CollectionModification.md)
  - [CollectionPrivacy](docs/CollectionPrivacy.md)
  - [CollectionType](docs/CollectionType.md)
+ - [EduLibrary](docs/EduLibrary.md)
+ - [EduResource](docs/EduResource.md)
+ - [EduResourceCapabilities](docs/EduResourceCapabilities.md)
+ - [EduResourceCopy](docs/EduResourceCopy.md)
+ - [EduResourceCreation](docs/EduResourceCreation.md)
+ - [EduResourceMove](docs/EduResourceMove.md)
+ - [EduResourcePrivacy](docs/EduResourcePrivacy.md)
+ - [EduResourceResource](docs/EduResourceResource.md)
+ - [EduResourceType](docs/EduResourceType.md)
+ - [EduResourceUpdate](docs/EduResourceUpdate.md)
+ - [EduResourceUseInClass](docs/EduResourceUseInClass.md)
+ - [EduSkillsFocused](docs/EduSkillsFocused.md)
  - [FlatErrorResponse](docs/FlatErrorResponse.md)
  - [FlatLocales](docs/FlatLocales.md)
  - [GoogleClassroomCoursework](docs/GoogleClassroomCoursework.md)
  - [GoogleClassroomSubmission](docs/GoogleClassroomSubmission.md)
  - [Group](docs/Group.md)
  - [GroupDetails](docs/GroupDetails.md)
  - [GroupType](docs/GroupType.md)
@@ -259,30 +288,28 @@
  - [MediaScoreSharingMode](docs/MediaScoreSharingMode.md)
  - [MicrosoftGraphAssignment](docs/MicrosoftGraphAssignment.md)
  - [MicrosoftGraphSubmission](docs/MicrosoftGraphSubmission.md)
  - [OrganizationInvitation](docs/OrganizationInvitation.md)
  - [OrganizationInvitationCreation](docs/OrganizationInvitationCreation.md)
  - [OrganizationRoles](docs/OrganizationRoles.md)
  - [OrganizationUserAccessTokenCreation](docs/OrganizationUserAccessTokenCreation.md)
- - [OrganizationUserSigninLink](docs/OrganizationUserSigninLink.md)
- - [OrganizationUserSigninLinkCreation](docs/OrganizationUserSigninLinkCreation.md)
  - [ResourceCollaborator](docs/ResourceCollaborator.md)
  - [ResourceCollaboratorCreation](docs/ResourceCollaboratorCreation.md)
  - [ResourceRights](docs/ResourceRights.md)
  - [ScoreComment](docs/ScoreComment.md)
  - [ScoreCommentContext](docs/ScoreCommentContext.md)
  - [ScoreCommentCreation](docs/ScoreCommentCreation.md)
  - [ScoreCommentModeration](docs/ScoreCommentModeration.md)
  - [ScoreCommentUpdate](docs/ScoreCommentUpdate.md)
  - [ScoreCommentsCounts](docs/ScoreCommentsCounts.md)
  - [ScoreCreation](docs/ScoreCreation.md)
  - [ScoreCreationBuilderData](docs/ScoreCreationBuilderData.md)
  - [ScoreCreationBuilderDataLayoutData](docs/ScoreCreationBuilderDataLayoutData.md)
  - [ScoreCreationBuilderDataScoreData](docs/ScoreCreationBuilderDataScoreData.md)
- - [ScoreCreationBuilderDataScoreDataInstruments](docs/ScoreCreationBuilderDataScoreDataInstruments.md)
+ - [ScoreCreationBuilderDataScoreDataInstrumentsInner](docs/ScoreCreationBuilderDataScoreDataInstrumentsInner.md)
  - [ScoreCreationType](docs/ScoreCreationType.md)
  - [ScoreDetails](docs/ScoreDetails.md)
  - [ScoreFork](docs/ScoreFork.md)
  - [ScoreLicense](docs/ScoreLicense.md)
  - [ScoreLikesCounts](docs/ScoreLikesCounts.md)
  - [ScoreModification](docs/ScoreModification.md)
  - [ScorePlaysCounts](docs/ScorePlaysCounts.md)
@@ -297,21 +324,26 @@
  - [ScoreTrackState](docs/ScoreTrackState.md)
  - [ScoreTrackType](docs/ScoreTrackType.md)
  - [ScoreTrackUpdate](docs/ScoreTrackUpdate.md)
  - [ScoreViewsCounts](docs/ScoreViewsCounts.md)
  - [Task](docs/Task.md)
  - [TaskExportOptions](docs/TaskExportOptions.md)
  - [TaskProgress](docs/TaskProgress.md)
+ - [TaskResult](docs/TaskResult.md)
  - [UserAdminUpdate](docs/UserAdminUpdate.md)
+ - [UserAzureDetails](docs/UserAzureDetails.md)
+ - [UserCommunityProfileLinks](docs/UserCommunityProfileLinks.md)
  - [UserCreation](docs/UserCreation.md)
  - [UserDetails](docs/UserDetails.md)
  - [UserDetailsAdmin](docs/UserDetailsAdmin.md)
  - [UserDetailsAdminLicense](docs/UserDetailsAdminLicense.md)
  - [UserPublic](docs/UserPublic.md)
  - [UserPublicSummary](docs/UserPublicSummary.md)
+ - [UserSigninLink](docs/UserSigninLink.md)
+ - [UserSigninLinkCreation](docs/UserSigninLinkCreation.md)
 
 
 ## Documentation For Authorization
 
 
 ## OAuth2
 
@@ -324,14 +356,16 @@
  - **account.education_profile**: Provides access to the basic person's education profile and public organization information. 
  - **scores.readonly**: Allows read-only access to all a user's scores. You won't need this scope to read public scores. 
  - **scores.social**: Allow to post comments and like scores 
  - **scores**: Full, permissive scope to access all of a user's scores. 
  - **collections.readonly**: Allow read-only access to a user's collections.
  - **collections.add_scores**: Allow to add scores to a user's collections.
  - **collections**: Full, permissive scope to access all of a user's collections.
+ - **edu.resources**: Read-write access to the resource library.
+ - **edu.resources.readonly**: Read-only access to the resource library.
  - **edu.classes**: Full, permissive scope to manage the classes.
  - **edu.classes.readonly**: Read-only access to the classes.
  - **edu.assignments**: Read-write access to the assignments and submissions.
  - **edu.assignments.readonly**: Read-only access to the assignments and submissions.
  - **edu.admin**: Full, permissive scope to manage all the admin of an organization.
  - **edu.admin.lti**: Access and manage the LTI Credentials for an organization.
  - **edu.admin.lti.readonly**: Read-only access to the LTI Credentials of an organization.
@@ -341,9 +375,26 @@
 
 
 ## Author
 
 developers@flat.io
 
 
+## Notes for Large OpenAPI documents
+If the OpenAPI document is large, imports in flat_api.apis and flat_api.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+- `from flat_api.api.default_api import DefaultApi`
+- `from flat_api.model.pet import Pet`
 
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+```
+import sys
+sys.setrecursionlimit(1500)
+import flat_api
+from flat_api.apis import *
+from flat_api.models import *
+```
```

### Comparing `flat_api-0.8.1/flat_api.egg-info/SOURCES.txt` & `flat_api-1.0.0/flat_api.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,181 +1,228 @@
 LICENSE
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 flat_api/__init__.py
 flat_api/api_client.py
 flat_api/configuration.py
 flat_api/exceptions.py
+flat_api/model_utils.py
 flat_api/rest.py
 flat_api.egg-info/PKG-INFO
 flat_api.egg-info/SOURCES.txt
 flat_api.egg-info/dependency_links.txt
 flat_api.egg-info/requires.txt
 flat_api.egg-info/top_level.txt
 flat_api/api/__init__.py
 flat_api/api/account_api.py
 flat_api/api/class_api.py
 flat_api/api/collection_api.py
+flat_api/api/edu_resources_api.py
 flat_api/api/group_api.py
 flat_api/api/organization_api.py
 flat_api/api/score_api.py
 flat_api/api/task_api.py
 flat_api/api/user_api.py
+flat_api/apis/__init__.py
+flat_api/model/__init__.py
+flat_api/model/api_access_token.py
+flat_api/model/app_scopes.py
+flat_api/model/assignment.py
+flat_api/model/assignment_copy.py
+flat_api/model/assignment_copy_response.py
+flat_api/model/assignment_copy_response_capabilities.py
+flat_api/model/assignment_copy_response_capabilities_can_publish_in_class_error.py
+flat_api/model/assignment_submission.py
+flat_api/model/assignment_submission_comment.py
+flat_api/model/assignment_submission_comment_creation.py
+flat_api/model/assignment_submission_history.py
+flat_api/model/assignment_submission_history_attachment.py
+flat_api/model/assignment_submission_history_state.py
+flat_api/model/assignment_submission_state.py
+flat_api/model/assignment_submission_update.py
+flat_api/model/assignment_submission_update_comments.py
+flat_api/model/assignment_type.py
+flat_api/model/assignment_update.py
+flat_api/model/class_assignment.py
+flat_api/model/class_assignment_canvas.py
+flat_api/model/class_assignment_lti.py
+flat_api/model/class_assignment_mfc.py
+flat_api/model/class_assignment_update.py
+flat_api/model/class_assignment_update_google_classroom.py
+flat_api/model/class_assignment_update_microsoft_graph.py
+flat_api/model/class_attachment_creation.py
+flat_api/model/class_creation.py
+flat_api/model/class_details.py
+flat_api/model/class_details_canvas.py
+flat_api/model/class_details_clever.py
+flat_api/model/class_details_google_classroom.py
+flat_api/model/class_details_google_drive.py
+flat_api/model/class_details_issues.py
+flat_api/model/class_details_issues_sync_inner.py
+flat_api/model/class_details_lti.py
+flat_api/model/class_details_mfc.py
+flat_api/model/class_details_microsoft_graph.py
+flat_api/model/class_grade_level.py
+flat_api/model/class_roles.py
+flat_api/model/class_state.py
+flat_api/model/class_update.py
+flat_api/model/collection.py
+flat_api/model/collection_app.py
+flat_api/model/collection_capabilities.py
+flat_api/model/collection_creation.py
+flat_api/model/collection_modification.py
+flat_api/model/collection_privacy.py
+flat_api/model/collection_type.py
+flat_api/model/edu_library.py
+flat_api/model/edu_resource.py
+flat_api/model/edu_resource_capabilities.py
+flat_api/model/edu_resource_copy.py
+flat_api/model/edu_resource_creation.py
+flat_api/model/edu_resource_move.py
+flat_api/model/edu_resource_privacy.py
+flat_api/model/edu_resource_resource.py
+flat_api/model/edu_resource_type.py
+flat_api/model/edu_resource_update.py
+flat_api/model/edu_resource_use_in_class.py
+flat_api/model/edu_skills_focused.py
+flat_api/model/flat_error_response.py
+flat_api/model/flat_locales.py
+flat_api/model/google_classroom_coursework.py
+flat_api/model/google_classroom_submission.py
+flat_api/model/group.py
+flat_api/model/group_details.py
+flat_api/model/group_type.py
+flat_api/model/license_mode.py
+flat_api/model/license_sources.py
+flat_api/model/lms_name.py
+flat_api/model/lti_credentials.py
+flat_api/model/lti_credentials_creation.py
+flat_api/model/media_attachment.py
+flat_api/model/media_score_sharing_mode.py
+flat_api/model/microsoft_graph_assignment.py
+flat_api/model/microsoft_graph_submission.py
+flat_api/model/organization_invitation.py
+flat_api/model/organization_invitation_creation.py
+flat_api/model/organization_roles.py
+flat_api/model/organization_user_access_token_creation.py
+flat_api/model/resource_collaborator.py
+flat_api/model/resource_collaborator_creation.py
+flat_api/model/resource_rights.py
+flat_api/model/score_comment.py
+flat_api/model/score_comment_context.py
+flat_api/model/score_comment_creation.py
+flat_api/model/score_comment_moderation.py
+flat_api/model/score_comment_update.py
+flat_api/model/score_comments_counts.py
+flat_api/model/score_creation.py
+flat_api/model/score_creation_builder_data.py
+flat_api/model/score_creation_builder_data_layout_data.py
+flat_api/model/score_creation_builder_data_score_data.py
+flat_api/model/score_creation_builder_data_score_data_instruments_inner.py
+flat_api/model/score_creation_type.py
+flat_api/model/score_details.py
+flat_api/model/score_fork.py
+flat_api/model/score_license.py
+flat_api/model/score_likes_counts.py
+flat_api/model/score_modification.py
+flat_api/model/score_plays_counts.py
+flat_api/model/score_privacy.py
+flat_api/model/score_revision.py
+flat_api/model/score_revision_creation.py
+flat_api/model/score_revision_statistics.py
+flat_api/model/score_source.py
+flat_api/model/score_track.py
+flat_api/model/score_track_creation.py
+flat_api/model/score_track_point.py
+flat_api/model/score_track_state.py
+flat_api/model/score_track_type.py
+flat_api/model/score_track_update.py
+flat_api/model/score_views_counts.py
+flat_api/model/task.py
+flat_api/model/task_export_options.py
+flat_api/model/task_progress.py
+flat_api/model/task_result.py
+flat_api/model/user_admin_update.py
+flat_api/model/user_azure_details.py
+flat_api/model/user_community_profile_links.py
+flat_api/model/user_creation.py
+flat_api/model/user_details.py
+flat_api/model/user_details_admin.py
+flat_api/model/user_details_admin_license.py
+flat_api/model/user_public.py
+flat_api/model/user_public_summary.py
+flat_api/model/user_signin_link.py
+flat_api/model/user_signin_link_creation.py
 flat_api/models/__init__.py
-flat_api/models/api_access_token.py
-flat_api/models/app_scopes.py
-flat_api/models/assignment.py
-flat_api/models/assignment_canvas.py
-flat_api/models/assignment_copy.py
-flat_api/models/assignment_creation.py
-flat_api/models/assignment_creation_google_classroom.py
-flat_api/models/assignment_creation_microsoft_graph.py
-flat_api/models/assignment_lti.py
-flat_api/models/assignment_mfc.py
-flat_api/models/assignment_submission.py
-flat_api/models/assignment_submission_comment.py
-flat_api/models/assignment_submission_comment_creation.py
-flat_api/models/assignment_submission_history.py
-flat_api/models/assignment_submission_history_attachment.py
-flat_api/models/assignment_submission_state.py
-flat_api/models/assignment_submission_update.py
-flat_api/models/assignment_submission_update_comments.py
-flat_api/models/assignment_type.py
-flat_api/models/class_attachment_creation.py
-flat_api/models/class_creation.py
-flat_api/models/class_details.py
-flat_api/models/class_details_canvas.py
-flat_api/models/class_details_clever.py
-flat_api/models/class_details_google_classroom.py
-flat_api/models/class_details_google_drive.py
-flat_api/models/class_details_issues.py
-flat_api/models/class_details_issues_sync.py
-flat_api/models/class_details_lti.py
-flat_api/models/class_details_mfc.py
-flat_api/models/class_details_microsoft_graph.py
-flat_api/models/class_roles.py
-flat_api/models/class_state.py
-flat_api/models/class_update.py
-flat_api/models/collection.py
-flat_api/models/collection_app.py
-flat_api/models/collection_capabilities.py
-flat_api/models/collection_creation.py
-flat_api/models/collection_modification.py
-flat_api/models/collection_privacy.py
-flat_api/models/collection_type.py
-flat_api/models/flat_error_response.py
-flat_api/models/flat_locales.py
-flat_api/models/google_classroom_coursework.py
-flat_api/models/google_classroom_submission.py
-flat_api/models/group.py
-flat_api/models/group_details.py
-flat_api/models/group_type.py
-flat_api/models/license_mode.py
-flat_api/models/license_sources.py
-flat_api/models/lms_name.py
-flat_api/models/lti_credentials.py
-flat_api/models/lti_credentials_creation.py
-flat_api/models/media_attachment.py
-flat_api/models/media_score_sharing_mode.py
-flat_api/models/microsoft_graph_assignment.py
-flat_api/models/microsoft_graph_submission.py
-flat_api/models/organization_invitation.py
-flat_api/models/organization_invitation_creation.py
-flat_api/models/organization_roles.py
-flat_api/models/organization_user_access_token_creation.py
-flat_api/models/organization_user_signin_link.py
-flat_api/models/organization_user_signin_link_creation.py
-flat_api/models/resource_collaborator.py
-flat_api/models/resource_collaborator_creation.py
-flat_api/models/resource_rights.py
-flat_api/models/score_comment.py
-flat_api/models/score_comment_context.py
-flat_api/models/score_comment_creation.py
-flat_api/models/score_comment_moderation.py
-flat_api/models/score_comment_update.py
-flat_api/models/score_comments_counts.py
-flat_api/models/score_creation.py
-flat_api/models/score_creation_builder_data.py
-flat_api/models/score_creation_builder_data_layout_data.py
-flat_api/models/score_creation_builder_data_score_data.py
-flat_api/models/score_creation_builder_data_score_data_instruments.py
-flat_api/models/score_creation_type.py
-flat_api/models/score_details.py
-flat_api/models/score_fork.py
-flat_api/models/score_license.py
-flat_api/models/score_likes_counts.py
-flat_api/models/score_modification.py
-flat_api/models/score_plays_counts.py
-flat_api/models/score_privacy.py
-flat_api/models/score_revision.py
-flat_api/models/score_revision_creation.py
-flat_api/models/score_revision_statistics.py
-flat_api/models/score_source.py
-flat_api/models/score_track.py
-flat_api/models/score_track_creation.py
-flat_api/models/score_track_point.py
-flat_api/models/score_track_state.py
-flat_api/models/score_track_type.py
-flat_api/models/score_track_update.py
-flat_api/models/score_views_counts.py
-flat_api/models/task.py
-flat_api/models/task_export_options.py
-flat_api/models/task_progress.py
-flat_api/models/user_admin_update.py
-flat_api/models/user_creation.py
-flat_api/models/user_details.py
-flat_api/models/user_details_admin.py
-flat_api/models/user_details_admin_license.py
-flat_api/models/user_public.py
-flat_api/models/user_public_summary.py
-test/__init__.py
 test/test_account_api.py
 test/test_api_access_token.py
 test/test_app_scopes.py
 test/test_assignment.py
-test/test_assignment_canvas.py
 test/test_assignment_copy.py
-test/test_assignment_creation.py
-test/test_assignment_creation_google_classroom.py
-test/test_assignment_creation_microsoft_graph.py
-test/test_assignment_lti.py
-test/test_assignment_mfc.py
+test/test_assignment_copy_response.py
+test/test_assignment_copy_response_capabilities.py
+test/test_assignment_copy_response_capabilities_can_publish_in_class_error.py
 test/test_assignment_submission.py
 test/test_assignment_submission_comment.py
 test/test_assignment_submission_comment_creation.py
 test/test_assignment_submission_history.py
 test/test_assignment_submission_history_attachment.py
+test/test_assignment_submission_history_state.py
 test/test_assignment_submission_state.py
 test/test_assignment_submission_update.py
 test/test_assignment_submission_update_comments.py
 test/test_assignment_type.py
+test/test_assignment_update.py
 test/test_class_api.py
+test/test_class_assignment.py
+test/test_class_assignment_canvas.py
+test/test_class_assignment_lti.py
+test/test_class_assignment_mfc.py
+test/test_class_assignment_update.py
+test/test_class_assignment_update_google_classroom.py
+test/test_class_assignment_update_microsoft_graph.py
 test/test_class_attachment_creation.py
 test/test_class_creation.py
 test/test_class_details.py
 test/test_class_details_canvas.py
 test/test_class_details_clever.py
 test/test_class_details_google_classroom.py
 test/test_class_details_google_drive.py
 test/test_class_details_issues.py
-test/test_class_details_issues_sync.py
+test/test_class_details_issues_sync_inner.py
 test/test_class_details_lti.py
 test/test_class_details_mfc.py
 test/test_class_details_microsoft_graph.py
+test/test_class_grade_level.py
 test/test_class_roles.py
 test/test_class_state.py
 test/test_class_update.py
 test/test_collection.py
 test/test_collection_api.py
 test/test_collection_app.py
 test/test_collection_capabilities.py
 test/test_collection_creation.py
 test/test_collection_modification.py
 test/test_collection_privacy.py
 test/test_collection_type.py
+test/test_edu_library.py
+test/test_edu_resource.py
+test/test_edu_resource_capabilities.py
+test/test_edu_resource_copy.py
+test/test_edu_resource_creation.py
+test/test_edu_resource_move.py
+test/test_edu_resource_privacy.py
+test/test_edu_resource_resource.py
+test/test_edu_resource_type.py
+test/test_edu_resource_update.py
+test/test_edu_resource_use_in_class.py
+test/test_edu_resources_api.py
+test/test_edu_skills_focused.py
 test/test_flat_error_response.py
 test/test_flat_locales.py
 test/test_google_classroom_coursework.py
 test/test_google_classroom_submission.py
 test/test_group.py
 test/test_group_api.py
 test/test_group_details.py
@@ -190,31 +237,29 @@
 test/test_microsoft_graph_assignment.py
 test/test_microsoft_graph_submission.py
 test/test_organization_api.py
 test/test_organization_invitation.py
 test/test_organization_invitation_creation.py
 test/test_organization_roles.py
 test/test_organization_user_access_token_creation.py
-test/test_organization_user_signin_link.py
-test/test_organization_user_signin_link_creation.py
 test/test_resource_collaborator.py
 test/test_resource_collaborator_creation.py
 test/test_resource_rights.py
 test/test_score_api.py
 test/test_score_comment.py
 test/test_score_comment_context.py
 test/test_score_comment_creation.py
 test/test_score_comment_moderation.py
 test/test_score_comment_update.py
 test/test_score_comments_counts.py
 test/test_score_creation.py
 test/test_score_creation_builder_data.py
 test/test_score_creation_builder_data_layout_data.py
 test/test_score_creation_builder_data_score_data.py
-test/test_score_creation_builder_data_score_data_instruments.py
+test/test_score_creation_builder_data_score_data_instruments_inner.py
 test/test_score_creation_type.py
 test/test_score_details.py
 test/test_score_fork.py
 test/test_score_license.py
 test/test_score_likes_counts.py
 test/test_score_modification.py
 test/test_score_plays_counts.py
@@ -230,15 +275,20 @@
 test/test_score_track_type.py
 test/test_score_track_update.py
 test/test_score_views_counts.py
 test/test_task.py
 test/test_task_api.py
 test/test_task_export_options.py
 test/test_task_progress.py
+test/test_task_result.py
 test/test_user_admin_update.py
 test/test_user_api.py
+test/test_user_azure_details.py
+test/test_user_community_profile_links.py
 test/test_user_creation.py
 test/test_user_details.py
 test/test_user_details_admin.py
 test/test_user_details_admin_license.py
 test/test_user_public.py
-test/test_user_public_summary.py
+test/test_user_public_summary.py
+test/test_user_signin_link.py
+test/test_user_signin_link_creation.py
```

### Comparing `flat_api-0.8.1/setup.py` & `flat_api-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "flat_api"
-VERSION = "0.8.1"
+VERSION = "1.0.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -37,15 +37,15 @@
     author="The Flat Team (https://flat.io)",
     author_email="developers@flat.io",
     url="https://github.com/FlatIO/api-client-python",
     keywords=["Flat API", "MusicXML", "Music Notation", "MIDI"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["*test.*", "*test"]),
     include_package_data=True,
     license="Apache",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `flat_api-0.8.1/test/test_account_api.py` & `flat_api-1.0.0/test/test_account_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.account_api import AccountApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestAccountApi(unittest.TestCase):
     """AccountApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.account_api.AccountApi()  # noqa: E501
+        self.api = AccountApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_authenticated_user(self):
         """Test case for get_authenticated_user
 
-        Get current user profile  # noqa: E501
+        Get current user account  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_api_access_token.py` & `flat_api-1.0.0/test/test_api_access_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.api_access_token import ApiAccessToken  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.app_scopes import AppScopes
+globals()['AppScopes'] = AppScopes
+from flat_api.model.api_access_token import ApiAccessToken
 
 
 class TestApiAccessToken(unittest.TestCase):
     """ApiAccessToken unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testApiAccessToken(self):
         """Test ApiAccessToken"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.api_access_token.ApiAccessToken()  # noqa: E501
+        # model = ApiAccessToken()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_app_scopes.py` & `flat_api-1.0.0/test/test_app_scopes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.app_scopes import AppScopes  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.app_scopes import AppScopes
 
 
 class TestAppScopes(unittest.TestCase):
     """AppScopes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testAppScopes(self):
         """Test AppScopes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.app_scopes.AppScopes()  # noqa: E501
+        # model = AppScopes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment.py` & `flat_api-1.0.0/test/test_assignment_copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment import Assignment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_copy import AssignmentCopy
 
 
-class TestAssignment(unittest.TestCase):
-    """Assignment unit test stubs"""
+class TestAssignmentCopy(unittest.TestCase):
+    """AssignmentCopy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignment(self):
-        """Test Assignment"""
+    def testAssignmentCopy(self):
+        """Test AssignmentCopy"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment.Assignment()  # noqa: E501
+        # model = AssignmentCopy()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_canvas.py` & `flat_api-1.0.0/test/test_assignment_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_canvas import AssignmentCanvas  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_type import AssignmentType
 
 
-class TestAssignmentCanvas(unittest.TestCase):
-    """AssignmentCanvas unit test stubs"""
+class TestAssignmentType(unittest.TestCase):
+    """AssignmentType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentCanvas(self):
-        """Test AssignmentCanvas"""
+    def testAssignmentType(self):
+        """Test AssignmentType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_canvas.AssignmentCanvas()  # noqa: E501
+        # model = AssignmentType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_copy.py` & `flat_api-1.0.0/test/test_edu_resource_privacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_copy import AssignmentCopy  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_privacy import EduResourcePrivacy
 
 
-class TestAssignmentCopy(unittest.TestCase):
-    """AssignmentCopy unit test stubs"""
+class TestEduResourcePrivacy(unittest.TestCase):
+    """EduResourcePrivacy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentCopy(self):
-        """Test AssignmentCopy"""
+    def testEduResourcePrivacy(self):
+        """Test EduResourcePrivacy"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_copy.AssignmentCopy()  # noqa: E501
+        # model = EduResourcePrivacy()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_creation.py` & `flat_api-1.0.0/test/test_class_assignment_lti.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_creation import AssignmentCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_assignment_lti import ClassAssignmentLti
 
 
-class TestAssignmentCreation(unittest.TestCase):
-    """AssignmentCreation unit test stubs"""
+class TestClassAssignmentLti(unittest.TestCase):
+    """ClassAssignmentLti unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentCreation(self):
-        """Test AssignmentCreation"""
+    def testClassAssignmentLti(self):
+        """Test ClassAssignmentLti"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_creation.AssignmentCreation()  # noqa: E501
+        # model = ClassAssignmentLti()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_creation_google_classroom.py` & `flat_api-1.0.0/test/test_google_classroom_coursework.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_creation_google_classroom import AssignmentCreationGoogleClassroom  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.google_classroom_coursework import GoogleClassroomCoursework
 
 
-class TestAssignmentCreationGoogleClassroom(unittest.TestCase):
-    """AssignmentCreationGoogleClassroom unit test stubs"""
+class TestGoogleClassroomCoursework(unittest.TestCase):
+    """GoogleClassroomCoursework unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentCreationGoogleClassroom(self):
-        """Test AssignmentCreationGoogleClassroom"""
+    def testGoogleClassroomCoursework(self):
+        """Test GoogleClassroomCoursework"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_creation_google_classroom.AssignmentCreationGoogleClassroom()  # noqa: E501
+        # model = GoogleClassroomCoursework()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_creation_microsoft_graph.py` & `flat_api-1.0.0/test/test_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_creation_microsoft_graph import AssignmentCreationMicrosoftGraph  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.group import Group
 
 
-class TestAssignmentCreationMicrosoftGraph(unittest.TestCase):
-    """AssignmentCreationMicrosoftGraph unit test stubs"""
+class TestGroup(unittest.TestCase):
+    """Group unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentCreationMicrosoftGraph(self):
-        """Test AssignmentCreationMicrosoftGraph"""
+    def testGroup(self):
+        """Test Group"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_creation_microsoft_graph.AssignmentCreationMicrosoftGraph()  # noqa: E501
+        # model = Group()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_lti.py` & `flat_api-1.0.0/test/test_lms_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_lti import AssignmentLti  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.lms_name import LmsName
 
 
-class TestAssignmentLti(unittest.TestCase):
-    """AssignmentLti unit test stubs"""
+class TestLmsName(unittest.TestCase):
+    """LmsName unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentLti(self):
-        """Test AssignmentLti"""
+    def testLmsName(self):
+        """Test LmsName"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_lti.AssignmentLti()  # noqa: E501
+        # model = LmsName()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_mfc.py` & `flat_api-1.0.0/test/test_class_assignment_mfc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_mfc import AssignmentMfc  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_assignment_mfc import ClassAssignmentMfc
 
 
-class TestAssignmentMfc(unittest.TestCase):
-    """AssignmentMfc unit test stubs"""
+class TestClassAssignmentMfc(unittest.TestCase):
+    """ClassAssignmentMfc unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentMfc(self):
-        """Test AssignmentMfc"""
+    def testClassAssignmentMfc(self):
+        """Test ClassAssignmentMfc"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_mfc.AssignmentMfc()  # noqa: E501
+        # model = ClassAssignmentMfc()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission.py` & `flat_api-1.0.0/test/test_assignment_submission_comment_creation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission import AssignmentSubmission  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_comment_creation import AssignmentSubmissionCommentCreation
 
 
-class TestAssignmentSubmission(unittest.TestCase):
-    """AssignmentSubmission unit test stubs"""
+class TestAssignmentSubmissionCommentCreation(unittest.TestCase):
+    """AssignmentSubmissionCommentCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmission(self):
-        """Test AssignmentSubmission"""
+    def testAssignmentSubmissionCommentCreation(self):
+        """Test AssignmentSubmissionCommentCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission.AssignmentSubmission()  # noqa: E501
+        # model = AssignmentSubmissionCommentCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_comment.py` & `flat_api-1.0.0/test/test_assignment_submission_comment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_comment import AssignmentSubmissionComment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_comment import AssignmentSubmissionComment
 
 
 class TestAssignmentSubmissionComment(unittest.TestCase):
     """AssignmentSubmissionComment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testAssignmentSubmissionComment(self):
         """Test AssignmentSubmissionComment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_comment.AssignmentSubmissionComment()  # noqa: E501
+        # model = AssignmentSubmissionComment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_comment_creation.py` & `flat_api-1.0.0/test/test_assignment_submission_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_comment_creation import AssignmentSubmissionCommentCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_update_comments import AssignmentSubmissionUpdateComments
+from flat_api.model.class_attachment_creation import ClassAttachmentCreation
+globals()['AssignmentSubmissionUpdateComments'] = AssignmentSubmissionUpdateComments
+globals()['ClassAttachmentCreation'] = ClassAttachmentCreation
+from flat_api.model.assignment_submission_update import AssignmentSubmissionUpdate
 
 
-class TestAssignmentSubmissionCommentCreation(unittest.TestCase):
-    """AssignmentSubmissionCommentCreation unit test stubs"""
+class TestAssignmentSubmissionUpdate(unittest.TestCase):
+    """AssignmentSubmissionUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionCommentCreation(self):
-        """Test AssignmentSubmissionCommentCreation"""
+    def testAssignmentSubmissionUpdate(self):
+        """Test AssignmentSubmissionUpdate"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_comment_creation.AssignmentSubmissionCommentCreation()  # noqa: E501
+        # model = AssignmentSubmissionUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_history.py` & `flat_api-1.0.0/test/test_assignment_submission_history_attachment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_history import AssignmentSubmissionHistory  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_history_attachment import AssignmentSubmissionHistoryAttachment
 
 
-class TestAssignmentSubmissionHistory(unittest.TestCase):
-    """AssignmentSubmissionHistory unit test stubs"""
+class TestAssignmentSubmissionHistoryAttachment(unittest.TestCase):
+    """AssignmentSubmissionHistoryAttachment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionHistory(self):
-        """Test AssignmentSubmissionHistory"""
+    def testAssignmentSubmissionHistoryAttachment(self):
+        """Test AssignmentSubmissionHistoryAttachment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_history.AssignmentSubmissionHistory()  # noqa: E501
+        # model = AssignmentSubmissionHistoryAttachment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_history_attachment.py` & `flat_api-1.0.0/test/test_assignment_submission_history.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_history_attachment import AssignmentSubmissionHistoryAttachment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_history_attachment import AssignmentSubmissionHistoryAttachment
+from flat_api.model.assignment_submission_history_state import AssignmentSubmissionHistoryState
+globals()['AssignmentSubmissionHistoryAttachment'] = AssignmentSubmissionHistoryAttachment
+globals()['AssignmentSubmissionHistoryState'] = AssignmentSubmissionHistoryState
+from flat_api.model.assignment_submission_history import AssignmentSubmissionHistory
 
 
-class TestAssignmentSubmissionHistoryAttachment(unittest.TestCase):
-    """AssignmentSubmissionHistoryAttachment unit test stubs"""
+class TestAssignmentSubmissionHistory(unittest.TestCase):
+    """AssignmentSubmissionHistory unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionHistoryAttachment(self):
-        """Test AssignmentSubmissionHistoryAttachment"""
+    def testAssignmentSubmissionHistory(self):
+        """Test AssignmentSubmissionHistory"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_history_attachment.AssignmentSubmissionHistoryAttachment()  # noqa: E501
+        # model = AssignmentSubmissionHistory()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_state.py` & `flat_api-1.0.0/test/test_assignment_submission_history_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_state import AssignmentSubmissionState  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_history_state import AssignmentSubmissionHistoryState
 
 
-class TestAssignmentSubmissionState(unittest.TestCase):
-    """AssignmentSubmissionState unit test stubs"""
+class TestAssignmentSubmissionHistoryState(unittest.TestCase):
+    """AssignmentSubmissionHistoryState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionState(self):
-        """Test AssignmentSubmissionState"""
+    def testAssignmentSubmissionHistoryState(self):
+        """Test AssignmentSubmissionHistoryState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_state.AssignmentSubmissionState()  # noqa: E501
+        # model = AssignmentSubmissionHistoryState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_update.py` & `flat_api-1.0.0/test/test_assignment_submission_update_comments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_update import AssignmentSubmissionUpdate  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_submission_update_comments import AssignmentSubmissionUpdateComments
 
 
-class TestAssignmentSubmissionUpdate(unittest.TestCase):
-    """AssignmentSubmissionUpdate unit test stubs"""
+class TestAssignmentSubmissionUpdateComments(unittest.TestCase):
+    """AssignmentSubmissionUpdateComments unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionUpdate(self):
-        """Test AssignmentSubmissionUpdate"""
+    def testAssignmentSubmissionUpdateComments(self):
+        """Test AssignmentSubmissionUpdateComments"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_update.AssignmentSubmissionUpdate()  # noqa: E501
+        # model = AssignmentSubmissionUpdateComments()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_submission_update_comments.py` & `flat_api-1.0.0/test/test_score_comment_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_submission_update_comments import AssignmentSubmissionUpdateComments  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comment_context import ScoreCommentContext
+globals()['ScoreCommentContext'] = ScoreCommentContext
+from flat_api.model.score_comment_update import ScoreCommentUpdate
 
 
-class TestAssignmentSubmissionUpdateComments(unittest.TestCase):
-    """AssignmentSubmissionUpdateComments unit test stubs"""
+class TestScoreCommentUpdate(unittest.TestCase):
+    """ScoreCommentUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentSubmissionUpdateComments(self):
-        """Test AssignmentSubmissionUpdateComments"""
+    def testScoreCommentUpdate(self):
+        """Test ScoreCommentUpdate"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_submission_update_comments.AssignmentSubmissionUpdateComments()  # noqa: E501
+        # model = ScoreCommentUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_assignment_type.py` & `flat_api-1.0.0/test/test_edu_skills_focused.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.assignment_type import AssignmentType  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_skills_focused import EduSkillsFocused
 
 
-class TestAssignmentType(unittest.TestCase):
-    """AssignmentType unit test stubs"""
+class TestEduSkillsFocused(unittest.TestCase):
+    """EduSkillsFocused unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAssignmentType(self):
-        """Test AssignmentType"""
+    def testEduSkillsFocused(self):
+        """Test EduSkillsFocused"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.assignment_type.AssignmentType()  # noqa: E501
+        # model = EduSkillsFocused()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_api.py` & `flat_api-1.0.0/test/test_class_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.class_api import ClassApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestClassApi(unittest.TestCase):
     """ClassApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.class_api.ClassApi()  # noqa: E501
+        self.api = ClassApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_activate_class(self):
         """Test case for activate_class
 
@@ -60,46 +55,53 @@
     def test_copy_assignment(self):
         """Test case for copy_assignment
 
         Copy an assignment  # noqa: E501
         """
         pass
 
-    def test_create_assignment(self):
-        """Test case for create_assignment
+    def test_create_class(self):
+        """Test case for create_class
 
-        Assignment creation  # noqa: E501
+        Create a new class  # noqa: E501
         """
         pass
 
-    def test_create_class(self):
-        """Test case for create_class
+    def test_create_class_assignment(self):
+        """Test case for create_class_assignment
 
-        Create a new class  # noqa: E501
+        Assignment creation  # noqa: E501
         """
         pass
 
     def test_create_submission(self):
         """Test case for create_submission
 
         Create or edit a submission  # noqa: E501
         """
         pass
 
+    def test_create_test_student_account(self):
+        """Test case for create_test_student_account
+
+        Create a test student account  # noqa: E501
+        """
+        pass
+
     def test_delete_class_user(self):
         """Test case for delete_class_user
 
         Remove a user from the class  # noqa: E501
         """
         pass
 
     def test_delete_submission(self):
         """Test case for delete_submission
 
-        Delete a submission  # noqa: E501
+        Reset a submission  # noqa: E501
         """
         pass
 
     def test_delete_submission_comment(self):
         """Test case for delete_submission_comment
 
         Delete a feedback comment to a submission  # noqa: E501
@@ -130,21 +132,14 @@
     def test_export_submissions_reviews_as_excel(self):
         """Test case for export_submissions_reviews_as_excel
 
         Excel Grades exports  # noqa: E501
         """
         pass
 
-    def test_fork_score(self):
-        """Test case for fork_score
-
-        Fork a score  # noqa: E501
-        """
-        pass
-
     def test_get_class(self):
         """Test case for get_class
 
         Get the details of a single class  # noqa: E501
         """
         pass
```

### Comparing `flat_api-0.8.1/test/test_class_attachment_creation.py` & `flat_api-1.0.0/test/test_class_attachment_creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_attachment_creation import ClassAttachmentCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.media_score_sharing_mode import MediaScoreSharingMode
+globals()['MediaScoreSharingMode'] = MediaScoreSharingMode
+from flat_api.model.class_attachment_creation import ClassAttachmentCreation
 
 
 class TestClassAttachmentCreation(unittest.TestCase):
     """ClassAttachmentCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testClassAttachmentCreation(self):
         """Test ClassAttachmentCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_attachment_creation.ClassAttachmentCreation()  # noqa: E501
+        # model = ClassAttachmentCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_creation.py` & `flat_api-1.0.0/test/test_user_creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_creation import ClassCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.flat_locales import FlatLocales
+globals()['FlatLocales'] = FlatLocales
+from flat_api.model.user_creation import UserCreation
 
 
-class TestClassCreation(unittest.TestCase):
-    """ClassCreation unit test stubs"""
+class TestUserCreation(unittest.TestCase):
+    """UserCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassCreation(self):
-        """Test ClassCreation"""
+    def testUserCreation(self):
+        """Test UserCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_creation.ClassCreation()  # noqa: E501
+        # model = UserCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details.py` & `flat_api-1.0.0/test/test_class_details_mfc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details import ClassDetails  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_mfc import ClassDetailsMfc
 
 
-class TestClassDetails(unittest.TestCase):
-    """ClassDetails unit test stubs"""
+class TestClassDetailsMfc(unittest.TestCase):
+    """ClassDetailsMfc unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetails(self):
-        """Test ClassDetails"""
+    def testClassDetailsMfc(self):
+        """Test ClassDetailsMfc"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details.ClassDetails()  # noqa: E501
+        # model = ClassDetailsMfc()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_canvas.py` & `flat_api-1.0.0/test/test_class_details_lti.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_canvas import ClassDetailsCanvas  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_lti import ClassDetailsLti
 
 
-class TestClassDetailsCanvas(unittest.TestCase):
-    """ClassDetailsCanvas unit test stubs"""
+class TestClassDetailsLti(unittest.TestCase):
+    """ClassDetailsLti unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsCanvas(self):
-        """Test ClassDetailsCanvas"""
+    def testClassDetailsLti(self):
+        """Test ClassDetailsLti"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_canvas.ClassDetailsCanvas()  # noqa: E501
+        # model = ClassDetailsLti()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_clever.py` & `flat_api-1.0.0/test/test_class_details_issues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_clever import ClassDetailsClever  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_issues_sync_inner import ClassDetailsIssuesSyncInner
+globals()['ClassDetailsIssuesSyncInner'] = ClassDetailsIssuesSyncInner
+from flat_api.model.class_details_issues import ClassDetailsIssues
 
 
-class TestClassDetailsClever(unittest.TestCase):
-    """ClassDetailsClever unit test stubs"""
+class TestClassDetailsIssues(unittest.TestCase):
+    """ClassDetailsIssues unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsClever(self):
-        """Test ClassDetailsClever"""
+    def testClassDetailsIssues(self):
+        """Test ClassDetailsIssues"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_clever.ClassDetailsClever()  # noqa: E501
+        # model = ClassDetailsIssues()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_google_classroom.py` & `flat_api-1.0.0/test/test_class_details_google_classroom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_google_classroom import ClassDetailsGoogleClassroom  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_google_classroom import ClassDetailsGoogleClassroom
 
 
 class TestClassDetailsGoogleClassroom(unittest.TestCase):
     """ClassDetailsGoogleClassroom unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testClassDetailsGoogleClassroom(self):
         """Test ClassDetailsGoogleClassroom"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_google_classroom.ClassDetailsGoogleClassroom()  # noqa: E501
+        # model = ClassDetailsGoogleClassroom()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_google_drive.py` & `flat_api-1.0.0/test/test_class_details_google_drive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_google_drive import ClassDetailsGoogleDrive  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_google_drive import ClassDetailsGoogleDrive
 
 
 class TestClassDetailsGoogleDrive(unittest.TestCase):
     """ClassDetailsGoogleDrive unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testClassDetailsGoogleDrive(self):
         """Test ClassDetailsGoogleDrive"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_google_drive.ClassDetailsGoogleDrive()  # noqa: E501
+        # model = ClassDetailsGoogleDrive()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_issues.py` & `flat_api-1.0.0/test/test_class_details_issues_sync_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_issues import ClassDetailsIssues  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_issues_sync_inner import ClassDetailsIssuesSyncInner
 
 
-class TestClassDetailsIssues(unittest.TestCase):
-    """ClassDetailsIssues unit test stubs"""
+class TestClassDetailsIssuesSyncInner(unittest.TestCase):
+    """ClassDetailsIssuesSyncInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsIssues(self):
-        """Test ClassDetailsIssues"""
+    def testClassDetailsIssuesSyncInner(self):
+        """Test ClassDetailsIssuesSyncInner"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_issues.ClassDetailsIssues()  # noqa: E501
+        # model = ClassDetailsIssuesSyncInner()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_issues_sync.py` & `flat_api-1.0.0/test/test_score_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_issues_sync import ClassDetailsIssuesSync  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_source import ScoreSource
 
 
-class TestClassDetailsIssuesSync(unittest.TestCase):
-    """ClassDetailsIssuesSync unit test stubs"""
+class TestScoreSource(unittest.TestCase):
+    """ScoreSource unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsIssuesSync(self):
-        """Test ClassDetailsIssuesSync"""
+    def testScoreSource(self):
+        """Test ScoreSource"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_issues_sync.ClassDetailsIssuesSync()  # noqa: E501
+        # model = ScoreSource()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_lti.py` & `flat_api-1.0.0/test/test_class_assignment_canvas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_lti import ClassDetailsLti  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_assignment_canvas import ClassAssignmentCanvas
 
 
-class TestClassDetailsLti(unittest.TestCase):
-    """ClassDetailsLti unit test stubs"""
+class TestClassAssignmentCanvas(unittest.TestCase):
+    """ClassAssignmentCanvas unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsLti(self):
-        """Test ClassDetailsLti"""
+    def testClassAssignmentCanvas(self):
+        """Test ClassAssignmentCanvas"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_lti.ClassDetailsLti()  # noqa: E501
+        # model = ClassAssignmentCanvas()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_mfc.py` & `flat_api-1.0.0/test/test_class_details_microsoft_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_mfc import ClassDetailsMfc  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_microsoft_graph import ClassDetailsMicrosoftGraph
 
 
-class TestClassDetailsMfc(unittest.TestCase):
-    """ClassDetailsMfc unit test stubs"""
+class TestClassDetailsMicrosoftGraph(unittest.TestCase):
+    """ClassDetailsMicrosoftGraph unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsMfc(self):
-        """Test ClassDetailsMfc"""
+    def testClassDetailsMicrosoftGraph(self):
+        """Test ClassDetailsMicrosoftGraph"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_mfc.ClassDetailsMfc()  # noqa: E501
+        # model = ClassDetailsMicrosoftGraph()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_details_microsoft_graph.py` & `flat_api-1.0.0/test/test_resource_collaborator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_details_microsoft_graph import ClassDetailsMicrosoftGraph  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.group import Group
+from flat_api.model.user_public import UserPublic
+globals()['Group'] = Group
+globals()['UserPublic'] = UserPublic
+from flat_api.model.resource_collaborator import ResourceCollaborator
 
 
-class TestClassDetailsMicrosoftGraph(unittest.TestCase):
-    """ClassDetailsMicrosoftGraph unit test stubs"""
+class TestResourceCollaborator(unittest.TestCase):
+    """ResourceCollaborator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassDetailsMicrosoftGraph(self):
-        """Test ClassDetailsMicrosoftGraph"""
+    def testResourceCollaborator(self):
+        """Test ResourceCollaborator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_details_microsoft_graph.ClassDetailsMicrosoftGraph()  # noqa: E501
+        # model = ResourceCollaborator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_roles.py` & `flat_api-1.0.0/test/test_edu_resource_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_roles import ClassRoles  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_type import EduResourceType
 
 
-class TestClassRoles(unittest.TestCase):
-    """ClassRoles unit test stubs"""
+class TestEduResourceType(unittest.TestCase):
+    """EduResourceType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassRoles(self):
-        """Test ClassRoles"""
+    def testEduResourceType(self):
+        """Test EduResourceType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_roles.ClassRoles()  # noqa: E501
+        # model = EduResourceType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_state.py` & `flat_api-1.0.0/test/test_class_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_state import ClassState  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_state import ClassState
 
 
 class TestClassState(unittest.TestCase):
     """ClassState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testClassState(self):
         """Test ClassState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_state.ClassState()  # noqa: E501
+        # model = ClassState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_class_update.py` & `flat_api-1.0.0/test/test_collection_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.class_update import ClassUpdate  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.collection_type import CollectionType
 
 
-class TestClassUpdate(unittest.TestCase):
-    """ClassUpdate unit test stubs"""
+class TestCollectionType(unittest.TestCase):
+    """CollectionType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testClassUpdate(self):
-        """Test ClassUpdate"""
+    def testCollectionType(self):
+        """Test CollectionType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.class_update.ClassUpdate()  # noqa: E501
+        # model = CollectionType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection.py` & `flat_api-1.0.0/test/test_collection_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection import Collection  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.collection_app import CollectionApp
 
 
-class TestCollection(unittest.TestCase):
-    """Collection unit test stubs"""
+class TestCollectionApp(unittest.TestCase):
+    """CollectionApp unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollection(self):
-        """Test Collection"""
+    def testCollectionApp(self):
+        """Test CollectionApp"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection.Collection()  # noqa: E501
+        # model = CollectionApp()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_api.py` & `flat_api-1.0.0/test/test_collection_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.collection_api import CollectionApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestCollectionApi(unittest.TestCase):
     """CollectionApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.collection_api.CollectionApi()  # noqa: E501
+        self.api = CollectionApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_add_score_to_collection(self):
         """Test case for add_score_to_collection
```

### Comparing `flat_api-0.8.1/test/test_collection_app.py` & `flat_api-1.0.0/test/test_collection_capabilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_app import CollectionApp  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.collection_capabilities import CollectionCapabilities
 
 
-class TestCollectionApp(unittest.TestCase):
-    """CollectionApp unit test stubs"""
+class TestCollectionCapabilities(unittest.TestCase):
+    """CollectionCapabilities unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollectionApp(self):
-        """Test CollectionApp"""
+    def testCollectionCapabilities(self):
+        """Test CollectionCapabilities"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_app.CollectionApp()  # noqa: E501
+        # model = CollectionCapabilities()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_capabilities.py` & `flat_api-1.0.0/test/test_edu_resource_use_in_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_capabilities import CollectionCapabilities  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_use_in_class import EduResourceUseInClass
 
 
-class TestCollectionCapabilities(unittest.TestCase):
-    """CollectionCapabilities unit test stubs"""
+class TestEduResourceUseInClass(unittest.TestCase):
+    """EduResourceUseInClass unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollectionCapabilities(self):
-        """Test CollectionCapabilities"""
+    def testEduResourceUseInClass(self):
+        """Test EduResourceUseInClass"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_capabilities.CollectionCapabilities()  # noqa: E501
+        # model = EduResourceUseInClass()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_creation.py` & `flat_api-1.0.0/test/test_edu_resource_capabilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_creation import CollectionCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_capabilities import EduResourceCapabilities
 
 
-class TestCollectionCreation(unittest.TestCase):
-    """CollectionCreation unit test stubs"""
+class TestEduResourceCapabilities(unittest.TestCase):
+    """EduResourceCapabilities unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollectionCreation(self):
-        """Test CollectionCreation"""
+    def testEduResourceCapabilities(self):
+        """Test EduResourceCapabilities"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_creation.CollectionCreation()  # noqa: E501
+        # model = EduResourceCapabilities()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_modification.py` & `flat_api-1.0.0/test/test_collection_modification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_modification import CollectionModification  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.collection_privacy import CollectionPrivacy
+globals()['CollectionPrivacy'] = CollectionPrivacy
+from flat_api.model.collection_modification import CollectionModification
 
 
 class TestCollectionModification(unittest.TestCase):
     """CollectionModification unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testCollectionModification(self):
         """Test CollectionModification"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_modification.CollectionModification()  # noqa: E501
+        # model = CollectionModification()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_privacy.py` & `flat_api-1.0.0/test/test_score_comment_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_privacy import CollectionPrivacy  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comment_context import ScoreCommentContext
+globals()['ScoreCommentContext'] = ScoreCommentContext
+from flat_api.model.score_comment_creation import ScoreCommentCreation
 
 
-class TestCollectionPrivacy(unittest.TestCase):
-    """CollectionPrivacy unit test stubs"""
+class TestScoreCommentCreation(unittest.TestCase):
+    """ScoreCommentCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollectionPrivacy(self):
-        """Test CollectionPrivacy"""
+    def testScoreCommentCreation(self):
+        """Test ScoreCommentCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_privacy.CollectionPrivacy()  # noqa: E501
+        # model = ScoreCommentCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_collection_type.py` & `flat_api-1.0.0/test/test_score_likes_counts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.collection_type import CollectionType  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_likes_counts import ScoreLikesCounts
 
 
-class TestCollectionType(unittest.TestCase):
-    """CollectionType unit test stubs"""
+class TestScoreLikesCounts(unittest.TestCase):
+    """ScoreLikesCounts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCollectionType(self):
-        """Test CollectionType"""
+    def testScoreLikesCounts(self):
+        """Test ScoreLikesCounts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.collection_type.CollectionType()  # noqa: E501
+        # model = ScoreLikesCounts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_flat_error_response.py` & `flat_api-1.0.0/test/test_flat_error_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.flat_error_response import FlatErrorResponse  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.flat_error_response import FlatErrorResponse
 
 
 class TestFlatErrorResponse(unittest.TestCase):
     """FlatErrorResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testFlatErrorResponse(self):
         """Test FlatErrorResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.flat_error_response.FlatErrorResponse()  # noqa: E501
+        # model = FlatErrorResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_flat_locales.py` & `flat_api-1.0.0/test/test_flat_locales.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.flat_locales import FlatLocales  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.flat_locales import FlatLocales
 
 
 class TestFlatLocales(unittest.TestCase):
     """FlatLocales unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testFlatLocales(self):
         """Test FlatLocales"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.flat_locales.FlatLocales()  # noqa: E501
+        # model = FlatLocales()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_google_classroom_coursework.py` & `flat_api-1.0.0/test/test_user_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
-from flat_api.models.google_classroom_coursework import GoogleClassroomCoursework  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.api.user_api import UserApi  # noqa: E501
 
 
-class TestGoogleClassroomCoursework(unittest.TestCase):
-    """GoogleClassroomCoursework unit test stubs"""
+class TestUserApi(unittest.TestCase):
+    """UserApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = UserApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testGoogleClassroomCoursework(self):
-        """Test GoogleClassroomCoursework"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.google_classroom_coursework.GoogleClassroomCoursework()  # noqa: E501
+    def test_ger_user_likes(self):
+        """Test case for ger_user_likes
+
+        List liked scores  # noqa: E501
+        """
+        pass
+
+    def test_get_user(self):
+        """Test case for get_user
+
+        Get a public user profile  # noqa: E501
+        """
+        pass
+
+    def test_get_user_scores(self):
+        """Test case for get_user_scores
+
+        List user's scores  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_google_classroom_submission.py` & `flat_api-1.0.0/test/test_group_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.google_classroom_submission import GoogleClassroomSubmission  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.group_type import GroupType
 
 
-class TestGoogleClassroomSubmission(unittest.TestCase):
-    """GoogleClassroomSubmission unit test stubs"""
+class TestGroupType(unittest.TestCase):
+    """GroupType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGoogleClassroomSubmission(self):
-        """Test GoogleClassroomSubmission"""
+    def testGroupType(self):
+        """Test GroupType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.google_classroom_submission.GoogleClassroomSubmission()  # noqa: E501
+        # model = GroupType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_group.py` & `flat_api-1.0.0/test/test_license_sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.group import Group  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.license_sources import LicenseSources
 
 
-class TestGroup(unittest.TestCase):
-    """Group unit test stubs"""
+class TestLicenseSources(unittest.TestCase):
+    """LicenseSources unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroup(self):
-        """Test Group"""
+    def testLicenseSources(self):
+        """Test LicenseSources"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.group.Group()  # noqa: E501
+        # model = LicenseSources()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_group_api.py` & `flat_api-1.0.0/test/test_group_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.group_api import GroupApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestGroupApi(unittest.TestCase):
     """GroupApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.group_api.GroupApi()  # noqa: E501
+        self.api = GroupApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_group_details(self):
         """Test case for get_group_details
```

### Comparing `flat_api-0.8.1/test/test_group_details.py` & `flat_api-1.0.0/test/test_group_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.group_details import GroupDetails  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.group_type import GroupType
+globals()['GroupType'] = GroupType
+from flat_api.model.group_details import GroupDetails
 
 
 class TestGroupDetails(unittest.TestCase):
     """GroupDetails unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testGroupDetails(self):
         """Test GroupDetails"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.group_details.GroupDetails()  # noqa: E501
+        # model = GroupDetails()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_group_type.py` & `flat_api-1.0.0/test/test_user_azure_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.group_type import GroupType  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.user_azure_details import UserAzureDetails
 
 
-class TestGroupType(unittest.TestCase):
-    """GroupType unit test stubs"""
+class TestUserAzureDetails(unittest.TestCase):
+    """UserAzureDetails unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGroupType(self):
-        """Test GroupType"""
+    def testUserAzureDetails(self):
+        """Test UserAzureDetails"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.group_type.GroupType()  # noqa: E501
+        # model = UserAzureDetails()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_license_mode.py` & `flat_api-1.0.0/test/test_license_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.license_mode import LicenseMode  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.license_mode import LicenseMode
 
 
 class TestLicenseMode(unittest.TestCase):
     """LicenseMode unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testLicenseMode(self):
         """Test LicenseMode"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.license_mode.LicenseMode()  # noqa: E501
+        # model = LicenseMode()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_license_sources.py` & `flat_api-1.0.0/test/test_score_license.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.license_sources import LicenseSources  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_license import ScoreLicense
 
 
-class TestLicenseSources(unittest.TestCase):
-    """LicenseSources unit test stubs"""
+class TestScoreLicense(unittest.TestCase):
+    """ScoreLicense unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLicenseSources(self):
-        """Test LicenseSources"""
+    def testScoreLicense(self):
+        """Test ScoreLicense"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.license_sources.LicenseSources()  # noqa: E501
+        # model = ScoreLicense()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_lms_name.py` & `flat_api-1.0.0/test/test_task_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.lms_name import LmsName  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.task_result import TaskResult
 
 
-class TestLmsName(unittest.TestCase):
-    """LmsName unit test stubs"""
+class TestTaskResult(unittest.TestCase):
+    """TaskResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLmsName(self):
-        """Test LmsName"""
+    def testTaskResult(self):
+        """Test TaskResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.lms_name.LmsName()  # noqa: E501
+        # model = TaskResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_lti_credentials.py` & `flat_api-1.0.0/test/test_lti_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.lti_credentials import LtiCredentials  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.lms_name import LmsName
+globals()['LmsName'] = LmsName
+from flat_api.model.lti_credentials import LtiCredentials
 
 
 class TestLtiCredentials(unittest.TestCase):
     """LtiCredentials unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testLtiCredentials(self):
         """Test LtiCredentials"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.lti_credentials.LtiCredentials()  # noqa: E501
+        # model = LtiCredentials()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_lti_credentials_creation.py` & `flat_api-1.0.0/test/test_lti_credentials_creation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.lti_credentials_creation import LtiCredentialsCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.lms_name import LmsName
+globals()['LmsName'] = LmsName
+from flat_api.model.lti_credentials_creation import LtiCredentialsCreation
 
 
 class TestLtiCredentialsCreation(unittest.TestCase):
     """LtiCredentialsCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testLtiCredentialsCreation(self):
         """Test LtiCredentialsCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.lti_credentials_creation.LtiCredentialsCreation()  # noqa: E501
+        # model = LtiCredentialsCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_media_attachment.py` & `flat_api-1.0.0/test/test_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.media_attachment import MediaAttachment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.task_progress import TaskProgress
+from flat_api.model.task_result import TaskResult
+globals()['TaskProgress'] = TaskProgress
+globals()['TaskResult'] = TaskResult
+from flat_api.model.task import Task
 
 
-class TestMediaAttachment(unittest.TestCase):
-    """MediaAttachment unit test stubs"""
+class TestTask(unittest.TestCase):
+    """Task unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMediaAttachment(self):
-        """Test MediaAttachment"""
+    def testTask(self):
+        """Test Task"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.media_attachment.MediaAttachment()  # noqa: E501
+        # model = Task()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_media_score_sharing_mode.py` & `flat_api-1.0.0/test/test_score_comment_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.media_score_sharing_mode import MediaScoreSharingMode  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comment_context import ScoreCommentContext
 
 
-class TestMediaScoreSharingMode(unittest.TestCase):
-    """MediaScoreSharingMode unit test stubs"""
+class TestScoreCommentContext(unittest.TestCase):
+    """ScoreCommentContext unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMediaScoreSharingMode(self):
-        """Test MediaScoreSharingMode"""
+    def testScoreCommentContext(self):
+        """Test ScoreCommentContext"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.media_score_sharing_mode.MediaScoreSharingMode()  # noqa: E501
+        # model = ScoreCommentContext()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_microsoft_graph_assignment.py` & `flat_api-1.0.0/test/test_microsoft_graph_assignment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.microsoft_graph_assignment import MicrosoftGraphAssignment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.microsoft_graph_assignment import MicrosoftGraphAssignment
 
 
 class TestMicrosoftGraphAssignment(unittest.TestCase):
     """MicrosoftGraphAssignment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testMicrosoftGraphAssignment(self):
         """Test MicrosoftGraphAssignment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.microsoft_graph_assignment.MicrosoftGraphAssignment()  # noqa: E501
+        # model = MicrosoftGraphAssignment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_microsoft_graph_submission.py` & `flat_api-1.0.0/test/test_microsoft_graph_submission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.microsoft_graph_submission import MicrosoftGraphSubmission  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.microsoft_graph_submission import MicrosoftGraphSubmission
 
 
 class TestMicrosoftGraphSubmission(unittest.TestCase):
     """MicrosoftGraphSubmission unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testMicrosoftGraphSubmission(self):
         """Test MicrosoftGraphSubmission"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.microsoft_graph_submission.MicrosoftGraphSubmission()  # noqa: E501
+        # model = MicrosoftGraphSubmission()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_api.py` & `flat_api-1.0.0/test/test_organization_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.organization_api import OrganizationApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestOrganizationApi(unittest.TestCase):
     """OrganizationApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.organization_api.OrganizationApi()  # noqa: E501
+        self.api = OrganizationApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_count_orga_users(self):
         """Test case for count_orga_users
```

### Comparing `flat_api-0.8.1/test/test_organization_invitation.py` & `flat_api-1.0.0/test/test_organization_invitation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_invitation import OrganizationInvitation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.organization_roles import OrganizationRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+from flat_api.model.organization_invitation import OrganizationInvitation
 
 
 class TestOrganizationInvitation(unittest.TestCase):
     """OrganizationInvitation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testOrganizationInvitation(self):
         """Test OrganizationInvitation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_invitation.OrganizationInvitation()  # noqa: E501
+        # model = OrganizationInvitation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_invitation_creation.py` & `flat_api-1.0.0/test/test_organization_invitation_creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_invitation_creation import OrganizationInvitationCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.organization_roles import OrganizationRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+from flat_api.model.organization_invitation_creation import OrganizationInvitationCreation
 
 
 class TestOrganizationInvitationCreation(unittest.TestCase):
     """OrganizationInvitationCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testOrganizationInvitationCreation(self):
         """Test OrganizationInvitationCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_invitation_creation.OrganizationInvitationCreation()  # noqa: E501
+        # model = OrganizationInvitationCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_roles.py` & `flat_api-1.0.0/test/test_user_admin_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_roles import OrganizationRoles  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.organization_roles import OrganizationRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+from flat_api.model.user_admin_update import UserAdminUpdate
 
 
-class TestOrganizationRoles(unittest.TestCase):
-    """OrganizationRoles unit test stubs"""
+class TestUserAdminUpdate(unittest.TestCase):
+    """UserAdminUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationRoles(self):
-        """Test OrganizationRoles"""
+    def testUserAdminUpdate(self):
+        """Test UserAdminUpdate"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_roles.OrganizationRoles()  # noqa: E501
+        # model = UserAdminUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_user_access_token_creation.py` & `flat_api-1.0.0/test/test_organization_user_access_token_creation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_user_access_token_creation import OrganizationUserAccessTokenCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.app_scopes import AppScopes
+globals()['AppScopes'] = AppScopes
+from flat_api.model.organization_user_access_token_creation import OrganizationUserAccessTokenCreation
 
 
 class TestOrganizationUserAccessTokenCreation(unittest.TestCase):
     """OrganizationUserAccessTokenCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testOrganizationUserAccessTokenCreation(self):
         """Test OrganizationUserAccessTokenCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_user_access_token_creation.OrganizationUserAccessTokenCreation()  # noqa: E501
+        # model = OrganizationUserAccessTokenCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_user_signin_link.py` & `flat_api-1.0.0/test/test_score_privacy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_user_signin_link import OrganizationUserSigninLink  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_privacy import ScorePrivacy
 
 
-class TestOrganizationUserSigninLink(unittest.TestCase):
-    """OrganizationUserSigninLink unit test stubs"""
+class TestScorePrivacy(unittest.TestCase):
+    """ScorePrivacy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationUserSigninLink(self):
-        """Test OrganizationUserSigninLink"""
+    def testScorePrivacy(self):
+        """Test ScorePrivacy"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_user_signin_link.OrganizationUserSigninLink()  # noqa: E501
+        # model = ScorePrivacy()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_organization_user_signin_link_creation.py` & `flat_api-1.0.0/test/test_user_signin_link_creation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.organization_user_signin_link_creation import OrganizationUserSigninLinkCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.user_signin_link_creation import UserSigninLinkCreation
 
 
-class TestOrganizationUserSigninLinkCreation(unittest.TestCase):
-    """OrganizationUserSigninLinkCreation unit test stubs"""
+class TestUserSigninLinkCreation(unittest.TestCase):
+    """UserSigninLinkCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganizationUserSigninLinkCreation(self):
-        """Test OrganizationUserSigninLinkCreation"""
+    def testUserSigninLinkCreation(self):
+        """Test UserSigninLinkCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.organization_user_signin_link_creation.OrganizationUserSigninLinkCreation()  # noqa: E501
+        # model = UserSigninLinkCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_resource_collaborator.py` & `flat_api-1.0.0/test/test_edu_resource_move.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.resource_collaborator import ResourceCollaborator  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_move import EduResourceMove
 
 
-class TestResourceCollaborator(unittest.TestCase):
-    """ResourceCollaborator unit test stubs"""
+class TestEduResourceMove(unittest.TestCase):
+    """EduResourceMove unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testResourceCollaborator(self):
-        """Test ResourceCollaborator"""
+    def testEduResourceMove(self):
+        """Test EduResourceMove"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.resource_collaborator.ResourceCollaborator()  # noqa: E501
+        # model = EduResourceMove()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_resource_collaborator_creation.py` & `flat_api-1.0.0/test/test_resource_collaborator_creation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.resource_collaborator_creation import ResourceCollaboratorCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.resource_collaborator_creation import ResourceCollaboratorCreation
 
 
 class TestResourceCollaboratorCreation(unittest.TestCase):
     """ResourceCollaboratorCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testResourceCollaboratorCreation(self):
         """Test ResourceCollaboratorCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.resource_collaborator_creation.ResourceCollaboratorCreation()  # noqa: E501
+        # model = ResourceCollaboratorCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_resource_rights.py` & `flat_api-1.0.0/test/test_resource_rights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.resource_rights import ResourceRights  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.resource_rights import ResourceRights
 
 
 class TestResourceRights(unittest.TestCase):
     """ResourceRights unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testResourceRights(self):
         """Test ResourceRights"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.resource_rights.ResourceRights()  # noqa: E501
+        # model = ResourceRights()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_api.py` & `flat_api-1.0.0/test/test_score_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
 from flat_api.api.score_api import ScoreApi  # noqa: E501
-from flat_api.rest import ApiException
 
 
 class TestScoreApi(unittest.TestCase):
     """ScoreApi unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.score_api.ScoreApi()  # noqa: E501
+        self.api = ScoreApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_add_score_collaborator(self):
         """Test case for add_score_collaborator
```

### Comparing `flat_api-0.8.1/test/test_score_comment.py` & `flat_api-1.0.0/test/test_score_plays_counts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comment import ScoreComment  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_plays_counts import ScorePlaysCounts
 
 
-class TestScoreComment(unittest.TestCase):
-    """ScoreComment unit test stubs"""
+class TestScorePlaysCounts(unittest.TestCase):
+    """ScorePlaysCounts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreComment(self):
-        """Test ScoreComment"""
+    def testScorePlaysCounts(self):
+        """Test ScorePlaysCounts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comment.ScoreComment()  # noqa: E501
+        # model = ScorePlaysCounts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_comment_context.py` & `flat_api-1.0.0/test/test_score_comment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comment_context import ScoreCommentContext  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comment_context import ScoreCommentContext
+from flat_api.model.score_comment_moderation import ScoreCommentModeration
+globals()['ScoreCommentContext'] = ScoreCommentContext
+globals()['ScoreCommentModeration'] = ScoreCommentModeration
+from flat_api.model.score_comment import ScoreComment
 
 
-class TestScoreCommentContext(unittest.TestCase):
-    """ScoreCommentContext unit test stubs"""
+class TestScoreComment(unittest.TestCase):
+    """ScoreComment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCommentContext(self):
-        """Test ScoreCommentContext"""
+    def testScoreComment(self):
+        """Test ScoreComment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comment_context.ScoreCommentContext()  # noqa: E501
+        # model = ScoreComment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_comment_creation.py` & `flat_api-1.0.0/test/test_edu_resource_creation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comment_creation import ScoreCommentCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_type import EduResourceType
+globals()['EduResourceType'] = EduResourceType
+from flat_api.model.edu_resource_creation import EduResourceCreation
 
 
-class TestScoreCommentCreation(unittest.TestCase):
-    """ScoreCommentCreation unit test stubs"""
+class TestEduResourceCreation(unittest.TestCase):
+    """EduResourceCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCommentCreation(self):
-        """Test ScoreCommentCreation"""
+    def testEduResourceCreation(self):
+        """Test EduResourceCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comment_creation.ScoreCommentCreation()  # noqa: E501
+        # model = EduResourceCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_comment_moderation.py` & `flat_api-1.0.0/test/test_score_comment_moderation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comment_moderation import ScoreCommentModeration  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comment_moderation import ScoreCommentModeration
 
 
 class TestScoreCommentModeration(unittest.TestCase):
     """ScoreCommentModeration unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreCommentModeration(self):
         """Test ScoreCommentModeration"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comment_moderation.ScoreCommentModeration()  # noqa: E501
+        # model = ScoreCommentModeration()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_comment_update.py` & `flat_api-1.0.0/test/test_score_creation_builder_data_layout_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comment_update import ScoreCommentUpdate  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_creation_builder_data_layout_data import ScoreCreationBuilderDataLayoutData
 
 
-class TestScoreCommentUpdate(unittest.TestCase):
-    """ScoreCommentUpdate unit test stubs"""
+class TestScoreCreationBuilderDataLayoutData(unittest.TestCase):
+    """ScoreCreationBuilderDataLayoutData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCommentUpdate(self):
-        """Test ScoreCommentUpdate"""
+    def testScoreCreationBuilderDataLayoutData(self):
+        """Test ScoreCreationBuilderDataLayoutData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comment_update.ScoreCommentUpdate()  # noqa: E501
+        # model = ScoreCreationBuilderDataLayoutData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_comments_counts.py` & `flat_api-1.0.0/test/test_score_views_counts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_comments_counts import ScoreCommentsCounts  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_views_counts import ScoreViewsCounts
 
 
-class TestScoreCommentsCounts(unittest.TestCase):
-    """ScoreCommentsCounts unit test stubs"""
+class TestScoreViewsCounts(unittest.TestCase):
+    """ScoreViewsCounts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCommentsCounts(self):
-        """Test ScoreCommentsCounts"""
+    def testScoreViewsCounts(self):
+        """Test ScoreViewsCounts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_comments_counts.ScoreCommentsCounts()  # noqa: E501
+        # model = ScoreViewsCounts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation.py` & `flat_api-1.0.0/test/test_google_classroom_submission.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation import ScoreCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.google_classroom_submission import GoogleClassroomSubmission
 
 
-class TestScoreCreation(unittest.TestCase):
-    """ScoreCreation unit test stubs"""
+class TestGoogleClassroomSubmission(unittest.TestCase):
+    """GoogleClassroomSubmission unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreation(self):
-        """Test ScoreCreation"""
+    def testGoogleClassroomSubmission(self):
+        """Test GoogleClassroomSubmission"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation.ScoreCreation()  # noqa: E501
+        # model = GoogleClassroomSubmission()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation_builder_data.py` & `flat_api-1.0.0/test/test_score_creation_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation_builder_data import ScoreCreationBuilderData  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_creation_type import ScoreCreationType
 
 
-class TestScoreCreationBuilderData(unittest.TestCase):
-    """ScoreCreationBuilderData unit test stubs"""
+class TestScoreCreationType(unittest.TestCase):
+    """ScoreCreationType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreationBuilderData(self):
-        """Test ScoreCreationBuilderData"""
+    def testScoreCreationType(self):
+        """Test ScoreCreationType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation_builder_data.ScoreCreationBuilderData()  # noqa: E501
+        # model = ScoreCreationType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation_builder_data_layout_data.py` & `flat_api-1.0.0/test/test_score_creation_builder_data_score_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation_builder_data_layout_data import ScoreCreationBuilderDataLayoutData  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_creation_builder_data_score_data_instruments_inner import ScoreCreationBuilderDataScoreDataInstrumentsInner
+globals()['ScoreCreationBuilderDataScoreDataInstrumentsInner'] = ScoreCreationBuilderDataScoreDataInstrumentsInner
+from flat_api.model.score_creation_builder_data_score_data import ScoreCreationBuilderDataScoreData
 
 
-class TestScoreCreationBuilderDataLayoutData(unittest.TestCase):
-    """ScoreCreationBuilderDataLayoutData unit test stubs"""
+class TestScoreCreationBuilderDataScoreData(unittest.TestCase):
+    """ScoreCreationBuilderDataScoreData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreationBuilderDataLayoutData(self):
-        """Test ScoreCreationBuilderDataLayoutData"""
+    def testScoreCreationBuilderDataScoreData(self):
+        """Test ScoreCreationBuilderDataScoreData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation_builder_data_layout_data.ScoreCreationBuilderDataLayoutData()  # noqa: E501
+        # model = ScoreCreationBuilderDataScoreData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation_builder_data_score_data.py` & `flat_api-1.0.0/test/test_score_creation_builder_data_score_data_instruments_inner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation_builder_data_score_data import ScoreCreationBuilderDataScoreData  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_creation_builder_data_score_data_instruments_inner import ScoreCreationBuilderDataScoreDataInstrumentsInner
 
 
-class TestScoreCreationBuilderDataScoreData(unittest.TestCase):
-    """ScoreCreationBuilderDataScoreData unit test stubs"""
+class TestScoreCreationBuilderDataScoreDataInstrumentsInner(unittest.TestCase):
+    """ScoreCreationBuilderDataScoreDataInstrumentsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreationBuilderDataScoreData(self):
-        """Test ScoreCreationBuilderDataScoreData"""
+    def testScoreCreationBuilderDataScoreDataInstrumentsInner(self):
+        """Test ScoreCreationBuilderDataScoreDataInstrumentsInner"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation_builder_data_score_data.ScoreCreationBuilderDataScoreData()  # noqa: E501
+        # model = ScoreCreationBuilderDataScoreDataInstrumentsInner()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation_builder_data_score_data_instruments.py` & `flat_api-1.0.0/test/test_media_attachment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation_builder_data_score_data_instruments import ScoreCreationBuilderDataScoreDataInstruments  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.media_score_sharing_mode import MediaScoreSharingMode
+globals()['MediaScoreSharingMode'] = MediaScoreSharingMode
+from flat_api.model.media_attachment import MediaAttachment
 
 
-class TestScoreCreationBuilderDataScoreDataInstruments(unittest.TestCase):
-    """ScoreCreationBuilderDataScoreDataInstruments unit test stubs"""
+class TestMediaAttachment(unittest.TestCase):
+    """MediaAttachment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreationBuilderDataScoreDataInstruments(self):
-        """Test ScoreCreationBuilderDataScoreDataInstruments"""
+    def testMediaAttachment(self):
+        """Test MediaAttachment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation_builder_data_score_data_instruments.ScoreCreationBuilderDataScoreDataInstruments()  # noqa: E501
+        # model = MediaAttachment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_creation_type.py` & `flat_api-1.0.0/test/test_score_revision.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_creation_type import ScoreCreationType  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_revision_statistics import ScoreRevisionStatistics
+globals()['ScoreRevisionStatistics'] = ScoreRevisionStatistics
+from flat_api.model.score_revision import ScoreRevision
 
 
-class TestScoreCreationType(unittest.TestCase):
-    """ScoreCreationType unit test stubs"""
+class TestScoreRevision(unittest.TestCase):
+    """ScoreRevision unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreCreationType(self):
-        """Test ScoreCreationType"""
+    def testScoreRevision(self):
+        """Test ScoreRevision"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_creation_type.ScoreCreationType()  # noqa: E501
+        # model = ScoreRevision()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_details.py` & `flat_api-1.0.0/test/test_organization_roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_details import ScoreDetails  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.organization_roles import OrganizationRoles
 
 
-class TestScoreDetails(unittest.TestCase):
-    """ScoreDetails unit test stubs"""
+class TestOrganizationRoles(unittest.TestCase):
+    """OrganizationRoles unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreDetails(self):
-        """Test ScoreDetails"""
+    def testOrganizationRoles(self):
+        """Test OrganizationRoles"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_details.ScoreDetails()  # noqa: E501
+        # model = OrganizationRoles()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_fork.py` & `flat_api-1.0.0/test/test_score_fork.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_fork import ScoreFork  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_fork import ScoreFork
 
 
 class TestScoreFork(unittest.TestCase):
     """ScoreFork unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreFork(self):
         """Test ScoreFork"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_fork.ScoreFork()  # noqa: E501
+        # model = ScoreFork()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_license.py` & `flat_api-1.0.0/test/test_edu_library.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_license import ScoreLicense  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_library import EduLibrary
 
 
-class TestScoreLicense(unittest.TestCase):
-    """ScoreLicense unit test stubs"""
+class TestEduLibrary(unittest.TestCase):
+    """EduLibrary unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreLicense(self):
-        """Test ScoreLicense"""
+    def testEduLibrary(self):
+        """Test EduLibrary"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_license.ScoreLicense()  # noqa: E501
+        # model = EduLibrary()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_likes_counts.py` & `flat_api-1.0.0/test/test_task_progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_likes_counts import ScoreLikesCounts  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.task_progress import TaskProgress
 
 
-class TestScoreLikesCounts(unittest.TestCase):
-    """ScoreLikesCounts unit test stubs"""
+class TestTaskProgress(unittest.TestCase):
+    """TaskProgress unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreLikesCounts(self):
-        """Test ScoreLikesCounts"""
+    def testTaskProgress(self):
+        """Test TaskProgress"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_likes_counts.ScoreLikesCounts()  # noqa: E501
+        # model = TaskProgress()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_modification.py` & `flat_api-1.0.0/test/test_score_modification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_modification import ScoreModification  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_creation_type import ScoreCreationType
+from flat_api.model.score_license import ScoreLicense
+from flat_api.model.score_privacy import ScorePrivacy
+globals()['ScoreCreationType'] = ScoreCreationType
+globals()['ScoreLicense'] = ScoreLicense
+globals()['ScorePrivacy'] = ScorePrivacy
+from flat_api.model.score_modification import ScoreModification
 
 
 class TestScoreModification(unittest.TestCase):
     """ScoreModification unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreModification(self):
         """Test ScoreModification"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_modification.ScoreModification()  # noqa: E501
+        # model = ScoreModification()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_plays_counts.py` & `flat_api-1.0.0/test/test_user_community_profile_links.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_plays_counts import ScorePlaysCounts  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.user_community_profile_links import UserCommunityProfileLinks
 
 
-class TestScorePlaysCounts(unittest.TestCase):
-    """ScorePlaysCounts unit test stubs"""
+class TestUserCommunityProfileLinks(unittest.TestCase):
+    """UserCommunityProfileLinks unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScorePlaysCounts(self):
-        """Test ScorePlaysCounts"""
+    def testUserCommunityProfileLinks(self):
+        """Test UserCommunityProfileLinks"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_plays_counts.ScorePlaysCounts()  # noqa: E501
+        # model = UserCommunityProfileLinks()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_privacy.py` & `flat_api-1.0.0/test/test_class_roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_privacy import ScorePrivacy  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_roles import ClassRoles
 
 
-class TestScorePrivacy(unittest.TestCase):
-    """ScorePrivacy unit test stubs"""
+class TestClassRoles(unittest.TestCase):
+    """ClassRoles unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScorePrivacy(self):
-        """Test ScorePrivacy"""
+    def testClassRoles(self):
+        """Test ClassRoles"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_privacy.ScorePrivacy()  # noqa: E501
+        # model = ClassRoles()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_revision.py` & `flat_api-1.0.0/test/test_task_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 import unittest
 
 import flat_api
-from flat_api.models.score_revision import ScoreRevision  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.api.task_api import TaskApi  # noqa: E501
 
 
-class TestScoreRevision(unittest.TestCase):
-    """ScoreRevision unit test stubs"""
+class TestTaskApi(unittest.TestCase):
+    """TaskApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = TaskApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testScoreRevision(self):
-        """Test ScoreRevision"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_revision.ScoreRevision()  # noqa: E501
+    def test_get_task(self):
+        """Test case for get_task
+
+        Get a task details  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_revision_creation.py` & `flat_api-1.0.0/test/test_score_revision_creation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_revision_creation import ScoreRevisionCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_revision_creation import ScoreRevisionCreation
 
 
 class TestScoreRevisionCreation(unittest.TestCase):
     """ScoreRevisionCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreRevisionCreation(self):
         """Test ScoreRevisionCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_revision_creation.ScoreRevisionCreation()  # noqa: E501
+        # model = ScoreRevisionCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_revision_statistics.py` & `flat_api-1.0.0/test/test_score_revision_statistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_revision_statistics import ScoreRevisionStatistics  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_revision_statistics import ScoreRevisionStatistics
 
 
 class TestScoreRevisionStatistics(unittest.TestCase):
     """ScoreRevisionStatistics unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreRevisionStatistics(self):
         """Test ScoreRevisionStatistics"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_revision_statistics.ScoreRevisionStatistics()  # noqa: E501
+        # model = ScoreRevisionStatistics()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_source.py` & `flat_api-1.0.0/test/test_assignment_copy_response_capabilities_can_publish_in_class_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_source import ScoreSource  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_copy_response_capabilities_can_publish_in_class_error import AssignmentCopyResponseCapabilitiesCanPublishInClassError
 
 
-class TestScoreSource(unittest.TestCase):
-    """ScoreSource unit test stubs"""
+class TestAssignmentCopyResponseCapabilitiesCanPublishInClassError(unittest.TestCase):
+    """AssignmentCopyResponseCapabilitiesCanPublishInClassError unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreSource(self):
-        """Test ScoreSource"""
+    def testAssignmentCopyResponseCapabilitiesCanPublishInClassError(self):
+        """Test AssignmentCopyResponseCapabilitiesCanPublishInClassError"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_source.ScoreSource()  # noqa: E501
+        # model = AssignmentCopyResponseCapabilitiesCanPublishInClassError()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track.py` & `flat_api-1.0.0/test/test_score_track_point.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track import ScoreTrack  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_track_point import ScoreTrackPoint
 
 
-class TestScoreTrack(unittest.TestCase):
-    """ScoreTrack unit test stubs"""
+class TestScoreTrackPoint(unittest.TestCase):
+    """ScoreTrackPoint unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreTrack(self):
-        """Test ScoreTrack"""
+    def testScoreTrackPoint(self):
+        """Test ScoreTrackPoint"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track.ScoreTrack()  # noqa: E501
+        # model = ScoreTrackPoint()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track_creation.py` & `flat_api-1.0.0/test/test_class_details_canvas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track_creation import ScoreTrackCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_details_canvas import ClassDetailsCanvas
 
 
-class TestScoreTrackCreation(unittest.TestCase):
-    """ScoreTrackCreation unit test stubs"""
+class TestClassDetailsCanvas(unittest.TestCase):
+    """ClassDetailsCanvas unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreTrackCreation(self):
-        """Test ScoreTrackCreation"""
+    def testClassDetailsCanvas(self):
+        """Test ClassDetailsCanvas"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track_creation.ScoreTrackCreation()  # noqa: E501
+        # model = ClassDetailsCanvas()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track_point.py` & `flat_api-1.0.0/test/test_score_track_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track_point import ScoreTrackPoint  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_track_point import ScoreTrackPoint
+from flat_api.model.score_track_state import ScoreTrackState
+globals()['ScoreTrackPoint'] = ScoreTrackPoint
+globals()['ScoreTrackState'] = ScoreTrackState
+from flat_api.model.score_track_update import ScoreTrackUpdate
 
 
-class TestScoreTrackPoint(unittest.TestCase):
-    """ScoreTrackPoint unit test stubs"""
+class TestScoreTrackUpdate(unittest.TestCase):
+    """ScoreTrackUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreTrackPoint(self):
-        """Test ScoreTrackPoint"""
+    def testScoreTrackUpdate(self):
+        """Test ScoreTrackUpdate"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track_point.ScoreTrackPoint()  # noqa: E501
+        # model = ScoreTrackUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track_state.py` & `flat_api-1.0.0/test/test_score_track_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track_state import ScoreTrackState  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_track_state import ScoreTrackState
 
 
 class TestScoreTrackState(unittest.TestCase):
     """ScoreTrackState unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreTrackState(self):
         """Test ScoreTrackState"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track_state.ScoreTrackState()  # noqa: E501
+        # model = ScoreTrackState()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track_type.py` & `flat_api-1.0.0/test/test_score_track_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track_type import ScoreTrackType  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_track_type import ScoreTrackType
 
 
 class TestScoreTrackType(unittest.TestCase):
     """ScoreTrackType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScoreTrackType(self):
         """Test ScoreTrackType"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track_type.ScoreTrackType()  # noqa: E501
+        # model = ScoreTrackType()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_track_update.py` & `flat_api-1.0.0/test/test_score_track.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_track_update import ScoreTrackUpdate  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_track_point import ScoreTrackPoint
+from flat_api.model.score_track_state import ScoreTrackState
+from flat_api.model.score_track_type import ScoreTrackType
+globals()['ScoreTrackPoint'] = ScoreTrackPoint
+globals()['ScoreTrackState'] = ScoreTrackState
+globals()['ScoreTrackType'] = ScoreTrackType
+from flat_api.model.score_track import ScoreTrack
 
 
-class TestScoreTrackUpdate(unittest.TestCase):
-    """ScoreTrackUpdate unit test stubs"""
+class TestScoreTrack(unittest.TestCase):
+    """ScoreTrack unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreTrackUpdate(self):
-        """Test ScoreTrackUpdate"""
+    def testScoreTrack(self):
+        """Test ScoreTrack"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_track_update.ScoreTrackUpdate()  # noqa: E501
+        # model = ScoreTrack()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_score_views_counts.py` & `flat_api-1.0.0/test/test_class_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.score_views_counts import ScoreViewsCounts  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_grade_level import ClassGradeLevel
+from flat_api.model.edu_skills_focused import EduSkillsFocused
+globals()['ClassGradeLevel'] = ClassGradeLevel
+globals()['EduSkillsFocused'] = EduSkillsFocused
+from flat_api.model.class_creation import ClassCreation
 
 
-class TestScoreViewsCounts(unittest.TestCase):
-    """ScoreViewsCounts unit test stubs"""
+class TestClassCreation(unittest.TestCase):
+    """ClassCreation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScoreViewsCounts(self):
-        """Test ScoreViewsCounts"""
+    def testClassCreation(self):
+        """Test ClassCreation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.score_views_counts.ScoreViewsCounts()  # noqa: E501
+        # model = ClassCreation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_task.py` & `flat_api-1.0.0/test/test_user_signin_link.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.task import Task  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.user_signin_link import UserSigninLink
 
 
-class TestTask(unittest.TestCase):
-    """Task unit test stubs"""
+class TestUserSigninLink(unittest.TestCase):
+    """UserSigninLink unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTask(self):
-        """Test Task"""
+    def testUserSigninLink(self):
+        """Test UserSigninLink"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.task.Task()  # noqa: E501
+        # model = UserSigninLink()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_task_api.py` & `flat_api-1.0.0/test/test_edu_resource_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.api.task_api import TaskApi  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.edu_resource_update import EduResourceUpdate
 
 
-class TestTaskApi(unittest.TestCase):
-    """TaskApi unit test stubs"""
+class TestEduResourceUpdate(unittest.TestCase):
+    """EduResourceUpdate unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.task_api.TaskApi()  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    def test_get_task(self):
-        """Test case for get_task
-
-        Get a task details  # noqa: E501
-        """
+    def testEduResourceUpdate(self):
+        """Test EduResourceUpdate"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = EduResourceUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_task_export_options.py` & `flat_api-1.0.0/test/test_task_export_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.task_export_options import TaskExportOptions  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.task_export_options import TaskExportOptions
 
 
 class TestTaskExportOptions(unittest.TestCase):
     """TaskExportOptions unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testTaskExportOptions(self):
         """Test TaskExportOptions"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.task_export_options.TaskExportOptions()  # noqa: E501
+        # model = TaskExportOptions()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_task_progress.py` & `flat_api-1.0.0/test/test_score_comments_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.task_progress import TaskProgress  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.score_comments_counts import ScoreCommentsCounts
 
 
-class TestTaskProgress(unittest.TestCase):
-    """TaskProgress unit test stubs"""
+class TestScoreCommentsCounts(unittest.TestCase):
+    """ScoreCommentsCounts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTaskProgress(self):
-        """Test TaskProgress"""
+    def testScoreCommentsCounts(self):
+        """Test ScoreCommentsCounts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.task_progress.TaskProgress()  # noqa: E501
+        # model = ScoreCommentsCounts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_admin_update.py` & `flat_api-1.0.0/test/test_user_public_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_admin_update import UserAdminUpdate  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_roles import ClassRoles
+from flat_api.model.organization_roles import OrganizationRoles
+globals()['ClassRoles'] = ClassRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+from flat_api.model.user_public_summary import UserPublicSummary
 
 
-class TestUserAdminUpdate(unittest.TestCase):
-    """UserAdminUpdate unit test stubs"""
+class TestUserPublicSummary(unittest.TestCase):
+    """UserPublicSummary unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserAdminUpdate(self):
-        """Test UserAdminUpdate"""
+    def testUserPublicSummary(self):
+        """Test UserPublicSummary"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_admin_update.UserAdminUpdate()  # noqa: E501
+        # model = UserPublicSummary()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_api.py` & `flat_api-1.0.0/test/test_user_details.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.api.user_api import UserApi  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_roles import ClassRoles
+from flat_api.model.flat_locales import FlatLocales
+from flat_api.model.organization_roles import OrganizationRoles
+from flat_api.model.user_azure_details import UserAzureDetails
+from flat_api.model.user_community_profile_links import UserCommunityProfileLinks
+globals()['ClassRoles'] = ClassRoles
+globals()['FlatLocales'] = FlatLocales
+globals()['OrganizationRoles'] = OrganizationRoles
+globals()['UserAzureDetails'] = UserAzureDetails
+globals()['UserCommunityProfileLinks'] = UserCommunityProfileLinks
+from flat_api.model.user_details import UserDetails
 
 
-class TestUserApi(unittest.TestCase):
-    """UserApi unit test stubs"""
+class TestUserDetails(unittest.TestCase):
+    """UserDetails unit test stubs"""
 
     def setUp(self):
-        self.api = flat_api.api.user_api.UserApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_ger_user_likes(self):
-        """Test case for ger_user_likes
-
-        List liked scores  # noqa: E501
-        """
         pass
 
-    def test_get_user(self):
-        """Test case for get_user
-
-        Get a public user profile  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_get_user_scores(self):
-        """Test case for get_user_scores
-
-        List user's scores  # noqa: E501
-        """
+    def testUserDetails(self):
+        """Test UserDetails"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = UserDetails()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_creation.py` & `flat_api-1.0.0/test/test_assignment_copy_response_capabilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_creation import UserCreation  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.assignment_copy_response_capabilities_can_publish_in_class_error import AssignmentCopyResponseCapabilitiesCanPublishInClassError
+globals()['AssignmentCopyResponseCapabilitiesCanPublishInClassError'] = AssignmentCopyResponseCapabilitiesCanPublishInClassError
+from flat_api.model.assignment_copy_response_capabilities import AssignmentCopyResponseCapabilities
 
 
-class TestUserCreation(unittest.TestCase):
-    """UserCreation unit test stubs"""
+class TestAssignmentCopyResponseCapabilities(unittest.TestCase):
+    """AssignmentCopyResponseCapabilities unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserCreation(self):
-        """Test UserCreation"""
+    def testAssignmentCopyResponseCapabilities(self):
+        """Test AssignmentCopyResponseCapabilities"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_creation.UserCreation()  # noqa: E501
+        # model = AssignmentCopyResponseCapabilities()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_details.py` & `flat_api-1.0.0/test/test_class_grade_level.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_details import UserDetails  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_grade_level import ClassGradeLevel
 
 
-class TestUserDetails(unittest.TestCase):
-    """UserDetails unit test stubs"""
+class TestClassGradeLevel(unittest.TestCase):
+    """ClassGradeLevel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserDetails(self):
-        """Test UserDetails"""
+    def testClassGradeLevel(self):
+        """Test ClassGradeLevel"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_details.UserDetails()  # noqa: E501
+        # model = ClassGradeLevel()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_details_admin.py` & `flat_api-1.0.0/test/test_class_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_details_admin import UserDetailsAdmin  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_grade_level import ClassGradeLevel
+from flat_api.model.edu_skills_focused import EduSkillsFocused
+globals()['ClassGradeLevel'] = ClassGradeLevel
+globals()['EduSkillsFocused'] = EduSkillsFocused
+from flat_api.model.class_update import ClassUpdate
 
 
-class TestUserDetailsAdmin(unittest.TestCase):
-    """UserDetailsAdmin unit test stubs"""
+class TestClassUpdate(unittest.TestCase):
+    """ClassUpdate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserDetailsAdmin(self):
-        """Test UserDetailsAdmin"""
+    def testClassUpdate(self):
+        """Test ClassUpdate"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_details_admin.UserDetailsAdmin()  # noqa: E501
+        # model = ClassUpdate()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_details_admin_license.py` & `flat_api-1.0.0/test/test_user_details_admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_details_admin_license import UserDetailsAdminLicense  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_roles import ClassRoles
+from flat_api.model.organization_roles import OrganizationRoles
+from flat_api.model.user_details_admin_license import UserDetailsAdminLicense
+globals()['ClassRoles'] = ClassRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+globals()['UserDetailsAdminLicense'] = UserDetailsAdminLicense
+from flat_api.model.user_details_admin import UserDetailsAdmin
 
 
-class TestUserDetailsAdminLicense(unittest.TestCase):
-    """UserDetailsAdminLicense unit test stubs"""
+class TestUserDetailsAdmin(unittest.TestCase):
+    """UserDetailsAdmin unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserDetailsAdminLicense(self):
-        """Test UserDetailsAdminLicense"""
+    def testUserDetailsAdmin(self):
+        """Test UserDetailsAdmin"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_details_admin_license.UserDetailsAdminLicense()  # noqa: E501
+        # model = UserDetailsAdmin()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `flat_api-0.8.1/test/test_user_public.py` & `flat_api-1.0.0/flat_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-# coding: utf-8
+# flake8: noqa
 
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
+__version__ = "1.0.0"
 
-import unittest
+# import ApiClient
+from flat_api.api_client import ApiClient
 
-import flat_api
-from flat_api.models.user_public import UserPublic  # noqa: E501
-from flat_api.rest import ApiException
+# import Configuration
+from flat_api.configuration import Configuration
 
-
-class TestUserPublic(unittest.TestCase):
-    """UserPublic unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testUserPublic(self):
-        """Test UserPublic"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_public.UserPublic()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+# import exceptions
+from flat_api.exceptions import OpenApiException
+from flat_api.exceptions import ApiAttributeError
+from flat_api.exceptions import ApiTypeError
+from flat_api.exceptions import ApiValueError
+from flat_api.exceptions import ApiKeyError
+from flat_api.exceptions import ApiException
```

### Comparing `flat_api-0.8.1/test/test_user_public_summary.py` & `flat_api-1.0.0/test/test_user_public.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-# coding: utf-8
-
 """
     Flat API
 
     The Flat API allows you to easily extend the abilities of the [Flat Platform](https://flat.io), with a wide range of use cases including the following:  * Creating and importing new music scores using MusicXML, MIDI, Guitar Pro (GP3, GP4, GP5, GPX, GP), PowerTab, TuxGuitar and MuseScore files * Browsing, updating, copying, exporting the user's scores (for example in MP3, WAV or MIDI) * Managing educational resources with Flat for Education: creating & updating the organization accounts, the classes, rosters and assignments.  The Flat API is built on HTTP. Our API is RESTful It has predictable resource URLs. It returns HTTP response codes to indicate errors. It also accepts and returns JSON in the HTTP body. The [schema](/swagger.yaml) of this API follows the [OpenAPI Initiative (OAI) specification](https://www.openapis.org/), you can use and work with [compatible Swagger tools](http://swagger.io/open-source-integrations/). This API features Cross-Origin Resource Sharing (CORS) implemented in compliance with [W3C spec](https://www.w3.org/TR/cors/).  You can use your favorite HTTP/REST library for your programming language to use Flat's API. This specification and reference is [available on Github](https://github.com/FlatIO/api-reference).  Getting Started and learn more:  * [API Overview and introduction](https://flat.io/developers/docs/api/) * [Authentication (Personal Access Tokens or OAuth2)](https://flat.io/developers/docs/api/authentication.html) * [SDKs](https://flat.io/developers/docs/api/sdks.html) * [Rate Limits](https://flat.io/developers/docs/api/rate-limits.html) * [Changelog](https://flat.io/developers/docs/api/changelog.html)   # noqa: E501
 
-    OpenAPI spec version: 2.17.0
+    The version of the OpenAPI document: 2.18.0
     Contact: developers@flat.io
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import flat_api
-from flat_api.models.user_public_summary import UserPublicSummary  # noqa: E501
-from flat_api.rest import ApiException
+from flat_api.model.class_roles import ClassRoles
+from flat_api.model.organization_roles import OrganizationRoles
+from flat_api.model.user_community_profile_links import UserCommunityProfileLinks
+globals()['ClassRoles'] = ClassRoles
+globals()['OrganizationRoles'] = OrganizationRoles
+globals()['UserCommunityProfileLinks'] = UserCommunityProfileLinks
+from flat_api.model.user_public import UserPublic
 
 
-class TestUserPublicSummary(unittest.TestCase):
-    """UserPublicSummary unit test stubs"""
+class TestUserPublic(unittest.TestCase):
+    """UserPublic unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserPublicSummary(self):
-        """Test UserPublicSummary"""
+    def testUserPublic(self):
+        """Test UserPublic"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = flat_api.models.user_public_summary.UserPublicSummary()  # noqa: E501
+        # model = UserPublic()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```


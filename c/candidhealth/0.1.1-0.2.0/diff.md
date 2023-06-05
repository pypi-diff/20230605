# Comparing `tmp/candidhealth-0.1.1.tar.gz` & `tmp/candidhealth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.1.1.tar", max compression
+gzip compressed data, was "candidhealth-0.2.0.tar", max compression
```

## Comparing `candidhealth-0.1.1.tar` & `candidhealth-0.2.0.tar`

### file list

```diff
@@ -1,236 +1,255 @@
--rw-r--r--   0        0        0        0 2023-05-26 17:29:39.259210 candidhealth-0.1.1/README.md
--rw-r--r--   0        0        0      373 2023-05-26 17:29:39.259210 candidhealth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5601 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/__init__.py
--rw-r--r--   0        0        0     2009 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/client.py
--rw-r--r--   0        0        0      348 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      227 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/py.typed
--rw-r--r--   0        0        0     5767 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/__init__.py
--rw-r--r--   0        0        0      820 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/client.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/__init__.py
--rw-r--r--   0        0        0      304 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/__init__.py
--rw-r--r--   0        0        0     3502 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/client.py
--rw-r--r--   0        0        0      159 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      333 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      785 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
--rw-r--r--   0        0        0      806 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
--rw-r--r--   0        0        0      765 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
--rw-r--r--   0        0        0      191 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0     2831 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      256 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note.py
--rw-r--r--   0        0        0      813 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_id.py
--rw-r--r--   0        0        0      139 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1151 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     1305 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0     1928 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0       79 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/auth_0_id.py
--rw-r--r--   0        0        0       98 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0       90 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/content_download_url.py
--rw-r--r--   0        0        0       76 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0       91 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0    11148 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0    15447 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0       79 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     4686 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0    79514 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      735 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/region_national.py
--rw-r--r--   0        0        0      790 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/region_states.py
--rw-r--r--   0        0        0      633 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/regions.py
--rw-r--r--   0        0        0      864 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     6264 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1037 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0      985 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1003 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0       83 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/work_queue_id.py
--rw-r--r--   0        0        0      251 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      365 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      940 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/authorized_signatory.py
--rw-r--r--   0        0        0     1430 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract.py
--rw-r--r--   0        0        0     1517 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_base.py
--rw-r--r--   0        0        0      101 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      986 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_status.py
--rw-r--r--   0        0        0     1125 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/__init__.py
--rw-r--r--   0        0        0      886 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
--rw-r--r--   0        0        0      846 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_dates.py
--rw-r--r--   0        0        0      977 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_status.py
--rw-r--r--   0        0        0      809 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
--rw-r--r--   0        0        0      864 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
--rw-r--r--   0        0        0     2210 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span.py
--rw-r--r--   0        0        0      958 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
--rw-r--r--   0        0        0      118 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
--rw-r--r--   0        0        0      827 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/required_credentialing_dates.py
--rw-r--r--   0        0        0      279 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      958 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1904 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      903 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1092 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1284 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1244 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1244 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      832 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     2507 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/__init__.py
--rw-r--r--   0        0        0    31263 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/client.py
--rw-r--r--   0        0        0     3652 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0      103 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
--rw-r--r--   0        0        0     1206 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
--rw-r--r--   0        0        0      944 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
--rw-r--r--   0        0        0      874 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
--rw-r--r--   0        0        0      944 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
--rw-r--r--   0        0        0      894 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      659 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
--rw-r--r--   0        0        0      713 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
--rw-r--r--   0        0        0     2992 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter.py
--rw-r--r--   0        0        0      920 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
--rw-r--r--   0        0        0      388 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
--rw-r--r--   0        0        0     4498 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
--rw-r--r--   0        0        0      885 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
--rw-r--r--   0        0        0      568 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      855 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
--rw-r--r--   0        0        0      845 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      969 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
--rw-r--r--   0        0        0      891 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1303 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention.py
--rw-r--r--   0        0        0      865 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
--rw-r--r--   0        0        0      855 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab.py
--rw-r--r--   0        0        0      457 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
--rw-r--r--   0        0        0      834 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
--rw-r--r--   0        0        0      953 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/medication.py
--rw-r--r--   0        0        0      880 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status.py
--rw-r--r--   0        0        0     1164 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
--rw-r--r--   0        0        0     2615 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/note_category.py
--rw-r--r--   0        0        0      900 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
--rw-r--r--   0        0        0     1012 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
--rw-r--r--   0        0        0       77 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
--rw-r--r--   0        0        0      898 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      544 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
--rw-r--r--   0        0        0      893 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/vitals.py
--rw-r--r--   0        0        0      143 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      817 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      811 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      207 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0     5547 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      270 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/__init__.py
--rw-r--r--   0        0        0      729 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status.py
--rw-r--r--   0        0        0      981 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py
--rw-r--r--   0        0        0      399 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      545 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      821 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0      867 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1515 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      972 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1200 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      925 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      247 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1122 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1026 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      199 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      276 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      100 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_id.py
--rw-r--r--   0        0        0      849 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      501 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      704 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0      492 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
--rw-r--r--   0        0        0     2857 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1562 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
--rw-r--r--   0        0        0     1062 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0     2853 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
--rw-r--r--   0        0        0      113 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      510 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/__init__.py
--rw-r--r--   0        0        0      370 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py
--rw-r--r--   0        0        0      135 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0     4709 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      158 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/__init__.py
--rw-r--r--   0        0        0     1043 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/payer.py
--rw-r--r--   0        0        0      865 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/payer_page.py
--rw-r--r--   0        0        0      251 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0      975 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1574 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      671 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      978 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/denial_reason_content.py
--rw-r--r--   0        0        0     1104 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_id_qualifier.py
--rw-r--r--   0        0        0     1144 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line.py
--rw-r--r--   0        0        0      960 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_adjustment.py
--rw-r--r--   0        0        0      866 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base.py
--rw-r--r--   0        0        0     1899 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
--rw-r--r--   0        0        0     1618 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_create.py
--rw-r--r--   0        0        0     1099 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      917 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      799 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      861 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      113 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/__init__.py
--rw-r--r--   0        0        0      115 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/types/__init__.py
--rw-r--r--   0        0        0       97 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/types/task_id.py
--rw-r--r--   0        0        0      109 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/__init__.py
--rw-r--r--   0        0        0      108 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/types/__init__.py
--rw-r--r--   0        0        0      916 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/types/user.py
--rw-r--r--   0        0        0      111 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/__init__.py
--rw-r--r--   0        0        0      102 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/__init__.py
--rw-r--r--   0        0        0      207 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/__init__.py
--rw-r--r--   0        0        0      281 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
--rw-r--r--   0        0        0      893 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
--rw-r--r--   0        0        0     1242 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 candidhealth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      257 2023-06-05 17:07:20.463629 candidhealth-0.2.0/README.md
+-rw-r--r--   0        0        0      373 2023-06-05 17:07:20.463629 candidhealth-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5809 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/__init__.py
+-rw-r--r--   0        0        0     3166 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/candid_api_client.py
+-rw-r--r--   0        0        0     2274 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/client.py
+-rw-r--r--   0        0        0      348 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      227 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/py.typed
+-rw-r--r--   0        0        0     5975 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     3502 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      785 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      806 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      765 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      191 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      256 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note.py
+-rw-r--r--   0        0        0      813 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_id.py
+-rw-r--r--   0        0        0      139 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1151 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     1445 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0     2150 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/auth_0_id.py
+-rw-r--r--   0        0        0       98 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0      905 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/contact_info.py
+-rw-r--r--   0        0        0       90 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/content_download_url.py
+-rw-r--r--   0        0        0       76 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0       77 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/email.py
+-rw-r--r--   0        0        0       91 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0    11148 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0    15447 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0       79 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0       81 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     4686 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0      822 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      620 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/phone_number_type.py
+-rw-r--r--   0        0        0    79514 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      735 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/region_national.py
+-rw-r--r--   0        0        0      790 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/region_states.py
+-rw-r--r--   0        0        0      633 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/regions.py
+-rw-r--r--   0        0        0      864 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     6264 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1037 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0      985 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1003 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0       83 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      251 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      365 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/authorized_signatory.py
+-rw-r--r--   0        0        0     1430 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract.py
+-rw-r--r--   0        0        0     1517 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_base.py
+-rw-r--r--   0        0        0      101 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      986 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/contracts/types/contract_status.py
+-rw-r--r--   0        0        0     1125 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/credentialing/__init__.py
+-rw-r--r--   0        0        0     1472 2023-06-05 17:07:20.463629 candidhealth-0.2.0/src/candid/resources/credentialing/types/__init__.py
+-rw-r--r--   0        0        0      886 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
+-rw-r--r--   0        0        0      846 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
+-rw-r--r--   0        0        0      977 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_status.py
+-rw-r--r--   0        0        0      809 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
+-rw-r--r--   0        0        0      864 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
+-rw-r--r--   0        0        0     2210 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
+-rw-r--r--   0        0        0      958 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
+-rw-r--r--   0        0        0      118 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
+-rw-r--r--   0        0        0      827 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
+-rw-r--r--   0        0        0      279 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1904 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      903 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1092 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1260 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1244 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1244 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     2694 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    34265 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0      202 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
+-rw-r--r--   0        0        0     3794 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
+-rw-r--r--   0        0        0     1206 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
+-rw-r--r--   0        0        0      944 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
+-rw-r--r--   0        0        0      874 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      944 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      894 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      659 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0      713 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
+-rw-r--r--   0        0        0     2992 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0      920 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
+-rw-r--r--   0        0        0      388 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
+-rw-r--r--   0        0        0     4498 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      889 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
+-rw-r--r--   0        0        0      885 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      568 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      855 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
+-rw-r--r--   0        0        0      845 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      969 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      891 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1303 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      855 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      834 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
+-rw-r--r--   0        0        0      953 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0      880 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
+-rw-r--r--   0        0        0     1164 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
+-rw-r--r--   0        0        0     2615 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0      900 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
+-rw-r--r--   0        0        0     1012 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0       77 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      898 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      544 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      893 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      811 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      207 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0     5547 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      270 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status.py
+-rw-r--r--   0        0        0      981 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/client.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/__init__.py
+-rw-r--r--   0        0        0     8114 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/client.py
+-rw-r--r--   0        0        0      300 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      867 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
+-rw-r--r--   0        0        0     1020 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
+-rw-r--r--   0        0        0      804 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
+-rw-r--r--   0        0        0      435 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      821 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0      861 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1614 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient_base.py
+-rw-r--r--   0        0        0      794 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      972 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1200 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      925 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      247 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1122 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1026 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      199 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1397 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      100 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_id.py
+-rw-r--r--   0        0        0      849 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0      492 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
+-rw-r--r--   0        0        0     2857 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1562 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
+-rw-r--r--   0        0        0     1062 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0     2853 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
+-rw-r--r--   0        0        0      113 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      510 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1682 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
+-rw-r--r--   0        0        0      135 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0     4709 2023-06-05 17:07:20.467629 candidhealth-0.2.0/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      158 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/__init__.py
+-rw-r--r--   0        0        0     1043 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/payer.py
+-rw-r--r--   0        0        0      865 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/payers/types/payer_page.py
+-rw-r--r--   0        0        0      251 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0      975 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1574 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      671 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      978 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1104 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     1144 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line.py
+-rw-r--r--   0        0        0      960 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_adjustment.py
+-rw-r--r--   0        0        0      866 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base.py
+-rw-r--r--   0        0        0     1899 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
+-rw-r--r--   0        0        0     1618 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_create.py
+-rw-r--r--   0        0        0     1099 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      917 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      861 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      113 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/types/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/tasks/types/task_id.py
+-rw-r--r--   0        0        0      109 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/users/types/user.py
+-rw-r--r--   0        0        0      111 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      281 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
+-rw-r--r--   0        0        0      893 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
+-rw-r--r--   0        0        0     1242 2023-06-05 17:07:20.471629 candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.2.0/PKG-INFO
```

### Comparing `candidhealth-0.1.1/src/candid/__init__.py` & `candidhealth-0.2.0/src/candid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     AuthorizedSignatory,
     BillingNote,
     BillingNoteBase,
     BillingNoteId,
     Claim,
     ClaimId,
     ClaimStatus,
+    ContactInfo,
     ContentDownloadUrl,
     Contract,
     ContractBase,
     ContractId,
     ContractStatus,
     CredentialedEncounterStatusResult,
     CredentialingSpanDates,
@@ -23,14 +24,15 @@
     Date,
     DenialReasonContent,
     Diagnosis,
     DiagnosisCreate,
     DiagnosisId,
     DiagnosisTypeCode,
     DrugIdentification,
+    Email,
     EncounterCredentialingStatusResult,
     EncounterCredentialingStatusResult_Credentialed,
     EncounterCredentialingStatusResult_NotCredentialed,
     EncounterExternalId,
     EncounterId,
     EncounterServiceFacility,
     EncounterServiceFacilityBase,
@@ -55,19 +57,22 @@
     LinkUrl,
     MeasurementUnitCode,
     NonRequiredCredentialingDates,
     Npi,
     OrganizationId,
     PageToken,
     Patient,
+    PatientBase,
     PatientCreate,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
     Payer,
     PayerPage,
+    PhoneNumber,
+    PhoneNumberType,
     ProcedureModifier,
     ProviderCredentialingSpan,
     ProviderCredentialingSpanBase,
     ProviderCredentialingSpanId,
     RegionNational,
     Regions,
     Regions_National,
@@ -109,14 +114,15 @@
     contracts,
     credentialing,
     diagnoses,
     encounter_providers,
     encounters,
     era,
     expected_network_status,
+    guarantor,
     individual,
     insurance_card,
     invoices,
     organization_providers,
     patient_payments,
     payers,
     service_facility,
@@ -133,14 +139,15 @@
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "CandidApiEnvironment",
     "Claim",
     "ClaimId",
     "ClaimStatus",
+    "ContactInfo",
     "ContentDownloadUrl",
     "Contract",
     "ContractBase",
     "ContractId",
     "ContractStatus",
     "CredentialedEncounterStatusResult",
     "CredentialingSpanDates",
@@ -150,14 +157,15 @@
     "Date",
     "DenialReasonContent",
     "Diagnosis",
     "DiagnosisCreate",
     "DiagnosisId",
     "DiagnosisTypeCode",
     "DrugIdentification",
+    "Email",
     "EncounterCredentialingStatusResult",
     "EncounterCredentialingStatusResult_Credentialed",
     "EncounterCredentialingStatusResult_NotCredentialed",
     "EncounterExternalId",
     "EncounterId",
     "EncounterServiceFacility",
     "EncounterServiceFacilityBase",
@@ -182,19 +190,22 @@
     "LinkUrl",
     "MeasurementUnitCode",
     "NonRequiredCredentialingDates",
     "Npi",
     "OrganizationId",
     "PageToken",
     "Patient",
+    "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "Payer",
     "PayerPage",
+    "PhoneNumber",
+    "PhoneNumberType",
     "ProcedureModifier",
     "ProviderCredentialingSpan",
     "ProviderCredentialingSpanBase",
     "ProviderCredentialingSpanId",
     "RegionNational",
     "RegionStates",
     "Regions",
@@ -236,14 +247,15 @@
     "contracts",
     "credentialing",
     "diagnoses",
     "encounter_providers",
     "encounters",
     "era",
     "expected_network_status",
+    "guarantor",
     "individual",
     "insurance_card",
     "invoices",
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
```

### Comparing `candidhealth-0.1.1/src/candid/client.py` & `candidhealth-0.2.0/src/candid/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,36 +3,39 @@
 import typing
 
 from .environment import CandidApiEnvironment
 from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.billing_notes.client import AsyncBillingNotesClient, BillingNotesClient
 from .resources.encounters.client import AsyncEncountersClient, EncountersClient
 from .resources.expected_network_status.client import AsyncExpectedNetworkStatusClient, ExpectedNetworkStatusClient
+from .resources.guarantor.client import AsyncGuarantorClient, GuarantorClient
 from .resources.payers.client import AsyncPayersClient, PayersClient
 
 
 class CandidApi:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
         self.auth = AuthClient(environment=self._environment, token=self._token)
         self.encounters = EncountersClient(environment=self._environment, token=self._token)
+        self.guarantor = GuarantorClient(environment=self._environment, token=self._token)
         self.billing_notes = BillingNotesClient(environment=self._environment, token=self._token)
         self.expected_network_status = ExpectedNetworkStatusClient(environment=self._environment, token=self._token)
         self.payers = PayersClient(environment=self._environment, token=self._token)
 
 
 class AsyncCandidApi:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
         self.auth = AsyncAuthClient(environment=self._environment, token=self._token)
         self.encounters = AsyncEncountersClient(environment=self._environment, token=self._token)
+        self.guarantor = AsyncGuarantorClient(environment=self._environment, token=self._token)
         self.billing_notes = AsyncBillingNotesClient(environment=self._environment, token=self._token)
         self.expected_network_status = AsyncExpectedNetworkStatusClient(
             environment=self._environment, token=self._token
         )
         self.payers = AsyncPayersClient(environment=self._environment, token=self._token)
```

### Comparing `candidhealth-0.1.1/src/candid/core/datetime_utils.py` & `candidhealth-0.2.0/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/core/jsonable_encoder.py` & `candidhealth-0.2.0/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/__init__.py` & `candidhealth-0.2.0/src/candid/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     contracts,
     credentialing,
     diagnoses,
     encounter_providers,
     encounters,
     era,
     expected_network_status,
+    guarantor,
     individual,
     insurance_card,
     invoices,
     organization_providers,
     patient_payments,
     payers,
     service_facility,
@@ -26,26 +27,30 @@
     work_queues,
 )
 from .billing_notes import BillingNote, BillingNoteBase, BillingNoteId
 from .claims import Claim, ClaimStatus
 from .commons import (
     Auth0Id,
     ClaimId,
+    ContactInfo,
     ContentDownloadUrl,
     Date,
+    Email,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
     LinkUrl,
     Npi,
     OrganizationId,
     PageToken,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
+    PhoneNumber,
+    PhoneNumberType,
     ProcedureModifier,
     RegionNational,
     Regions,
     Regions_National,
     Regions_States,
     RegionStates,
     ResourcePage,
@@ -78,14 +83,15 @@
 from .era import Era, EraBase, EraId
 from .expected_network_status import ExpectedNetworkStatus, ExpectedNetworkStatusResponse
 from .individual import (
     Gender,
     IndividualBase,
     IndividualId,
     Patient,
+    PatientBase,
     PatientCreate,
     Subscriber,
     SubscriberBase,
     SubscriberCreate,
 )
 from .insurance_card import InsuranceCard, InsuranceCardBase, InsuranceCardCreate, InsuranceCardId
 from .invoices import Invoice, InvoiceId, InvoiceItem, InvoiceStatus
@@ -113,14 +119,15 @@
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "Claim",
     "ClaimId",
     "ClaimStatus",
+    "ContactInfo",
     "ContentDownloadUrl",
     "Contract",
     "ContractBase",
     "ContractId",
     "ContractStatus",
     "CredentialedEncounterStatusResult",
     "CredentialingSpanDates",
@@ -130,14 +137,15 @@
     "Date",
     "DenialReasonContent",
     "Diagnosis",
     "DiagnosisCreate",
     "DiagnosisId",
     "DiagnosisTypeCode",
     "DrugIdentification",
+    "Email",
     "EncounterCredentialingStatusResult",
     "EncounterCredentialingStatusResult_Credentialed",
     "EncounterCredentialingStatusResult_NotCredentialed",
     "EncounterExternalId",
     "EncounterId",
     "EncounterServiceFacility",
     "EncounterServiceFacilityBase",
@@ -162,19 +170,22 @@
     "LinkUrl",
     "MeasurementUnitCode",
     "NonRequiredCredentialingDates",
     "Npi",
     "OrganizationId",
     "PageToken",
     "Patient",
+    "PatientBase",
     "PatientCreate",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
     "Payer",
     "PayerPage",
+    "PhoneNumber",
+    "PhoneNumberType",
     "ProcedureModifier",
     "ProviderCredentialingSpan",
     "ProviderCredentialingSpanBase",
     "ProviderCredentialingSpanId",
     "RegionNational",
     "RegionStates",
     "Regions",
@@ -216,14 +227,15 @@
     "contracts",
     "credentialing",
     "diagnoses",
     "encounter_providers",
     "encounters",
     "era",
     "expected_network_status",
+    "guarantor",
     "individual",
     "insurance_card",
     "invoices",
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
```

### Comparing `candidhealth-0.1.1/src/candid/resources/auth/client.py` & `candidhealth-0.2.0/src/candid/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/client.py` & `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py` & `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py` & `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py` & `candidhealth-0.2.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/billing_notes/client.py` & `candidhealth-0.2.0/src/candid/resources/billing_notes/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note.py` & `candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_base.py` & `candidhealth-0.2.0/src/candid/resources/billing_notes/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/claims/types/claim.py` & `candidhealth-0.2.0/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.2.0/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/__init__.py` & `candidhealth-0.2.0/src/candid/resources/commons/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Auth0Id,
     ClaimId,
+    ContactInfo,
     ContentDownloadUrl,
     Date,
+    Email,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
     LinkUrl,
     Npi,
     OrganizationId,
     PageToken,
     PatientExternalId,
     PatientRelationshipToInsuredCodeAll,
+    PhoneNumber,
+    PhoneNumberType,
     ProcedureModifier,
     RegionNational,
     Regions,
     Regions_National,
     Regions_States,
     RegionStates,
     ResourcePage,
@@ -31,26 +35,30 @@
     StreetAddressShortZip,
     WorkQueueId,
 )
 
 __all__ = [
     "Auth0Id",
     "ClaimId",
+    "ContactInfo",
     "ContentDownloadUrl",
     "Date",
+    "Email",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
     "LinkUrl",
     "Npi",
     "OrganizationId",
     "PageToken",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
+    "PhoneNumber",
+    "PhoneNumberType",
     "ProcedureModifier",
     "RegionNational",
     "RegionStates",
     "Regions",
     "Regions_National",
     "Regions_States",
     "ResourcePage",
```

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .auth_0_id import Auth0Id
 from .claim_id import ClaimId
+from .contact_info import ContactInfo
 from .content_download_url import ContentDownloadUrl
 from .date import Date
+from .email import Email
 from .encounter_external_id import EncounterExternalId
 from .encounter_id import EncounterId
 from .facility_type_code import FacilityTypeCode
 from .insurance_type_code import InsuranceTypeCode
 from .link_url import LinkUrl
 from .npi import Npi
 from .organization_id import OrganizationId
 from .page_token import PageToken
 from .patient_external_id import PatientExternalId
 from .patient_relationship_to_insured_code_all import PatientRelationshipToInsuredCodeAll
+from .phone_number import PhoneNumber
+from .phone_number_type import PhoneNumberType
 from .procedure_modifier import ProcedureModifier
 from .region_national import RegionNational
 from .region_states import RegionStates
 from .regions import Regions, Regions_National, Regions_States
 from .resource_page import ResourcePage
 from .service_line_id import ServiceLineId
 from .service_line_units import ServiceLineUnits
@@ -27,26 +31,30 @@
 from .street_address_long_zip import StreetAddressLongZip
 from .street_address_short_zip import StreetAddressShortZip
 from .work_queue_id import WorkQueueId
 
 __all__ = [
     "Auth0Id",
     "ClaimId",
+    "ContactInfo",
     "ContentDownloadUrl",
     "Date",
+    "Email",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
     "LinkUrl",
     "Npi",
     "OrganizationId",
     "PageToken",
     "PatientExternalId",
     "PatientRelationshipToInsuredCodeAll",
+    "PhoneNumber",
+    "PhoneNumberType",
     "ProcedureModifier",
     "RegionNational",
     "RegionStates",
     "Regions",
     "Regions_National",
     "Regions_States",
     "ResourcePage",
```

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/region_national.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/region_national.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/region_states.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/region_states.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/regions.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/regions.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/state.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.2.0/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/contracts/types/authorized_signatory.py` & `candidhealth-0.2.0/src/candid/resources/contracts/types/authorized_signatory.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/contracts/types/contract.py` & `candidhealth-0.2.0/src/candid/resources/contracts/types/contract.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/contracts/types/contract_base.py` & `candidhealth-0.2.0/src/candid/resources/contracts/types/contract_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/contracts/types/contract_status.py` & `candidhealth-0.2.0/src/candid/resources/contracts/types/contract_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/__init__.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_dates.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_status.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/credentialing_span_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/credentialing/types/required_credentialing_dates.py` & `candidhealth-0.2.0/src/candid/resources/credentialing/types/required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.2.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.2.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
 
 
 class EncounterProviderBase(pydantic.BaseModel):
     first_name: typing.Optional[str] = pydantic.Field(
-        description=("If the billing provider is an individual, this should be set instead of organization name\n")
+        description=("If the provider is an individual, this should be set instead of organization name\n")
     )
     last_name: typing.Optional[str] = pydantic.Field(
-        description=("If the billing provider is an individual, this should be set instead of organization name\n")
+        description=("If the provider is an individual, this should be set instead of organization name\n")
     )
     organization_name: typing.Optional[str] = pydantic.Field(
-        description=("If the billing provider is an organization, this should be set instead of first + last name\n")
+        description=("If the provider is an organization, this should be set instead of first + last name\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.2.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/client.py` & `candidhealth-0.2.0/src/candid/resources/encounters/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/__init__.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .errors import EncounterExternalIdUniquenessError
 from .types import (
     AttachmentId,
     AttributableContractingStatusResult,
     AttributableContractingStatusResult_InNetwork,
     AttributableContractingStatusResult_OutOfNetwork,
     AttributableContractingStatusResult_Unknown,
     BaseAttachment,
@@ -12,14 +13,15 @@
     ClinicalNoteCategoryCreate,
     CodingAttributionType,
     ContractingOutOfOfNetworkReason,
     Encounter,
     EncounterAttachment,
     EncounterAttachmentType,
     EncounterBase,
+    EncounterExternalIdUniquenessErrorType,
     EncounterPage,
     EncounterSortOptions,
     GenerateClinicalNotesPdfResponse,
     GenerateClinicalNotesPdfResponse_Success,
     InNetworkContractingStatusResult,
     IntakeFollowUp,
     IntakeFollowUpId,
@@ -57,14 +59,16 @@
     "ClinicalNoteCategoryCreate",
     "CodingAttributionType",
     "ContractingOutOfOfNetworkReason",
     "Encounter",
     "EncounterAttachment",
     "EncounterAttachmentType",
     "EncounterBase",
+    "EncounterExternalIdUniquenessError",
+    "EncounterExternalIdUniquenessErrorType",
     "EncounterPage",
     "EncounterSortOptions",
     "GenerateClinicalNotesPdfResponse",
     "GenerateClinicalNotesPdfResponse_Success",
     "InNetworkContractingStatusResult",
     "IntakeFollowUp",
     "IntakeFollowUpId",
```

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/client.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,22 +23,26 @@
 from ....commons.types.street_address_long_zip import StreetAddressLongZip
 from ....commons.types.work_queue_id import WorkQueueId
 from ....diagnoses.types.diagnosis_create import DiagnosisCreate
 from ....diagnoses.types.diagnosis_id import DiagnosisId
 from ....encounter_providers.resources.v_2.types.billing_provider import BillingProvider
 from ....encounter_providers.resources.v_2.types.referring_provider import ReferringProvider
 from ....encounter_providers.resources.v_2.types.rendering_provider import RenderingProvider
+from ....guarantor.resources.v_1.types.guarantor_create import GuarantorCreate
+from ....guarantor.resources.v_1.types.guarantor_id import GuarantorId
 from ....individual.types.patient_create import PatientCreate
 from ....individual.types.subscriber_create import SubscriberCreate
 from ....service_facility.types.encounter_service_facility_base import EncounterServiceFacilityBase
 from ....service_lines.types.service_line_create import ServiceLineCreate
 from ....tags.types.tag_id import TagId
+from .errors.encounter_external_id_uniqueness_error import EncounterExternalIdUniquenessError
 from .types.clinical_note_category_create import ClinicalNoteCategoryCreate
 from .types.encounter import Encounter
 from .types.encounter_attachment import EncounterAttachment
+from .types.encounter_external_id_uniqueness_error_type import EncounterExternalIdUniquenessErrorType
 from .types.encounter_page import EncounterPage
 from .types.encounter_sort_options import EncounterSortOptions
 from .types.generate_clinical_notes_pdf_response import GenerateClinicalNotesPdfResponse
 from .types.intervention import Intervention
 from .types.mark_as_not_billable_response import MarkAsNotBillableResponse
 from .types.medication import Medication
 from .types.network_status_computation_results import NetworkStatusComputationResults
@@ -125,26 +129,28 @@
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         patient: PatientCreate,
+        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
         billing_provider: BillingProvider,
         rendering_provider: RenderingProvider,
         referring_provider: typing.Optional[ReferringProvider] = OMIT,
         service_facility: typing.Optional[EncounterServiceFacilityBase] = OMIT,
         subscriber_primary: typing.Optional[SubscriberCreate] = OMIT,
         subscriber_secondary: typing.Optional[SubscriberCreate] = OMIT,
         diagnoses: typing.List[DiagnosisCreate],
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         billing_notes: typing.Optional[typing.List[BillingNoteBase]] = OMIT,
         place_of_service_code: FacilityTypeCode,
         patient_histories: typing.Optional[typing.List[PatientHistoryCategory]] = OMIT,
         service_lines: typing.Optional[typing.List[ServiceLineCreate]] = OMIT,
+        guarantor: typing.Optional[GuarantorCreate] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: Date,
         end_date_of_service: typing.Optional[Date] = OMIT,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         patient_authorized_release: bool,
         benefits_assigned_to_provider: bool,
         provider_accepts_assignment: bool,
@@ -163,14 +169,16 @@
             "diagnoses": diagnoses,
             "place_of_service_code": place_of_service_code,
             "date_of_service": date_of_service,
             "patient_authorized_release": patient_authorized_release,
             "benefits_assigned_to_provider": benefits_assigned_to_provider,
             "provider_accepts_assignment": provider_accepts_assignment,
         }
+        if patient_is_self_guarantor is not OMIT:
+            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
         if referring_provider is not OMIT:
             _request["referring_provider"] = referring_provider
         if service_facility is not OMIT:
             _request["service_facility"] = service_facility
         if subscriber_primary is not OMIT:
             _request["subscriber_primary"] = subscriber_primary
         if subscriber_secondary is not OMIT:
@@ -179,14 +187,16 @@
             _request["clinical_notes"] = clinical_notes
         if billing_notes is not OMIT:
             _request["billing_notes"] = billing_notes
         if patient_histories is not OMIT:
             _request["patient_histories"] = patient_histories
         if service_lines is not OMIT:
             _request["service_lines"] = service_lines
+        if guarantor is not OMIT:
+            _request["guarantor"] = guarantor
         if external_id is not OMIT:
             _request["external_id"] = external_id
         if end_date_of_service is not OMIT:
             _request["end_date_of_service"] = end_date_of_service
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if appointment_type is not OMIT:
@@ -214,27 +224,34 @@
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
+                raise EncounterExternalIdUniquenessError(
+                    pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         encounter_id: EncounterId,
         *,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: typing.Optional[Date] = OMIT,
         diagnosis_ids: typing.Optional[typing.List[DiagnosisId]] = OMIT,
         tag_ids: typing.Optional[typing.List[TagId]] = OMIT,
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
+        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
+        guarantor_id: typing.Optional[GuarantorId] = OMIT,
     ) -> Encounter:
         _request: typing.Dict[str, typing.Any] = {}
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if external_id is not OMIT:
             _request["external_id"] = external_id
         if date_of_service is not OMIT:
@@ -243,14 +260,18 @@
             _request["diagnosis_ids"] = diagnosis_ids
         if tag_ids is not OMIT:
             _request["tag_ids"] = tag_ids
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
+        if patient_is_self_guarantor is not OMIT:
+            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
+        if guarantor_id is not OMIT:
+            _request["guarantor_id"] = guarantor_id
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -258,14 +279,19 @@
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
+                raise EncounterExternalIdUniquenessError(
+                    pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_attachments(self, encounter_id: EncounterId) -> typing.List[EncounterAttachment]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/attachments"),
             headers=remove_none_from_headers(
@@ -415,26 +441,28 @@
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         patient: PatientCreate,
+        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
         billing_provider: BillingProvider,
         rendering_provider: RenderingProvider,
         referring_provider: typing.Optional[ReferringProvider] = OMIT,
         service_facility: typing.Optional[EncounterServiceFacilityBase] = OMIT,
         subscriber_primary: typing.Optional[SubscriberCreate] = OMIT,
         subscriber_secondary: typing.Optional[SubscriberCreate] = OMIT,
         diagnoses: typing.List[DiagnosisCreate],
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         billing_notes: typing.Optional[typing.List[BillingNoteBase]] = OMIT,
         place_of_service_code: FacilityTypeCode,
         patient_histories: typing.Optional[typing.List[PatientHistoryCategory]] = OMIT,
         service_lines: typing.Optional[typing.List[ServiceLineCreate]] = OMIT,
+        guarantor: typing.Optional[GuarantorCreate] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: Date,
         end_date_of_service: typing.Optional[Date] = OMIT,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         patient_authorized_release: bool,
         benefits_assigned_to_provider: bool,
         provider_accepts_assignment: bool,
@@ -453,14 +481,16 @@
             "diagnoses": diagnoses,
             "place_of_service_code": place_of_service_code,
             "date_of_service": date_of_service,
             "patient_authorized_release": patient_authorized_release,
             "benefits_assigned_to_provider": benefits_assigned_to_provider,
             "provider_accepts_assignment": provider_accepts_assignment,
         }
+        if patient_is_self_guarantor is not OMIT:
+            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
         if referring_provider is not OMIT:
             _request["referring_provider"] = referring_provider
         if service_facility is not OMIT:
             _request["service_facility"] = service_facility
         if subscriber_primary is not OMIT:
             _request["subscriber_primary"] = subscriber_primary
         if subscriber_secondary is not OMIT:
@@ -469,14 +499,16 @@
             _request["clinical_notes"] = clinical_notes
         if billing_notes is not OMIT:
             _request["billing_notes"] = billing_notes
         if patient_histories is not OMIT:
             _request["patient_histories"] = patient_histories
         if service_lines is not OMIT:
             _request["service_lines"] = service_lines
+        if guarantor is not OMIT:
+            _request["guarantor"] = guarantor
         if external_id is not OMIT:
             _request["external_id"] = external_id
         if end_date_of_service is not OMIT:
             _request["end_date_of_service"] = end_date_of_service
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if appointment_type is not OMIT:
@@ -505,27 +537,34 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
+                raise EncounterExternalIdUniquenessError(
+                    pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         encounter_id: EncounterId,
         *,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: typing.Optional[Date] = OMIT,
         diagnosis_ids: typing.Optional[typing.List[DiagnosisId]] = OMIT,
         tag_ids: typing.Optional[typing.List[TagId]] = OMIT,
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
+        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
+        guarantor_id: typing.Optional[GuarantorId] = OMIT,
     ) -> Encounter:
         _request: typing.Dict[str, typing.Any] = {}
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if external_id is not OMIT:
             _request["external_id"] = external_id
         if date_of_service is not OMIT:
@@ -534,14 +573,18 @@
             _request["diagnosis_ids"] = diagnosis_ids
         if tag_ids is not OMIT:
             _request["tag_ids"] = tag_ids
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
+        if patient_is_self_guarantor is not OMIT:
+            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
+        if guarantor_id is not OMIT:
+            _request["guarantor_id"] = guarantor_id
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
@@ -550,14 +593,19 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
+                raise EncounterExternalIdUniquenessError(
+                    pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_attachments(self, encounter_id: EncounterId) -> typing.List[EncounterAttachment]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/attachments"),
```

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .clinical_note_category_create import ClinicalNoteCategoryCreate
 from .coding_attribution_type import CodingAttributionType
 from .contracting_out_of_of_network_reason import ContractingOutOfOfNetworkReason
 from .encounter import Encounter
 from .encounter_attachment import EncounterAttachment
 from .encounter_attachment_type import EncounterAttachmentType
 from .encounter_base import EncounterBase
+from .encounter_external_id_uniqueness_error_type import EncounterExternalIdUniquenessErrorType
 from .encounter_page import EncounterPage
 from .encounter_sort_options import EncounterSortOptions
 from .generate_clinical_notes_pdf_response import (
     GenerateClinicalNotesPdfResponse,
     GenerateClinicalNotesPdfResponse_Success,
 )
 from .in_network_contracting_status_result import InNetworkContractingStatusResult
@@ -59,14 +60,15 @@
     "ClinicalNoteCategoryCreate",
     "CodingAttributionType",
     "ContractingOutOfOfNetworkReason",
     "Encounter",
     "EncounterAttachment",
     "EncounterAttachmentType",
     "EncounterBase",
+    "EncounterExternalIdUniquenessErrorType",
     "EncounterPage",
     "EncounterSortOptions",
     "GenerateClinicalNotesPdfResponse",
     "GenerateClinicalNotesPdfResponse_Success",
     "InNetworkContractingStatusResult",
     "IntakeFollowUp",
     "IntakeFollowUpId",
```

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .....commons.types.encounter_id import EncounterId
 from .....commons.types.facility_type_code import FacilityTypeCode
 from .....commons.types.link_url import LinkUrl
 from .....diagnoses.types.diagnosis import Diagnosis
 from .....encounter_providers.resources.v_2.types.encounter_provider import EncounterProvider
 from .....individual.types.patient import Patient
 from .....individual.types.subscriber import Subscriber
-from .....patient_payments.resources.v_2.types.patient_payment import PatientPayment
+from .....patient_payments.resources.v_3.types.patient_payment import PatientPayment
 from .....service_facility.types.encounter_service_facility import EncounterServiceFacility
 from .....tags.types.tag import Tag
 from .....work_queues.resources.v_1.types.work_queue import WorkQueue
 from .clinical_note_category import ClinicalNoteCategory
 from .coding_attribution_type import CodingAttributionType
 from .encounter_base import EncounterBase
 from .patient_history_category import PatientHistoryCategory
```

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/medication.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/note_category.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/vitals.py` & `candidhealth-0.2.0/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/era/types/era.py` & `candidhealth-0.2.0/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/era/types/era_base.py` & `candidhealth-0.2.0/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.2.0/src/candid/resources/expected_network_status/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status.py` & `candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py` & `candidhealth-0.2.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/gender.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/patient.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/patient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from .individual_id import IndividualId
-from .patient_create import PatientCreate
+from .patient_base import PatientBase
 
 
-class Patient(PatientCreate):
+class Patient(PatientBase):
     individual_id: IndividualId
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,38 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.date import Date
-from ...commons.types.street_address_short_zip import StreetAddressShortZip
-from .individual_base import IndividualBase
-
-
-class PatientCreate(IndividualBase):
-    external_id: str = pydantic.Field(
-        description=(
-            "Another ID you want to associate with this patient.\n"
-            "For example, your internal patient ID or a Dr. Chrono patient ID. Box 1a on the CMS-1500 claim form\n"
-        )
-    )
-    date_of_birth: Date = pydantic.Field(
-        description=(
-            "Box 3 on the CMS-1500 claim form. The date format should be in ISO 8601 date; formatted YYYY-MM-DD (i.e. 2012-02-01)\n"
-        )
-    )
-    address: StreetAddressShortZip = pydantic.Field(description=("Box 5 on the CMS-1500 claim form.\n"))
+from ...commons.types.source_of_payment_code import SourceOfPaymentCode
+
+
+class InsuranceCardBase(pydantic.BaseModel):
+    group_number: typing.Optional[str] = pydantic.Field(description=("Box 11 on the CMS-1500 claim form.\n"))
+    plan_name: typing.Optional[str] = pydantic.Field(description=("Box 11c on the CMS-1500 claim form.\n"))
+    plan_type: typing.Optional[SourceOfPaymentCode]
+    insurance_type: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.2.0/src/candid/resources/individual/types/subscriber_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/drug_identification.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.source_of_payment_code import SourceOfPaymentCode
+from .measurement_unit_code import MeasurementUnitCode
+from .service_id_qualifier import ServiceIdQualifier
 
 
-class InsuranceCardBase(pydantic.BaseModel):
-    group_number: typing.Optional[str] = pydantic.Field(description=("Box 11 on the CMS-1500 claim form.\n"))
-    plan_name: typing.Optional[str] = pydantic.Field(description=("Box 11c on the CMS-1500 claim form.\n"))
-    plan_type: typing.Optional[SourceOfPaymentCode]
-    insurance_type: typing.Optional[str]
+class DrugIdentification(pydantic.BaseModel):
+    service_id_qualifier: ServiceIdQualifier
+    national_drug_code: str
+    national_drug_unit_count: str
+    measurement_unit_code: MeasurementUnitCode
+    link_sequence_number: typing.Optional[str]
+    pharmacy_prescription_number: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.2.0/src/candid/resources/insurance_card/types/insurance_card_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.2.0/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py` & `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py` & `candidhealth-0.2.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py` & `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....commons.types.encounter_id import EncounterId
+from .....commons.types.encounter_external_id import EncounterExternalId
 from .....commons.types.organization_id import OrganizationId
 from .....commons.types.patient_external_id import PatientExternalId
 from .....commons.types.service_line_id import ServiceLineId
 from .patient_payment_id import PatientPaymentId
 from .patient_payment_source import PatientPaymentSource
 from .patient_payment_status import PatientPaymentStatus
 
@@ -22,15 +22,15 @@
     source: PatientPaymentSource
     amount_cents: int
     payment_timestamp: typing.Optional[dt.datetime]
     status: typing.Optional[PatientPaymentStatus]
     payment_name: typing.Optional[str]
     payment_note: typing.Optional[str]
     patient_external_id: typing.Optional[PatientExternalId]
-    encounter_id: typing.Optional[EncounterId]
+    encounter_external_id: typing.Optional[EncounterExternalId]
     service_line_id: typing.Optional[ServiceLineId]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py` & `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py` & `candidhealth-0.2.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/payers/client.py` & `candidhealth-0.2.0/src/candid/resources/payers/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/payers/types/payer.py` & `candidhealth-0.2.0/src/candid/resources/payers/types/payer.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/payers/types/payer_page.py` & `candidhealth-0.2.0/src/candid/resources/payers/types/payer_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.2.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/__init__.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/__init__.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/denial_reason_content.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/drug_identification.py` & `candidhealth-0.2.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .measurement_unit_code import MeasurementUnitCode
-from .service_id_qualifier import ServiceIdQualifier
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.contact_info import ContactInfo
+from .....commons.types.street_address_long_zip import StreetAddressLongZip
 
 
-class DrugIdentification(pydantic.BaseModel):
-    service_id_qualifier: ServiceIdQualifier
-    national_drug_code: str
-    national_drug_unit_count: str
-    measurement_unit_code: MeasurementUnitCode
-    link_sequence_number: typing.Optional[str]
-    pharmacy_prescription_number: typing.Optional[str]
+class GuarantorBase(pydantic.BaseModel):
+    first_name: str
+    last_name: str
+    external_id: str
+    date_of_birth: dt.date
+    address: StreetAddressLongZip
+    contact_info: ContactInfo
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/measurement_unit_code.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_id_qualifier.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_adjustment.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_create.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_denial_reason.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_denial_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_era_data.py` & `candidhealth-0.2.0/src/candid/resources/service_lines/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/tags/types/tag.py` & `candidhealth-0.2.0/src/candid/resources/tags/types/tag.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.2.0/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.2.0/src/candid/resources/tags/types/tag_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/users/types/user.py` & `candidhealth-0.2.0/src/candid/resources/users/types/user.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue.py` & `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py` & `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py` & `candidhealth-0.2.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py`

 * *Files identical despite different names*


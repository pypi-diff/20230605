# Comparing `tmp/google_fhir_r4-0.9.2-py3-none-any.whl.zip` & `tmp/google_fhir_r4-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,185 +1,719 @@
-Zip file size: 5360934 bytes, number of entries: 183
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/__init__.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Apr-17 20:06 google/fhir/r4/fhir_path.py
--rw-r--r--  2.0 unx     8224 b- defN 23-Apr-17 20:06 google/fhir/r4/json_format.py
--rw-r--r--  2.0 unx     8526 b- defN 23-Apr-17 20:06 google/fhir/r4/primitive_handler.py
--rw-r--r--  2.0 unx     2262 b- defN 23-Apr-17 20:06 google/fhir/r4/r4_package.py
--rw-r--r--  2.0 unx     1045 b- defN 23-Apr-17 20:06 google/fhir/r4/resource_validation.py
--rw-r--r--  2.0 unx  4531911 b- defN 23-Apr-17 20:07 google/fhir/r4/data/hl7.fhir.r4.core.tgz
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/__init__.py
--rw-r--r--  2.0 unx     4145 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/fhirproto_extensions_pb2.py
--rw-r--r--  2.0 unx     6354 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/fhirproto_pb2.py
--rw-r--r--  2.0 unx     8181 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/google_extensions_pb2.py
--rw-r--r--  2.0 unx     5430 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/ml_extensions_pb2.py
--rw-r--r--  2.0 unx     3609 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/primitive_test_suite_pb2.py
--rw-r--r--  2.0 unx  1363080 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/uscore_codes_pb2.py
--rw-r--r--  2.0 unx   490992 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/uscore_pb2.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/core/__init__.py
--rw-r--r--  2.0 unx   481645 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/codes_pb2.py
--rw-r--r--  2.0 unx   192704 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/datatypes_pb2.py
--rw-r--r--  2.0 unx   430564 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/extensions_pb2.py
--rw-r--r--  2.0 unx   256371 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/valuesets_pb2.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/proto/core/resources/__init__.py
--rw-r--r--  2.0 unx     8207 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/account_pb2.py
--rw-r--r--  2.0 unx    20009 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/activity_definition_pb2.py
--rw-r--r--  2.0 unx    12409 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/adverse_event_pb2.py
--rw-r--r--  2.0 unx    20459 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
--rw-r--r--  2.0 unx    13544 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/appointment_pb2.py
--rw-r--r--  2.0 unx     6800 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/appointment_response_pb2.py
--rw-r--r--  2.0 unx    15947 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/audit_event_pb2.py
--rw-r--r--  2.0 unx     4453 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/basic_pb2.py
--rw-r--r--  2.0 unx     3381 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/binary_pb2.py
--rw-r--r--  2.0 unx    12077 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
--rw-r--r--  2.0 unx     4000 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/body_structure_pb2.py
--rw-r--r--  2.0 unx    57948 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
--rw-r--r--  2.0 unx    52078 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/capability_statement_pb2.py
--rw-r--r--  2.0 unx    26499 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/care_plan_pb2.py
--rw-r--r--  2.0 unx    13460 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/care_team_pb2.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
--rw-r--r--  2.0 unx    12070 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
--rw-r--r--  2.0 unx    14188 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/charge_item_pb2.py
--rw-r--r--  2.0 unx    32406 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/claim_pb2.py
--rw-r--r--  2.0 unx    28636 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/claim_response_pb2.py
--rw-r--r--  2.0 unx    15685 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
--rw-r--r--  2.0 unx    31726 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/code_system_pb2.py
--rw-r--r--  2.0 unx    13084 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/communication_pb2.py
--rw-r--r--  2.0 unx    14646 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/communication_request_pb2.py
--rw-r--r--  2.0 unx    21926 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/composition_pb2.py
--rw-r--r--  2.0 unx    30618 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/concept_map_pb2.py
--rw-r--r--  2.0 unx    18941 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/condition_pb2.py
--rw-r--r--  2.0 unx    22205 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/consent_pb2.py
--rw-r--r--  2.0 unx    40639 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/contract_pb2.py
--rw-r--r--  2.0 unx    15086 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
--rw-r--r--  2.0 unx    16937 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
--rw-r--r--  2.0 unx    10797 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/coverage_pb2.py
--rw-r--r--  2.0 unx    13803 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/detected_issue_pb2.py
--rw-r--r--  2.0 unx    12389 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_definition_pb2.py
--rw-r--r--  2.0 unx     9691 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_metric_pb2.py
--rw-r--r--  2.0 unx    13617 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_pb2.py
--rw-r--r--  2.0 unx    21906 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_request_pb2.py
--rw-r--r--  2.0 unx    11028 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
--rw-r--r--  2.0 unx    18783 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
--rw-r--r--  2.0 unx    13747 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/document_manifest_pb2.py
--rw-r--r--  2.0 unx    21174 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/document_reference_pb2.py
--rw-r--r--  2.0 unx     2668 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/domain_resource_pb2.py
--rw-r--r--  2.0 unx    16416 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
--rw-r--r--  2.0 unx    24578 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/encounter_pb2.py
--rw-r--r--  2.0 unx     6808 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/endpoint_pb2.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
--rw-r--r--  2.0 unx     6272 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
--rw-r--r--  2.0 unx    15586 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
--rw-r--r--  2.0 unx    10854 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/event_definition_pb2.py
--rw-r--r--  2.0 unx    10239 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/evidence_pb2.py
--rw-r--r--  2.0 unx    15011 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
--rw-r--r--  2.0 unx    17163 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/example_scenario_pb2.py
--rw-r--r--  2.0 unx    51948 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
--rw-r--r--  2.0 unx    17644 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/family_member_history_pb2.py
--rw-r--r--  2.0 unx    10517 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/flag_pb2.py
--rw-r--r--  2.0 unx    14696 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/goal_pb2.py
--rw-r--r--  2.0 unx    27335 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/graph_definition_pb2.py
--rw-r--r--  2.0 unx     9644 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/group_pb2.py
--rw-r--r--  2.0 unx     8195 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/guidance_response_pb2.py
--rw-r--r--  2.0 unx    10292 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
--rw-r--r--  2.0 unx    19394 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/imaging_study_pb2.py
--rw-r--r--  2.0 unx     8356 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
--rw-r--r--  2.0 unx    20660 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_pb2.py
--rw-r--r--  2.0 unx    10630 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
--rw-r--r--  2.0 unx    40492 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
--rw-r--r--  2.0 unx    15742 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
--rw-r--r--  2.0 unx    11997 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/invoice_pb2.py
--rw-r--r--  2.0 unx    10737 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/library_pb2.py
--rw-r--r--  2.0 unx     5474 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/linkage_pb2.py
--rw-r--r--  2.0 unx    15879 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/list_pb2.py
--rw-r--r--  2.0 unx    10784 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/location_pb2.py
--rw-r--r--  2.0 unx    15256 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/measure_pb2.py
--rw-r--r--  2.0 unx    13798 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/measure_report_pb2.py
--rw-r--r--  2.0 unx     9603 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/media_pb2.py
--rw-r--r--  2.0 unx    20081 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_administration_pb2.py
--rw-r--r--  2.0 unx    20813 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
--rw-r--r--  2.0 unx    25122 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
--rw-r--r--  2.0 unx     8655 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_pb2.py
--rw-r--r--  2.0 unx    25736 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_request_pb2.py
--rw-r--r--  2.0 unx    16838 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medication_statement_pb2.py
--rw-r--r--  2.0 unx     8121 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
--rw-r--r--  2.0 unx     6396 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
--rw-r--r--  2.0 unx     6399 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
--rw-r--r--  2.0 unx     8172 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
--rw-r--r--  2.0 unx     5575 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
--rw-r--r--  2.0 unx     4252 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
--rw-r--r--  2.0 unx     8256 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
--rw-r--r--  2.0 unx    12806 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
--rw-r--r--  2.0 unx     9456 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
--rw-r--r--  2.0 unx     3655 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
--rw-r--r--  2.0 unx    27083 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/message_definition_pb2.py
--rw-r--r--  2.0 unx    12434 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/message_header_pb2.py
--rw-r--r--  2.0 unx     4736 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
--rw-r--r--  2.0 unx    20413 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
--rw-r--r--  2.0 unx    22452 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/naming_system_pb2.py
--rw-r--r--  2.0 unx    19470 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
--rw-r--r--  2.0 unx     9643 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/observation_definition_pb2.py
--rw-r--r--  2.0 unx    30284 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/observation_pb2.py
--rw-r--r--  2.0 unx    33371 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/operation_definition_pb2.py
--rw-r--r--  2.0 unx     5813 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
--rw-r--r--  2.0 unx     7402 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
--rw-r--r--  2.0 unx     6931 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/organization_pb2.py
--rw-r--r--  2.0 unx     7778 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/parameters_pb2.py
--rw-r--r--  2.0 unx    16878 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/patient_pb2.py
--rw-r--r--  2.0 unx     7546 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/payment_notice_pb2.py
--rw-r--r--  2.0 unx    12640 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
--rw-r--r--  2.0 unx    11234 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/person_pb2.py
--rw-r--r--  2.0 unx    29886 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/plan_definition_pb2.py
--rw-r--r--  2.0 unx    10079 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/practitioner_pb2.py
--rw-r--r--  2.0 unx    10255 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
--rw-r--r--  2.0 unx    21341 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/procedure_pb2.py
--rw-r--r--  2.0 unx     9745 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/provenance_pb2.py
--rw-r--r--  2.0 unx    23215 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/questionnaire_pb2.py
--rw-r--r--  2.0 unx    11758 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
--rw-r--r--  2.0 unx    10112 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/related_person_pb2.py
--rw-r--r--  2.0 unx    23693 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/request_group_pb2.py
--rw-r--r--  2.0 unx    12354 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_definition_pb2.py
--rw-r--r--  2.0 unx    20107 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
--rw-r--r--  2.0 unx    10004 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_study_pb2.py
--rw-r--r--  2.0 unx     5870 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/research_subject_pb2.py
--rw-r--r--  2.0 unx     3335 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/resource_pb2.py
--rw-r--r--  2.0 unx    17088 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
--rw-r--r--  2.0 unx    13588 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
--rw-r--r--  2.0 unx     4777 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/schedule_pb2.py
--rw-r--r--  2.0 unx    28042 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/search_parameter_pb2.py
--rw-r--r--  2.0 unx    22943 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/service_request_pb2.py
--rw-r--r--  2.0 unx     5952 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/slot_pb2.py
--rw-r--r--  2.0 unx    10042 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
--rw-r--r--  2.0 unx    12144 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/specimen_pb2.py
--rw-r--r--  2.0 unx    37026 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/structure_definition_pb2.py
--rw-r--r--  2.0 unx    41607 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/structure_map_pb2.py
--rw-r--r--  2.0 unx     8013 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/subscription_pb2.py
--rw-r--r--  2.0 unx     5348 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
--rw-r--r--  2.0 unx     7494 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_pb2.py
--rw-r--r--  2.0 unx     7301 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
--rw-r--r--  2.0 unx     3919 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_protein_pb2.py
--rw-r--r--  2.0 unx     7891 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
--rw-r--r--  2.0 unx     8179 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
--rw-r--r--  2.0 unx    19386 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/substance_specification_pb2.py
--rw-r--r--  2.0 unx    13065 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
--rw-r--r--  2.0 unx    13766 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/supply_request_pb2.py
--rw-r--r--  2.0 unx    24739 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/task_pb2.py
--rw-r--r--  2.0 unx    31441 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
--rw-r--r--  2.0 unx    16193 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/test_report_pb2.py
--rw-r--r--  2.0 unx    39144 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/test_script_pb2.py
--rw-r--r--  2.0 unx    31172 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/value_set_pb2.py
--rw-r--r--  2.0 unx     9345 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/verification_result_pb2.py
--rw-r--r--  2.0 unx    16474 b- defN 23-Apr-17 20:07 google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/__init__.py
--rw-r--r--  2.0 unx     8965 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/local_value_set_resolver.py
--rw-r--r--  2.0 unx    10349 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/local_value_set_resolver_test.py
--rw-r--r--  2.0 unx    12355 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/terminology_service_client.py
--rw-r--r--  2.0 unx     9061 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/terminology_service_client_test.py
--rw-r--r--  2.0 unx     7948 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_set_tables.py
--rw-r--r--  2.0 unx     8259 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_set_tables_test.py
--rw-r--r--  2.0 unx    10248 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_sets.py
--rw-r--r--  2.0 unx    14084 b- defN 23-Apr-17 20:06 google/fhir/r4/terminology/value_sets_test.py
--rw-r--r--  2.0 unx     1050 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    20653 b- defN 23-Apr-17 20:07 google_fhir_r4-0.9.2.dist-info/RECORD
-183 files, 10277777 bytes uncompressed, 5326678 bytes compressed:  48.2%
+Zip file size: 7866497 bytes, number of entries: 717
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/fhir_path.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/json_format.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/primitive_handler.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/r4_package.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/proto/__init__.py
+-rw-r--r--  2.0 unx     4145 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+-rw-r--r--  2.0 unx     6354 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+-rw-r--r--  2.0 unx     5430 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+-rw-r--r--  2.0 unx  1363080 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+-rw-r--r--  2.0 unx   490992 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/uscore_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/__init__.py
+-rw-r--r--  2.0 unx   481645 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/codes_pb2.py
+-rw-r--r--  2.0 unx   192704 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+-rw-r--r--  2.0 unx   430564 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+-rw-r--r--  2.0 unx   256371 b- defN 23-Jun-05 20:11 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/__init__.py
+-rw-r--r--  2.0 unx     8207 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+-rw-r--r--  2.0 unx    12409 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+-rw-r--r--  2.0 unx    20459 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+-rw-r--r--  2.0 unx    13544 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+-rw-r--r--  2.0 unx     6800 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+-rw-r--r--  2.0 unx     4453 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+-rw-r--r--  2.0 unx    57948 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+-rw-r--r--  2.0 unx    52078 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+-rw-r--r--  2.0 unx    26499 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+-rw-r--r--  2.0 unx    12070 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+-rw-r--r--  2.0 unx    32406 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+-rw-r--r--  2.0 unx    28636 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+-rw-r--r--  2.0 unx    15685 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+-rw-r--r--  2.0 unx    31726 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+-rw-r--r--  2.0 unx    13084 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+-rw-r--r--  2.0 unx    14646 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+-rw-r--r--  2.0 unx    21926 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+-rw-r--r--  2.0 unx    30618 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+-rw-r--r--  2.0 unx    18941 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+-rw-r--r--  2.0 unx    22205 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+-rw-r--r--  2.0 unx    40639 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+-rw-r--r--  2.0 unx    15086 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+-rw-r--r--  2.0 unx    16937 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+-rw-r--r--  2.0 unx    13803 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+-rw-r--r--  2.0 unx    12389 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+-rw-r--r--  2.0 unx     9691 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+-rw-r--r--  2.0 unx    13617 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+-rw-r--r--  2.0 unx    21906 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+-rw-r--r--  2.0 unx    11028 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+-rw-r--r--  2.0 unx    18783 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+-rw-r--r--  2.0 unx    13747 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+-rw-r--r--  2.0 unx    21174 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+-rw-r--r--  2.0 unx    16416 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx    24578 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+-rw-r--r--  2.0 unx     6808 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+-rw-r--r--  2.0 unx    15586 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+-rw-r--r--  2.0 unx    10854 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+-rw-r--r--  2.0 unx    10239 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+-rw-r--r--  2.0 unx    15011 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+-rw-r--r--  2.0 unx    17163 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+-rw-r--r--  2.0 unx    51948 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+-rw-r--r--  2.0 unx    10517 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+-rw-r--r--  2.0 unx    27335 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+-rw-r--r--  2.0 unx     9644 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+-rw-r--r--  2.0 unx    10292 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+-rw-r--r--  2.0 unx    19394 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+-rw-r--r--  2.0 unx     8356 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+-rw-r--r--  2.0 unx    20660 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+-rw-r--r--  2.0 unx    10630 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+-rw-r--r--  2.0 unx    40492 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+-rw-r--r--  2.0 unx    15742 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+-rw-r--r--  2.0 unx    11997 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+-rw-r--r--  2.0 unx    10737 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+-rw-r--r--  2.0 unx     5474 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+-rw-r--r--  2.0 unx    15879 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+-rw-r--r--  2.0 unx    10784 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+-rw-r--r--  2.0 unx    15256 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+-rw-r--r--  2.0 unx    13798 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+-rw-r--r--  2.0 unx     9603 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+-rw-r--r--  2.0 unx    20813 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+-rw-r--r--  2.0 unx    25122 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+-rw-r--r--  2.0 unx     8655 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+-rw-r--r--  2.0 unx    25736 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+-rw-r--r--  2.0 unx    16838 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+-rw-r--r--  2.0 unx     6399 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+-rw-r--r--  2.0 unx     5575 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+-rw-r--r--  2.0 unx     8256 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+-rw-r--r--  2.0 unx    12806 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+-rw-r--r--  2.0 unx     3655 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+-rw-r--r--  2.0 unx    27083 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+-rw-r--r--  2.0 unx    20413 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+-rw-r--r--  2.0 unx    22452 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+-rw-r--r--  2.0 unx    19470 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+-rw-r--r--  2.0 unx    30284 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+-rw-r--r--  2.0 unx    33371 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+-rw-r--r--  2.0 unx     6931 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+-rw-r--r--  2.0 unx     7778 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+-rw-r--r--  2.0 unx    16878 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+-rw-r--r--  2.0 unx     7546 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+-rw-r--r--  2.0 unx    12640 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+-rw-r--r--  2.0 unx    29886 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+-rw-r--r--  2.0 unx    10255 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+-rw-r--r--  2.0 unx    21341 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+-rw-r--r--  2.0 unx     9745 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+-rw-r--r--  2.0 unx    23215 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+-rw-r--r--  2.0 unx    11758 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+-rw-r--r--  2.0 unx    23693 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+-rw-r--r--  2.0 unx    20107 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+-rw-r--r--  2.0 unx     5870 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+-rw-r--r--  2.0 unx    17088 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+-rw-r--r--  2.0 unx    13588 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx     4777 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+-rw-r--r--  2.0 unx    28042 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+-rw-r--r--  2.0 unx    22943 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+-rw-r--r--  2.0 unx    10042 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+-rw-r--r--  2.0 unx    37026 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+-rw-r--r--  2.0 unx    41607 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+-rw-r--r--  2.0 unx     8013 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+-rw-r--r--  2.0 unx     7891 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+-rw-r--r--  2.0 unx     8179 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+-rw-r--r--  2.0 unx    19386 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+-rw-r--r--  2.0 unx    13065 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+-rw-r--r--  2.0 unx    13766 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+-rw-r--r--  2.0 unx    24739 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+-rw-r--r--  2.0 unx    31441 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+-rw-r--r--  2.0 unx    39144 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+-rw-r--r--  2.0 unx    31172 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+-rw-r--r--  2.0 unx     9345 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+-rw-r--r--  2.0 unx    16474 b- defN 23-Jun-05 20:12 build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/terminology/__init__.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+-rw-r--r--  2.0 unx    12355 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client.py
+-rw-r--r--  2.0 unx     9061 b- defN 23-May-18 18:49 build/lib/build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+-rw-r--r--  2.0 unx     8103 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_set_tables.py
+-rw-r--r--  2.0 unx     8030 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+-rw-r--r--  2.0 unx    10248 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_sets.py
+-rw-r--r--  2.0 unx    14084 b- defN 23-May-18 18:51 build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_sets_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/fhir_path.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/json_format.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/primitive_handler.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/r4_package.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/proto/__init__.py
+-rw-r--r--  2.0 unx     4145 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+-rw-r--r--  2.0 unx     6354 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+-rw-r--r--  2.0 unx     5430 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+-rw-r--r--  2.0 unx  1363080 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+-rw-r--r--  2.0 unx   490992 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/uscore_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/proto/core/__init__.py
+-rw-r--r--  2.0 unx   481645 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/codes_pb2.py
+-rw-r--r--  2.0 unx   192704 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+-rw-r--r--  2.0 unx   430564 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+-rw-r--r--  2.0 unx   256371 b- defN 23-Jun-05 20:11 build/lib/build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/proto/core/resources/__init__.py
+-rw-r--r--  2.0 unx     8207 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+-rw-r--r--  2.0 unx    12409 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+-rw-r--r--  2.0 unx    20459 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+-rw-r--r--  2.0 unx    13544 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+-rw-r--r--  2.0 unx     6800 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+-rw-r--r--  2.0 unx     4453 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+-rw-r--r--  2.0 unx    57948 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+-rw-r--r--  2.0 unx    52078 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+-rw-r--r--  2.0 unx    26499 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+-rw-r--r--  2.0 unx    12070 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+-rw-r--r--  2.0 unx    32406 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+-rw-r--r--  2.0 unx    28636 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+-rw-r--r--  2.0 unx    15685 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+-rw-r--r--  2.0 unx    31726 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+-rw-r--r--  2.0 unx    13084 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+-rw-r--r--  2.0 unx    14646 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+-rw-r--r--  2.0 unx    21926 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+-rw-r--r--  2.0 unx    30618 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+-rw-r--r--  2.0 unx    18941 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+-rw-r--r--  2.0 unx    22205 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+-rw-r--r--  2.0 unx    40639 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+-rw-r--r--  2.0 unx    15086 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+-rw-r--r--  2.0 unx    16937 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+-rw-r--r--  2.0 unx    13803 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+-rw-r--r--  2.0 unx    12389 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+-rw-r--r--  2.0 unx     9691 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+-rw-r--r--  2.0 unx    13617 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+-rw-r--r--  2.0 unx    21906 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+-rw-r--r--  2.0 unx    11028 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+-rw-r--r--  2.0 unx    18783 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+-rw-r--r--  2.0 unx    13747 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+-rw-r--r--  2.0 unx    21174 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+-rw-r--r--  2.0 unx    16416 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx    24578 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+-rw-r--r--  2.0 unx     6808 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+-rw-r--r--  2.0 unx    15586 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+-rw-r--r--  2.0 unx    10854 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+-rw-r--r--  2.0 unx    10239 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+-rw-r--r--  2.0 unx    15011 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+-rw-r--r--  2.0 unx    17163 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+-rw-r--r--  2.0 unx    51948 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+-rw-r--r--  2.0 unx    10517 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+-rw-r--r--  2.0 unx    27335 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+-rw-r--r--  2.0 unx     9644 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+-rw-r--r--  2.0 unx    10292 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+-rw-r--r--  2.0 unx    19394 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+-rw-r--r--  2.0 unx     8356 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+-rw-r--r--  2.0 unx    20660 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+-rw-r--r--  2.0 unx    10630 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+-rw-r--r--  2.0 unx    40492 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+-rw-r--r--  2.0 unx    15742 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+-rw-r--r--  2.0 unx    11997 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+-rw-r--r--  2.0 unx    10737 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+-rw-r--r--  2.0 unx     5474 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+-rw-r--r--  2.0 unx    15879 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+-rw-r--r--  2.0 unx    10784 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+-rw-r--r--  2.0 unx    15256 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+-rw-r--r--  2.0 unx    13798 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+-rw-r--r--  2.0 unx     9603 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+-rw-r--r--  2.0 unx    20813 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+-rw-r--r--  2.0 unx    25122 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+-rw-r--r--  2.0 unx     8655 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+-rw-r--r--  2.0 unx    25736 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+-rw-r--r--  2.0 unx    16838 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+-rw-r--r--  2.0 unx     6399 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+-rw-r--r--  2.0 unx     5575 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+-rw-r--r--  2.0 unx     8256 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+-rw-r--r--  2.0 unx    12806 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+-rw-r--r--  2.0 unx     3655 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+-rw-r--r--  2.0 unx    27083 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+-rw-r--r--  2.0 unx    20413 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+-rw-r--r--  2.0 unx    22452 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+-rw-r--r--  2.0 unx    19470 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+-rw-r--r--  2.0 unx    30284 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+-rw-r--r--  2.0 unx    33371 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+-rw-r--r--  2.0 unx     6931 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+-rw-r--r--  2.0 unx     7778 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+-rw-r--r--  2.0 unx    16878 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+-rw-r--r--  2.0 unx     7546 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+-rw-r--r--  2.0 unx    12640 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+-rw-r--r--  2.0 unx    29886 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+-rw-r--r--  2.0 unx    10255 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+-rw-r--r--  2.0 unx    21341 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+-rw-r--r--  2.0 unx     9745 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+-rw-r--r--  2.0 unx    23215 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+-rw-r--r--  2.0 unx    11758 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+-rw-r--r--  2.0 unx    23693 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+-rw-r--r--  2.0 unx    20107 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+-rw-r--r--  2.0 unx     5870 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+-rw-r--r--  2.0 unx    17088 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+-rw-r--r--  2.0 unx    13588 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx     4777 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+-rw-r--r--  2.0 unx    28042 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+-rw-r--r--  2.0 unx    22943 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+-rw-r--r--  2.0 unx    10042 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+-rw-r--r--  2.0 unx    37026 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+-rw-r--r--  2.0 unx    41607 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+-rw-r--r--  2.0 unx     8013 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+-rw-r--r--  2.0 unx     7891 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+-rw-r--r--  2.0 unx     8179 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+-rw-r--r--  2.0 unx    19386 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+-rw-r--r--  2.0 unx    13065 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+-rw-r--r--  2.0 unx    13766 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+-rw-r--r--  2.0 unx    24739 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+-rw-r--r--  2.0 unx    31441 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+-rw-r--r--  2.0 unx    39144 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+-rw-r--r--  2.0 unx    31172 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+-rw-r--r--  2.0 unx     9345 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+-rw-r--r--  2.0 unx    16474 b- defN 23-Jun-05 20:12 build/lib/build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/terminology/__init__.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+-rw-r--r--  2.0 unx    12355 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client.py
+-rw-r--r--  2.0 unx     9061 b- defN 23-May-18 18:49 build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+-rw-r--r--  2.0 unx     8103 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/value_set_tables.py
+-rw-r--r--  2.0 unx     8030 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+-rw-r--r--  2.0 unx    10248 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/value_sets.py
+-rw-r--r--  2.0 unx    14084 b- defN 23-May-18 18:51 build/lib/build/lib/google/fhir/r4/terminology/value_sets_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/fhir_path.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/json_format.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/primitive_handler.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/r4_package.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/resource_validation.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/proto/__init__.py
+-rw-r--r--  2.0 unx     4145 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+-rw-r--r--  2.0 unx     6354 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+-rw-r--r--  2.0 unx     5430 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+-rw-r--r--  2.0 unx  1363080 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+-rw-r--r--  2.0 unx   490992 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/uscore_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/proto/core/__init__.py
+-rw-r--r--  2.0 unx   481645 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/codes_pb2.py
+-rw-r--r--  2.0 unx   192704 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+-rw-r--r--  2.0 unx   430564 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+-rw-r--r--  2.0 unx   256371 b- defN 23-Jun-05 20:11 build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/proto/core/resources/__init__.py
+-rw-r--r--  2.0 unx     8207 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+-rw-r--r--  2.0 unx    12409 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+-rw-r--r--  2.0 unx    20459 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+-rw-r--r--  2.0 unx    13544 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+-rw-r--r--  2.0 unx     6800 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+-rw-r--r--  2.0 unx     4453 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+-rw-r--r--  2.0 unx    57948 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+-rw-r--r--  2.0 unx    52078 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+-rw-r--r--  2.0 unx    26499 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+-rw-r--r--  2.0 unx    12070 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+-rw-r--r--  2.0 unx    32406 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+-rw-r--r--  2.0 unx    28636 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+-rw-r--r--  2.0 unx    15685 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+-rw-r--r--  2.0 unx    31726 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+-rw-r--r--  2.0 unx    13084 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+-rw-r--r--  2.0 unx    14646 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+-rw-r--r--  2.0 unx    21926 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+-rw-r--r--  2.0 unx    30618 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+-rw-r--r--  2.0 unx    18941 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+-rw-r--r--  2.0 unx    22205 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+-rw-r--r--  2.0 unx    40639 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+-rw-r--r--  2.0 unx    15086 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+-rw-r--r--  2.0 unx    16937 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+-rw-r--r--  2.0 unx    13803 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+-rw-r--r--  2.0 unx    12389 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+-rw-r--r--  2.0 unx     9691 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+-rw-r--r--  2.0 unx    13617 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+-rw-r--r--  2.0 unx    21906 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+-rw-r--r--  2.0 unx    11028 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+-rw-r--r--  2.0 unx    18783 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+-rw-r--r--  2.0 unx    13747 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+-rw-r--r--  2.0 unx    21174 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+-rw-r--r--  2.0 unx    16416 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx    24578 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+-rw-r--r--  2.0 unx     6808 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+-rw-r--r--  2.0 unx    15586 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+-rw-r--r--  2.0 unx    10854 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+-rw-r--r--  2.0 unx    10239 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+-rw-r--r--  2.0 unx    15011 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+-rw-r--r--  2.0 unx    17163 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+-rw-r--r--  2.0 unx    51948 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+-rw-r--r--  2.0 unx    10517 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+-rw-r--r--  2.0 unx    27335 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+-rw-r--r--  2.0 unx     9644 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+-rw-r--r--  2.0 unx    10292 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+-rw-r--r--  2.0 unx    19394 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+-rw-r--r--  2.0 unx     8356 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+-rw-r--r--  2.0 unx    20660 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+-rw-r--r--  2.0 unx    10630 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+-rw-r--r--  2.0 unx    40492 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+-rw-r--r--  2.0 unx    15742 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+-rw-r--r--  2.0 unx    11997 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+-rw-r--r--  2.0 unx    10737 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+-rw-r--r--  2.0 unx     5474 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+-rw-r--r--  2.0 unx    15879 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+-rw-r--r--  2.0 unx    10784 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+-rw-r--r--  2.0 unx    15256 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+-rw-r--r--  2.0 unx    13798 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+-rw-r--r--  2.0 unx     9603 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+-rw-r--r--  2.0 unx    20813 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+-rw-r--r--  2.0 unx    25122 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+-rw-r--r--  2.0 unx     8655 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+-rw-r--r--  2.0 unx    25736 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+-rw-r--r--  2.0 unx    16838 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+-rw-r--r--  2.0 unx     6399 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+-rw-r--r--  2.0 unx     5575 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+-rw-r--r--  2.0 unx     8256 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+-rw-r--r--  2.0 unx    12806 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+-rw-r--r--  2.0 unx     3655 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+-rw-r--r--  2.0 unx    27083 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+-rw-r--r--  2.0 unx    20413 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+-rw-r--r--  2.0 unx    22452 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+-rw-r--r--  2.0 unx    19470 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+-rw-r--r--  2.0 unx    30284 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+-rw-r--r--  2.0 unx    33371 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+-rw-r--r--  2.0 unx     6931 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+-rw-r--r--  2.0 unx     7778 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+-rw-r--r--  2.0 unx    16878 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+-rw-r--r--  2.0 unx     7546 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+-rw-r--r--  2.0 unx    12640 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+-rw-r--r--  2.0 unx    29886 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+-rw-r--r--  2.0 unx    10255 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+-rw-r--r--  2.0 unx    21341 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+-rw-r--r--  2.0 unx     9745 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+-rw-r--r--  2.0 unx    23215 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+-rw-r--r--  2.0 unx    11758 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+-rw-r--r--  2.0 unx    23693 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+-rw-r--r--  2.0 unx    20107 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+-rw-r--r--  2.0 unx     5870 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+-rw-r--r--  2.0 unx    17088 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+-rw-r--r--  2.0 unx    13588 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx     4777 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+-rw-r--r--  2.0 unx    28042 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+-rw-r--r--  2.0 unx    22943 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+-rw-r--r--  2.0 unx    10042 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+-rw-r--r--  2.0 unx    37026 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+-rw-r--r--  2.0 unx    41607 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+-rw-r--r--  2.0 unx     8013 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+-rw-r--r--  2.0 unx     7891 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+-rw-r--r--  2.0 unx     8179 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+-rw-r--r--  2.0 unx    19386 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+-rw-r--r--  2.0 unx    13065 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+-rw-r--r--  2.0 unx    13766 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+-rw-r--r--  2.0 unx    24739 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+-rw-r--r--  2.0 unx    31441 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+-rw-r--r--  2.0 unx    39144 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+-rw-r--r--  2.0 unx    31172 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+-rw-r--r--  2.0 unx     9345 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+-rw-r--r--  2.0 unx    16474 b- defN 23-Jun-05 20:12 build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/terminology/__init__.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+-rw-r--r--  2.0 unx    12355 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/terminology/terminology_service_client.py
+-rw-r--r--  2.0 unx     9061 b- defN 23-May-18 18:49 build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+-rw-r--r--  2.0 unx     8103 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/value_set_tables.py
+-rw-r--r--  2.0 unx     8030 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+-rw-r--r--  2.0 unx    10248 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/value_sets.py
+-rw-r--r--  2.0 unx    14084 b- defN 23-May-18 18:51 build/lib/google/fhir/r4/terminology/value_sets_test.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/r4/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-May-18 18:51 google/fhir/r4/fhir_path.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-May-18 18:49 google/fhir/r4/json_format.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-May-18 18:49 google/fhir/r4/primitive_handler.py
+-rw-r--r--  2.0 unx     2262 b- defN 23-May-18 18:51 google/fhir/r4/r4_package.py
+-rw-r--r--  2.0 unx     1045 b- defN 23-May-18 18:49 google/fhir/r4/resource_validation.py
+-rw-r--r--  2.0 unx  4531911 b- defN 23-Jun-05 20:12 google/fhir/r4/data/hl7.fhir.r4.core.tgz
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/r4/proto/__init__.py
+-rw-r--r--  2.0 unx     4145 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/fhirproto_extensions_pb2.py
+-rw-r--r--  2.0 unx     6354 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/fhirproto_pb2.py
+-rw-r--r--  2.0 unx     8181 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/google_extensions_pb2.py
+-rw-r--r--  2.0 unx     5430 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/ml_extensions_pb2.py
+-rw-r--r--  2.0 unx     3609 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/primitive_test_suite_pb2.py
+-rw-r--r--  2.0 unx  1363080 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/uscore_codes_pb2.py
+-rw-r--r--  2.0 unx   490992 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/uscore_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/r4/proto/core/__init__.py
+-rw-r--r--  2.0 unx   481645 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/codes_pb2.py
+-rw-r--r--  2.0 unx   192704 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/datatypes_pb2.py
+-rw-r--r--  2.0 unx   430564 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/core/extensions_pb2.py
+-rw-r--r--  2.0 unx   256371 b- defN 23-Jun-05 20:11 google/fhir/r4/proto/core/valuesets_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/r4/proto/core/resources/__init__.py
+-rw-r--r--  2.0 unx     8207 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/account_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+-rw-r--r--  2.0 unx    12409 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+-rw-r--r--  2.0 unx    20459 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+-rw-r--r--  2.0 unx    13544 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/appointment_pb2.py
+-rw-r--r--  2.0 unx     6800 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+-rw-r--r--  2.0 unx    15947 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/audit_event_pb2.py
+-rw-r--r--  2.0 unx     4453 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/basic_pb2.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/binary_pb2.py
+-rw-r--r--  2.0 unx    12077 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+-rw-r--r--  2.0 unx     4000 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/body_structure_pb2.py
+-rw-r--r--  2.0 unx    57948 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+-rw-r--r--  2.0 unx    52078 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+-rw-r--r--  2.0 unx    26499 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/care_plan_pb2.py
+-rw-r--r--  2.0 unx    13460 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/care_team_pb2.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+-rw-r--r--  2.0 unx    12070 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+-rw-r--r--  2.0 unx    14188 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/charge_item_pb2.py
+-rw-r--r--  2.0 unx    32406 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/claim_pb2.py
+-rw-r--r--  2.0 unx    28636 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/claim_response_pb2.py
+-rw-r--r--  2.0 unx    15685 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+-rw-r--r--  2.0 unx    31726 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/code_system_pb2.py
+-rw-r--r--  2.0 unx    13084 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/communication_pb2.py
+-rw-r--r--  2.0 unx    14646 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/communication_request_pb2.py
+-rw-r--r--  2.0 unx    21926 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/composition_pb2.py
+-rw-r--r--  2.0 unx    30618 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/concept_map_pb2.py
+-rw-r--r--  2.0 unx    18941 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/condition_pb2.py
+-rw-r--r--  2.0 unx    22205 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/consent_pb2.py
+-rw-r--r--  2.0 unx    40639 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/contract_pb2.py
+-rw-r--r--  2.0 unx    15086 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+-rw-r--r--  2.0 unx    16937 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/coverage_pb2.py
+-rw-r--r--  2.0 unx    13803 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+-rw-r--r--  2.0 unx    12389 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/device_definition_pb2.py
+-rw-r--r--  2.0 unx     9691 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/device_metric_pb2.py
+-rw-r--r--  2.0 unx    13617 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/device_pb2.py
+-rw-r--r--  2.0 unx    21906 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/device_request_pb2.py
+-rw-r--r--  2.0 unx    11028 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+-rw-r--r--  2.0 unx    18783 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+-rw-r--r--  2.0 unx    13747 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+-rw-r--r--  2.0 unx    21174 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/document_reference_pb2.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+-rw-r--r--  2.0 unx    16416 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx    24578 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/encounter_pb2.py
+-rw-r--r--  2.0 unx     6808 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/endpoint_pb2.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+-rw-r--r--  2.0 unx    15586 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+-rw-r--r--  2.0 unx    10854 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/event_definition_pb2.py
+-rw-r--r--  2.0 unx    10239 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/evidence_pb2.py
+-rw-r--r--  2.0 unx    15011 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+-rw-r--r--  2.0 unx    17163 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+-rw-r--r--  2.0 unx    51948 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+-rw-r--r--  2.0 unx    17644 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+-rw-r--r--  2.0 unx    10517 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/flag_pb2.py
+-rw-r--r--  2.0 unx    14696 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/goal_pb2.py
+-rw-r--r--  2.0 unx    27335 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+-rw-r--r--  2.0 unx     9644 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/group_pb2.py
+-rw-r--r--  2.0 unx     8195 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+-rw-r--r--  2.0 unx    10292 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+-rw-r--r--  2.0 unx    19394 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+-rw-r--r--  2.0 unx     8356 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+-rw-r--r--  2.0 unx    20660 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/immunization_pb2.py
+-rw-r--r--  2.0 unx    10630 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+-rw-r--r--  2.0 unx    40492 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+-rw-r--r--  2.0 unx    15742 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+-rw-r--r--  2.0 unx    11997 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/invoice_pb2.py
+-rw-r--r--  2.0 unx    10737 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/library_pb2.py
+-rw-r--r--  2.0 unx     5474 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/linkage_pb2.py
+-rw-r--r--  2.0 unx    15879 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/list_pb2.py
+-rw-r--r--  2.0 unx    10784 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/location_pb2.py
+-rw-r--r--  2.0 unx    15256 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/measure_pb2.py
+-rw-r--r--  2.0 unx    13798 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/measure_report_pb2.py
+-rw-r--r--  2.0 unx     9603 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/media_pb2.py
+-rw-r--r--  2.0 unx    20081 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+-rw-r--r--  2.0 unx    20813 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+-rw-r--r--  2.0 unx    25122 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+-rw-r--r--  2.0 unx     8655 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_pb2.py
+-rw-r--r--  2.0 unx    25736 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_request_pb2.py
+-rw-r--r--  2.0 unx    16838 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+-rw-r--r--  2.0 unx     6399 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+-rw-r--r--  2.0 unx     8172 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+-rw-r--r--  2.0 unx     5575 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+-rw-r--r--  2.0 unx     8256 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+-rw-r--r--  2.0 unx    12806 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+-rw-r--r--  2.0 unx     3655 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+-rw-r--r--  2.0 unx    27083 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/message_definition_pb2.py
+-rw-r--r--  2.0 unx    12434 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/message_header_pb2.py
+-rw-r--r--  2.0 unx     4736 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+-rw-r--r--  2.0 unx    20413 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+-rw-r--r--  2.0 unx    22452 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/naming_system_pb2.py
+-rw-r--r--  2.0 unx    19470 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+-rw-r--r--  2.0 unx    30284 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/observation_pb2.py
+-rw-r--r--  2.0 unx    33371 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+-rw-r--r--  2.0 unx     5813 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+-rw-r--r--  2.0 unx     6931 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/organization_pb2.py
+-rw-r--r--  2.0 unx     7778 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/parameters_pb2.py
+-rw-r--r--  2.0 unx    16878 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/patient_pb2.py
+-rw-r--r--  2.0 unx     7546 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+-rw-r--r--  2.0 unx    12640 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/person_pb2.py
+-rw-r--r--  2.0 unx    29886 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/practitioner_pb2.py
+-rw-r--r--  2.0 unx    10255 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+-rw-r--r--  2.0 unx    21341 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/procedure_pb2.py
+-rw-r--r--  2.0 unx     9745 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/provenance_pb2.py
+-rw-r--r--  2.0 unx    23215 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+-rw-r--r--  2.0 unx    11758 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+-rw-r--r--  2.0 unx    10112 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/related_person_pb2.py
+-rw-r--r--  2.0 unx    23693 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/request_group_pb2.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/research_definition_pb2.py
+-rw-r--r--  2.0 unx    20107 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/research_study_pb2.py
+-rw-r--r--  2.0 unx     5870 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/research_subject_pb2.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/resource_pb2.py
+-rw-r--r--  2.0 unx    17088 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+-rw-r--r--  2.0 unx    13588 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+-rw-r--r--  2.0 unx     4777 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/schedule_pb2.py
+-rw-r--r--  2.0 unx    28042 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+-rw-r--r--  2.0 unx    22943 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/service_request_pb2.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/slot_pb2.py
+-rw-r--r--  2.0 unx    10042 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+-rw-r--r--  2.0 unx    12144 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/specimen_pb2.py
+-rw-r--r--  2.0 unx    37026 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+-rw-r--r--  2.0 unx    41607 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/structure_map_pb2.py
+-rw-r--r--  2.0 unx     8013 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/subscription_pb2.py
+-rw-r--r--  2.0 unx     5348 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_pb2.py
+-rw-r--r--  2.0 unx     7301 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+-rw-r--r--  2.0 unx     3919 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+-rw-r--r--  2.0 unx     7891 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+-rw-r--r--  2.0 unx     8179 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+-rw-r--r--  2.0 unx    19386 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+-rw-r--r--  2.0 unx    13065 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+-rw-r--r--  2.0 unx    13766 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/supply_request_pb2.py
+-rw-r--r--  2.0 unx    24739 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/task_pb2.py
+-rw-r--r--  2.0 unx    31441 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/test_report_pb2.py
+-rw-r--r--  2.0 unx    39144 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/test_script_pb2.py
+-rw-r--r--  2.0 unx    31172 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/value_set_pb2.py
+-rw-r--r--  2.0 unx     9345 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/verification_result_pb2.py
+-rw-r--r--  2.0 unx    16474 b- defN 23-Jun-05 20:12 google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+-rw-r--r--  2.0 unx      577 b- defN 23-May-18 18:49 google/fhir/r4/terminology/__init__.py
+-rw-r--r--  2.0 unx     8965 b- defN 23-May-18 18:51 google/fhir/r4/terminology/local_value_set_resolver.py
+-rw-r--r--  2.0 unx    10349 b- defN 23-May-18 18:51 google/fhir/r4/terminology/local_value_set_resolver_test.py
+-rw-r--r--  2.0 unx    12355 b- defN 23-May-18 18:49 google/fhir/r4/terminology/terminology_service_client.py
+-rw-r--r--  2.0 unx     9061 b- defN 23-May-18 18:49 google/fhir/r4/terminology/terminology_service_client_test.py
+-rw-r--r--  2.0 unx     8103 b- defN 23-May-18 18:51 google/fhir/r4/terminology/value_set_tables.py
+-rw-r--r--  2.0 unx     8030 b- defN 23-May-18 18:51 google/fhir/r4/terminology/value_set_tables_test.py
+-rw-r--r--  2.0 unx    10248 b- defN 23-May-18 18:51 google/fhir/r4/terminology/value_sets.py
+-rw-r--r--  2.0 unx    14084 b- defN 23-May-18 18:51 google/fhir/r4/terminology/value_sets_test.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-Jun-05 20:34 google_fhir_r4-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 20:34 google_fhir_r4-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-05 20:34 google_fhir_r4-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    92018 b- defN 23-Jun-05 20:34 google_fhir_r4-0.9.3.dist-info/RECORD
+717 files, 27521044 bytes uncompressed, 7710495 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,7 +1,1609 @@
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/fhir_path.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/json_format.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/primitive_handler.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/r4_package.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/resource_validation.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/uscore_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/codes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_set_tables.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_sets.py
+Comment: 
+
+Filename: build/lib/build/lib/build/lib/google/fhir/r4/terminology/value_sets_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/fhir_path.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/json_format.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/primitive_handler.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/r4_package.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/resource_validation.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/uscore_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/codes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/__init__.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/value_set_tables.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/value_sets.py
+Comment: 
+
+Filename: build/lib/build/lib/google/fhir/r4/terminology/value_sets_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/fhir_path.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/json_format.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/primitive_handler.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/r4_package.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/resource_validation.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/fhirproto_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/fhirproto_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/google_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/ml_extensions_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/primitive_test_suite_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/uscore_codes_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/uscore_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/codes_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/datatypes_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/extensions_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/valuesets_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/account_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/activity_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/adverse_event_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/allergy_intolerance_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/appointment_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/appointment_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/audit_event_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/basic_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/binary_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/biologically_derived_product_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/body_structure_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/bundle_and_contained_resource_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/capability_statement_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/care_plan_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/care_team_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/catalog_entry_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/charge_item_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/charge_item_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/claim_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/claim_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/clinical_impression_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/code_system_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/communication_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/communication_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/compartment_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/composition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/concept_map_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/condition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/consent_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/contract_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_eligibility_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/coverage_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/detected_issue_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/device_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/device_metric_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/device_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/device_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/device_use_statement_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/diagnostic_report_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/document_manifest_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/document_reference_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/domain_resource_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/effect_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/encounter_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/endpoint_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/enrollment_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/enrollment_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/episode_of_care_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/event_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/evidence_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/evidence_variable_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/example_scenario_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/explanation_of_benefit_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/family_member_history_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/flag_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/goal_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/graph_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/group_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/guidance_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/healthcare_service_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/imaging_study_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_evaluation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/immunization_recommendation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/implementation_guide_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/insurance_plan_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/invoice_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/library_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/linkage_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/list_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/location_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/measure_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/measure_report_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/media_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_administration_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_dispense_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_knowledge_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medication_statement_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_authorization_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_contraindication_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_indication_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_ingredient_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_interaction_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_manufactured_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_packaged_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_pharmaceutical_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/medicinal_product_undesirable_effect_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/message_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/message_header_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/metadata_resource_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/molecular_sequence_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/naming_system_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/nutrition_order_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/observation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/observation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/operation_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/operation_outcome_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/organization_affiliation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/organization_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/parameters_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/patient_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/payment_notice_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/payment_reconciliation_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/person_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/plan_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/practitioner_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/practitioner_role_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/procedure_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/provenance_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/questionnaire_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/questionnaire_response_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/related_person_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/request_group_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/research_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/research_element_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/research_study_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/research_subject_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/resource_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/risk_assessment_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/risk_evidence_synthesis_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/schedule_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/search_parameter_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/service_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/slot_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/specimen_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/specimen_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/structure_definition_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/structure_map_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/subscription_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_nucleic_acid_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_polymer_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_protein_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_reference_information_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_source_material_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/substance_specification_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/supply_delivery_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/supply_request_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/task_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/terminology_capabilities_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/test_report_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/test_script_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/value_set_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/verification_result_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/proto/core/resources/vision_prescription_pb2.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/__init__.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/local_value_set_resolver.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/local_value_set_resolver_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/terminology_service_client.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/terminology_service_client_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/value_set_tables.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/value_set_tables_test.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/value_sets.py
+Comment: 
+
+Filename: build/lib/google/fhir/r4/terminology/value_sets_test.py
+Comment: 
+
 Filename: google/fhir/r4/__init__.py
 Comment: 
 
 Filename: google/fhir/r4/fhir_path.py
 Comment: 
 
 Filename: google/fhir/r4/json_format.py
@@ -531,20 +2133,20 @@
 
 Filename: google/fhir/r4/terminology/value_sets.py
 Comment: 
 
 Filename: google/fhir/r4/terminology/value_sets_test.py
 Comment: 
 
-Filename: google_fhir_r4-0.9.2.dist-info/METADATA
+Filename: google_fhir_r4-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: google_fhir_r4-0.9.2.dist-info/WHEEL
+Filename: google_fhir_r4-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: google_fhir_r4-0.9.2.dist-info/top_level.txt
+Filename: google_fhir_r4-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: google_fhir_r4-0.9.2.dist-info/RECORD
+Filename: google_fhir_r4-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## google/fhir/r4/terminology/value_set_tables.py

```diff
@@ -26,15 +26,16 @@
 
 from google.fhir.r4.proto.core.resources import value_set_pb2
 
 
 def valueset_codes_insert_statement_for(
     expanded_value_sets: Iterable[value_set_pb2.ValueSet],
     table: sqlalchemy.sql.expression.TableClause,
-    batch_size: int = 500) -> Iterable[sqlalchemy.sql.dml.Insert]:
+    batch_size: int = 500,
+) -> Iterable[sqlalchemy.sql.dml.Insert]:
   """Builds INSERT statements for placing value sets' codes into a given table.
 
   The INSERT may be used to build a valueset_codes table as described by:
   https://github.com/FHIR/sql-on-fhir/blob/master/sql-on-fhir.md#valueset-support
 
   Returns an sqlalchemy insert expression which inserts all of the value set's
   expanded codes into the given table which do not already exist in the table.
@@ -58,24 +59,34 @@
     batch_size number of rows.
   Raises:
     ValueError: If the given table does not have the expected columns.
   """
   expected_cols = ('valueseturi', 'valuesetversion', 'system', 'code')
   missing_cols = [col for col in expected_cols if col not in table.columns]
   if missing_cols:
-    raise ValueError('Table %s missing expected columns: %s' %
-                     (table, ', '.join(missing_cols)))
-
-  def value_set_codes() -> Iterable[Tuple[
-      value_set_pb2.ValueSet, value_set_pb2.ValueSet.Expansion.Contains]]:
+    raise ValueError(
+        'Table %s missing expected columns: %s'
+        % (table, ', '.join(missing_cols))
+    )
+
+  def value_set_codes() -> (
+      Iterable[
+          Tuple[
+              value_set_pb2.ValueSet, value_set_pb2.ValueSet.Expansion.Contains
+          ]
+      ]
+  ):
     """Yields (value_set, code) tuples for each code in each value set."""
     for value_set in expanded_value_sets:
       if not value_set.expansion.contains:
-        logging.warning('Value set: %s version: %s has no expanded codes',
-                        value_set.url.value, value_set.version.value)
+        logging.warning(
+            'Value set: %s version: %s has no expanded codes',
+            value_set.url.value,
+            value_set.version.value,
+        )
       for code in value_set.expansion.contains:
         yield value_set, code
 
   # Break the value set codes into batches.
   batch_iterables = [iter(value_set_codes())] * batch_size
   batches = itertools.zip_longest(*batch_iterables)
 
@@ -87,35 +98,43 @@
       if pair is not None:
         value_set, code = pair
         code_literals.append(_code_as_select_literal(value_set, code))
 
     # UNION each SELECT to build a single select subquery for all codes.
     codes = sqlalchemy.union_all(*code_literals).alias('codes')
     # Filter the codes to those not already present in `table` with a LEFT JOIN.
-    new_codes = sqlalchemy.select((codes,)).select_from(
-        codes.outerjoin(
-            table,
-            sqlalchemy.and_(
-                codes.c.valueseturi == table.c.valueseturi,
-                codes.c.valuesetversion == table.c.valuesetversion,
-                codes.c.system == table.c.system,
-                codes.c.code == table.c.code,
-            ))).where(
+    new_codes = (
+        sqlalchemy.select(codes)
+        .select_from(
+            codes.outerjoin(
+                table,
                 sqlalchemy.and_(
-                    table.c.valueseturi.is_(None),
-                    table.c.valuesetversion.is_(None),
-                    table.c.system.is_(None),
-                    table.c.code.is_(None),
-                ))
-    yield table.insert().from_select(new_codes.columns, new_codes)
+                    codes.c.valueseturi == table.c.valueseturi,
+                    codes.c.valuesetversion == table.c.valuesetversion,
+                    codes.c.system == table.c.system,
+                    codes.c.code == table.c.code,
+                ),
+            )
+        )
+        .where(
+            sqlalchemy.and_(
+                table.c.valueseturi.is_(None),
+                table.c.valuesetversion.is_(None),
+                table.c.system.is_(None),
+                table.c.code.is_(None),
+            )
+        )
+    )
+    yield table.insert().from_select(new_codes.subquery().columns, new_codes)
 
 
 def get_num_code_systems_per_value_set(
     engine: sqlalchemy.engine.base.Engine,
-    table: sqlalchemy.sql.expression.TableClause) -> Dict[str, int]:
+    table: sqlalchemy.sql.expression.TableClause,
+) -> Dict[str, int]:
   """Queries `table` for the code systems referenced by each value set.
 
   Looks up the code systems referenced by each value set decribed in the
   valueset_codes `table`. Returns counts for the number of code systems
   referenced by each value set.
 
   If the value sets' URL contains a "|version" suffix, reports the number of
@@ -129,58 +148,63 @@
 
   Returns:
     A CodeSystemCounts object for accessing code systems information.
   """
   query = sqlalchemy.select([
       table.c.valueseturi,
       table.c.valuesetversion,
-      sqlalchemy.func.array_agg(sqlalchemy.distinct(
-          table.c.system)).label('systems'),
+      sqlalchemy.func.array_agg(sqlalchemy.distinct(table.c.system)).label(
+          'systems'
+      ),
   ]).group_by(table.c.valueseturi, table.c.valuesetversion)
   with engine.connect() as connection:
     systems_per_value_set = connection.execute(query)
     return _query_results_to_code_system_counts(
-        systems_per_value_set.fetchall())
+        systems_per_value_set.fetchall()
+    )
 
 
 def _query_results_to_code_system_counts(
     query_results
 ) -> Dict[str, int]:
   """Converts query results to a map of value set to code system counts."""
   # Build a map of {value_set_url: {value_set_version: [code_systems]}}
   systems_per_value_set: Dict[str, Dict[str, Collection[str]]] = {}
   for row in query_results:
     value_set_version = row.valuesetversion or ''
-    systems_per_value_set.setdefault(row.valueseturi,
-                                     {})[value_set_version] = row.systems
+    systems_per_value_set.setdefault(row.valueseturi, {})[
+        value_set_version
+    ] = row.systems
 
   # Convert the above map to {value_set_url|version: num_codes_systems}
   # Rows without versions inherit code systems from all value sets with the same
   # base URL.
   num_systems_per_url: Dict[str, int] = {}
   for value_set_url, systems_per_version in systems_per_value_set.items():
     for version, systems in systems_per_version.items():
       if version:
         num_systems_per_url['%s|%s' % (value_set_url, version)] = len(systems)
       # Also add a lookup for the version-less URL.
       num_systems_per_url[value_set_url] = len(
-          set(itertools.chain.from_iterable(systems_per_version.values())))
+          set(itertools.chain.from_iterable(systems_per_version.values()))
+      )
   return num_systems_per_url
 
 
 def _code_as_select_literal(
     value_set: value_set_pb2.ValueSet,
-    code: value_set_pb2.ValueSet.Expansion.Contains) -> sqlalchemy.select:
+    code: value_set_pb2.ValueSet.Expansion.Contains,
+) -> sqlalchemy.select:
   """Builds a SELECT statement for the literals in the given code."""
-  return sqlalchemy.select((
+  return sqlalchemy.select(
       _literal_or_null(value_set.url.value).label('valueseturi'),
       _literal_or_null(value_set.version.value).label('valuesetversion'),
       _literal_or_null(code.system.value).label('system'),
       _literal_or_null(code.code.value).label('code'),
-  ))
+  )
 
 
 def _literal_or_null(val: str) -> sqlalchemy.sql.elements.ColumnElement:
   """Returns a literal for the given string or NULL for an empty string."""
   if val:
     return sqlalchemy.sql.expression.literal(val)
   else:
```

## google/fhir/r4/terminology/value_set_tables_test.py

```diff
@@ -32,53 +32,54 @@
     for code, system in (('c1', 's1'), ('c2', 's2'), ('c3', 's3')):
       coding = value_set.expansion.contains.add()
       coding.code.value = code
       coding.system.value = system
 
     table = build_valueset_codes_table()
 
-    result = value_set_tables.valueset_codes_insert_statement_for([value_set],
-                                                                  table)
+    result = value_set_tables.valueset_codes_insert_statement_for(
+        [value_set], table
+    )
     query = list(result)[0]
     query_string = str(query.compile(compile_kwargs={'literal_binds': True}))
-    self.assertEqual(query_string, (
-        'INSERT INTO valueset_codes (valueseturi, valuesetversion, system, code) '
-        'SELECT codes.valueseturi, codes.valuesetversion, codes.system, codes.code '
-        '\nFROM ('
-        "SELECT 'vs-url' AS valueseturi, 'vs-version' AS valuesetversion, 's1' AS system, 'c1' AS code "
-        'UNION ALL '
-        "SELECT 'vs-url' AS valueseturi, 'vs-version' AS valuesetversion, 's2' AS system, 'c2' AS code "
-        'UNION ALL '
-        "SELECT 'vs-url' AS valueseturi, 'vs-version' AS valuesetversion, 's3' AS system, 'c3' AS code"
-        ') AS codes '
-        'LEFT OUTER JOIN valueset_codes '
-        'ON codes.valueseturi = valueset_codes.valueseturi '
-        'AND codes.valuesetversion = valueset_codes.valuesetversion '
-        'AND codes.system = valueset_codes.system '
-        'AND codes.code = valueset_codes.code '
-        '\nWHERE valueset_codes.valueseturi IS NULL '
-        'AND valueset_codes.valuesetversion IS NULL '
-        'AND valueset_codes.system IS NULL '
-        'AND valueset_codes.code IS NULL'))
+    self.assertEqual(
+        query_string,
+        (
+            'INSERT INTO valueset_codes (valueseturi, valuesetversion, system,'
+            ' code) SELECT codes.valueseturi, codes.valuesetversion,'
+            " codes.system, codes.code \nFROM (SELECT 'vs-url' AS valueseturi,"
+            " 'vs-version' AS valuesetversion, 's1' AS system, 'c1' AS code"
+            " UNION ALL SELECT 'vs-url' AS valueseturi, 'vs-version' AS"
+            " valuesetversion, 's2' AS system, 'c2' AS code UNION ALL SELECT"
+            " 'vs-url' AS valueseturi, 'vs-version' AS valuesetversion, 's3' AS"
+            " system, 'c3' AS code) AS codes LEFT OUTER JOIN valueset_codes ON"
+            ' codes.valueseturi = valueset_codes.valueseturi AND'
+            ' codes.valuesetversion = valueset_codes.valuesetversion AND'
+            ' codes.system = valueset_codes.system AND codes.code ='
+            ' valueset_codes.code \nWHERE valueset_codes.valueseturi IS NULL'
+            ' AND valueset_codes.valuesetversion IS NULL AND'
+            ' valueset_codes.system IS NULL AND valueset_codes.code IS NULL'
+        ),
+    )
 
   def testValueSetToInsertStatement_withBatches_buildsBatchedInserts(self):
     value_set = value_set_pb2.ValueSet()
     value_set.url.value = 'vs-url'
     value_set.version.value = 'vs-version'
 
     for code, system in (('c1', 's1'), ('c2', 's2'), ('c3', 's3')):
       coding = value_set.expansion.contains.add()
       coding.code.value = code
       coding.system.value = system
 
     table = build_valueset_codes_table()
 
-    result = value_set_tables.valueset_codes_insert_statement_for([value_set],
-                                                                  table,
-                                                                  batch_size=2)
+    result = value_set_tables.valueset_codes_insert_statement_for(
+        [value_set], table, batch_size=2
+    )
     expected_1 = (
         'INSERT INTO valueset_codes '
         '(valueseturi, valuesetversion, system, code) '
         'SELECT '
         'codes.valueseturi, codes.valuesetversion, codes.system, codes.code '
         '\nFROM ('
         "SELECT 'vs-url' AS valueseturi, 'vs-version' AS valuesetversion, "
@@ -91,15 +92,16 @@
         'ON codes.valueseturi = valueset_codes.valueseturi '
         'AND codes.valuesetversion = valueset_codes.valuesetversion '
         'AND codes.system = valueset_codes.system '
         'AND codes.code = valueset_codes.code '
         '\nWHERE valueset_codes.valueseturi IS NULL '
         'AND valueset_codes.valuesetversion IS NULL '
         'AND valueset_codes.system IS NULL '
-        'AND valueset_codes.code IS NULL')
+        'AND valueset_codes.code IS NULL'
+    )
 
     expected_2 = (
         'INSERT INTO valueset_codes '
         '(valueseturi, valuesetversion, system, code) '
         'SELECT '
         'codes.valueseturi, codes.valuesetversion, codes.system, codes.code '
         '\nFROM ('
@@ -110,15 +112,16 @@
         'ON codes.valueseturi = valueset_codes.valueseturi '
         'AND codes.valuesetversion = valueset_codes.valuesetversion '
         'AND codes.system = valueset_codes.system '
         'AND codes.code = valueset_codes.code '
         '\nWHERE valueset_codes.valueseturi IS NULL '
         'AND valueset_codes.valuesetversion IS NULL '
         'AND valueset_codes.system IS NULL '
-        'AND valueset_codes.code IS NULL')
+        'AND valueset_codes.code IS NULL'
+    )
 
     result_queries = [
         str(query.compile(compile_kwargs={'literal_binds': True}))
         for query in result
     ]
     self.assertListEqual(result_queries, [expected_1, expected_2])
 
@@ -127,69 +130,68 @@
     value_set.url.value = 'vs-url'
 
     coding = value_set.expansion.contains.add()
     coding.code.value = 'code'
 
     table = build_valueset_codes_table()
 
-    result = value_set_tables.valueset_codes_insert_statement_for([value_set],
-                                                                  table)
+    result = value_set_tables.valueset_codes_insert_statement_for(
+        [value_set], table
+    )
     query = list(result)[0]
     query_string = str(query.compile(compile_kwargs={'literal_binds': True}))
     self.assertEqual(
         query_string,
-        ('INSERT INTO valueset_codes '
-         '(valueseturi, valuesetversion, system, code) '
-         'SELECT '
-         'codes.valueseturi, codes.valuesetversion, codes.system, codes.code \n'
-         'FROM (SELECT '
-         "'vs-url' AS valueseturi, "
-         'NULL AS valuesetversion, '
-         'NULL AS system, '
-         "'code' AS code"
-         ') AS codes '
-         'LEFT OUTER JOIN valueset_codes ON '
-         'codes.valueseturi = valueset_codes.valueseturi AND '
-         'codes.valuesetversion = valueset_codes.valuesetversion AND '
-         'codes.system = valueset_codes.system AND '
-         'codes.code = valueset_codes.code \n'
-         'WHERE '
-         'valueset_codes.valueseturi IS NULL AND '
-         'valueset_codes.valuesetversion IS NULL AND '
-         'valueset_codes.system IS NULL AND '
-         'valueset_codes.code IS NULL'))
+        (
+            'INSERT INTO valueset_codes (valueseturi, valuesetversion, system,'
+            ' code) SELECT codes.valueseturi, codes.valuesetversion,'
+            " codes.system, codes.code \nFROM (SELECT 'vs-url' AS valueseturi,"
+            " NULL AS valuesetversion, NULL AS system, 'code' AS code) AS codes"
+            ' LEFT OUTER JOIN valueset_codes ON codes.valueseturi ='
+            ' valueset_codes.valueseturi AND codes.valuesetversion ='
+            ' valueset_codes.valuesetversion AND codes.system ='
+            ' valueset_codes.system AND codes.code = valueset_codes.code'
+            ' \nWHERE valueset_codes.valueseturi IS NULL AND'
+            ' valueset_codes.valuesetversion IS NULL AND valueset_codes.system'
+            ' IS NULL AND valueset_codes.code IS NULL'
+        ),
+    )
 
   def testValueSetToInsertStatement_withBadTable_raisesError(self):
     table = sqlalchemy.table('missing_columns')
     with self.assertRaises(ValueError):
       list(value_set_tables.valueset_codes_insert_statement_for([], table))
 
   def testGeNumCodeSystemsPerValueSet_withQueryResults_returnsCorrectCounts(
-      self):
-    # Construct named tuples to act in the place of SQLAlchemy RowProxy objects.
-    # RowProxy objects are quite similar to named tuples.
-    Row = collections.namedtuple('Row',
-                                 ['valueseturi', 'valuesetversion', 'systems'])
+      self,
+  ):
+    # Construct named tuples to act in the place of SQLAlchemy Row objects.
+    # Row objects are quite similar to named tuples.
+    Row = collections.namedtuple(
+        'Row', ['valueseturi', 'valuesetversion', 'systems']
+    )
     results = [
         Row('http://value.set/1', '1.0', ['a', 'b']),
         Row('http://value.set/1', '2.0', ['b', 'c', 'd']),
         Row('http://value.set/1', None, ['e']),
         Row('http://value.set/2', None, ['d', 'e']),
         Row('http://value.set/3', '1.0', ['f']),
     ]
     counts = value_set_tables._query_results_to_code_system_counts(results)
     self.assertDictEqual(
-        counts, {
+        counts,
+        {
             'http://value.set/1|1.0': 2,
             'http://value.set/1|2.0': 3,
             'http://value.set/1': 5,
             'http://value.set/2': 2,
             'http://value.set/3|1.0': 1,
             'http://value.set/3': 1,
-        })
+        },
+    )
 
 
 def build_valueset_codes_table() -> sqlalchemy.sql.expression.TableClause:
   return sqlalchemy.table(
       'valueset_codes',
       sqlalchemy.column('valueseturi'),
       sqlalchemy.column('valuesetversion'),
```

## Comparing `google_fhir_r4-0.9.2.dist-info/METADATA` & `google_fhir_r4-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: google-fhir-r4
-Version: 0.9.2
+Version: 0.9.3
 Summary: Components for working with FHIR R4.
 Home-page: https://github.com/google/fhir-py
 Download-URL: https://github.com/google-py/fhir/releases
 Author: Google LLC
 Author-email: google-fhir-pypi@google.com
 License: Apache 2.0
 Keywords: google,fhir,python,healthcare
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
-Requires-Dist: google-fhir-core (~=0.9.2)
+Requires-Dist: google-fhir-core (~=0.9.3)
 Requires-Dist: immutabledict (~=2.2)
 Requires-Dist: protobuf (~=3.19)
 Requires-Dist: python-dateutil (~=2.8)
 Requires-Dist: backports.zoneinfo (~=0.2.1) ; python_version < "3.9"
 
 Protocol buffer conversion and validation for with FHIR R4 resources.
```


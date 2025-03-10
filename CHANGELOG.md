## 1.205.0 (Unreleased)
## 1.204.0 (April 28, 2023)

- **New Resource:** `resource_alicloud_config_remediation` ([#6100](https://github.com/aliyun/terraform-provider-alicloud/issues/6100))
- **New Resource:** `alicloud_rds_db_instance_endpoint_address` ([#6090](https://github.com/aliyun/terraform-provider-alicloud/issues/6090))
- **New Resource:** `alicloud_tag_policy_attachment` ([#6071](https://github.com/aliyun/terraform-provider-alicloud/issues/6071))
- **New Resource:** `alicloud_eflo_subnet` ([#6019](https://github.com/aliyun/terraform-provider-alicloud/issues/6019))
- **New Resource:** `alicloud_service_catalog_portfolio` ([#6002](https://github.com/aliyun/terraform-provider-alicloud/issues/6002))
- **New Resource:** `alicloud_arms_remote_write` ([#5998](https://github.com/aliyun/terraform-provider-alicloud/issues/5998))
- **New Datasource:** `alicloud_rds_slots` ([#6075](https://github.com/aliyun/terraform-provider-alicloud/issues/6075))
- **New Datasource:** `alicloud_eflo_subnets` ([#6019](https://github.com/aliyun/terraform-provider-alicloud/issues/6019))
- **New Datasource:** `alicloud_service_catalog_portfolios` ([#6002](https://github.com/aliyun/terraform-provider-alicloud/issues/6002))
- **New Datasource:** `alicloud_arms_remote_writes` ([#5998](https://github.com/aliyun/terraform-provider-alicloud/issues/5998))

ENHANCEMENTS:

- resource/alicloud_resource_manager_resource_group: Added retry strategy for error code DeleteConflict.ResourceGroup.Resource. ([#6109](https://github.com/aliyun/terraform-provider-alicloud/issues/6109))
- resource/alicloud_cen_transit_router: Added retry strategy for error code IncorrectStatus.CenInstance. ([#6108](https://github.com/aliyun/terraform-provider-alicloud/issues/6108))
- resource/alicloud_cen_transit_router_vpc_attachment: Added the field auto_publish_route_enabled. ([#6106](https://github.com/aliyun/terraform-provider-alicloud/issues/6106))
- resource/alicloud_kvstore_instance: Engine version supports 7.0; Adds new attribute effective_time. ([#6104](https://github.com/aliyun/terraform-provider-alicloud/issues/6104))
- ci: Supports to checking the test file. ([#6102](https://github.com/aliyun/terraform-provider-alicloud/issues/6102))
- resource/alicloud_ecs_disk: Improves the deleting disk when it is PrePaid and setting DeleteWithInstance. ([#6099](https://github.com/aliyun/terraform-provider-alicloud/issues/6099))
- resource/alicloud_polardb_cluster: polardb support cluster serverless ([#6098](https://github.com/aliyun/terraform-provider-alicloud/issues/6098))
- resource/alicloud_emrv2_cluster: supported emr cluster data disk encrypted. ([#6097](https://github.com/aliyun/terraform-provider-alicloud/issues/6097))
- ci: Improves the ci and cd feature. ([#6096](https://github.com/aliyun/terraform-provider-alicloud/issues/6096))
- resource/alicloud_config_rule: Adds new attribute compliance,config_rule_arn,event_source etc. ([#6095](https://github.com/aliyun/terraform-provider-alicloud/issues/6095))
- resource/alicloud_cs_kubernetes_addon: Optimize component lifecycle management. ([#6091](https://github.com/aliyun/terraform-provider-alicloud/issues/6091))
- resource/alicloud_tag_policy: Added user_type compute and test fault tolerance. ([#6086](https://github.com/aliyun/terraform-provider-alicloud/issues/6086))
- resource/alicloud_oos_template: Removed the filed content validate limit; Supported content set to yaml value. ([#6085](https://github.com/aliyun/terraform-provider-alicloud/issues/6085))
- ci: Improves the integration test. ([#6084](https://github.com/aliyun/terraform-provider-alicloud/issues/6084))
- Revert "resource/alicloud_oss_bucket_object: Remvoes the server_side_encrypt on argument default value.". ([#6082](https://github.com/aliyun/terraform-provider-alicloud/issues/6082))
- ci: Improves the integration using concourse ci. ([#6080](https://github.com/aliyun/terraform-provider-alicloud/issues/6080))
- resource/alicloud_db_database : character_set are not case sensitive. ([#6008](https://github.com/aliyun/terraform-provider-alicloud/issues/6008))
- resource/alicloud_cen_transit_router_vpc_attachment: Added retry strategy for error code. ([#5949](https://github.com/aliyun/terraform-provider-alicloud/issues/5949))
- datasource/alicloud_instances: Supports filter enable_details and sets its default to true. ([#6107](https://github.com/aliyun/terraform-provider-alicloud/issues/6107))

BUG FIXES:

- resource/alicloud_db_account_privilege : Fix SQLServer account privilege time out bug. ([#6101](https://github.com/aliyun/terraform-provider-alicloud/issues/6101))
- data/alicloud_oss_buckets: Fixed lifecycleRule.Expiration nil bug. ([#6092](https://github.com/aliyun/terraform-provider-alicloud/issues/6092))
- resource/alicloud_resource_manager_account: Fixed abandon_able_check_id invalid error. ([#6055](https://github.com/aliyun/terraform-provider-alicloud/issues/6055))

## 1.203.0 (April 14, 2023)

- **New Resource:** `alicloud_arms_prometheus` ([#5961](https://github.com/aliyun/terraform-provider-alicloud/issues/5961))
- **New Resource:** `alicloud_tag_policy` ([#6057](https://github.com/aliyun/terraform-provider-alicloud/issues/6057))
- **New Resource:** `alicloud_oos_default_patch_baseline` ([#6058](https://github.com/aliyun/terraform-provider-alicloud/issues/6058))
- **New Resource:** `alicloud_ocean_base_instance` ([#6069](https://github.com/aliyun/terraform-provider-alicloud/issues/6069))
- **New Resource:** `alicloud_rds_db_instance_endpoint` ([#6056](https://github.com/aliyun/terraform-provider-alicloud/issues/6056))
- **New Resource** `alicloud_chatbot_publish_task` ([#6014](https://github.com/aliyun/terraform-provider-alicloud/issues/6014))
- **New Resource** `alicloud_arms_integration_exporter` ([#5990](https://github.com/aliyun/terraform-provider-alicloud/issues/5990))
- **New Datasource** `alicloud_arms_integration_exporters` ([#5990](https://github.com/aliyun/terraform-provider-alicloud/issues/5990))
- **New Datasource** `alicloud_chatbot_agents` ([#6014](https://github.com/aliyun/terraform-provider-alicloud/issues/6014))
- **New Datasource:** `alicloud_arms_prometheis` ([#5961](https://github.com/aliyun/terraform-provider-alicloud/issues/5961))
- **New Datasource:** `alicloud_ocean_base_instances` ([#6069](https://github.com/aliyun/terraform-provider-alicloud/issues/6069))

ENHANCEMENTS:

- resource/alicloud_log_alert add attribute template_configuration. ([#6026](https://github.com/aliyun/terraform-provider-alicloud/issues/6026))
- resource/alicloud_oss_bucket: Support ColdArchive storage class. ([#6049](https://github.com/aliyun/terraform-provider-alicloud/issues/6049))
- docs/alicloud_sae_application: Improves the examples.  ([#6051](https://github.com/aliyun/terraform-provider-alicloud/issues/6051))
- resource/alicloud_security_group_rule: Changed the Create SDK to common api to fix the read error caused by ipv6_cidr_ip value. ([#5988](https://github.com/aliyun/terraform-provider-alicloud/issues/5988))
- resource/alicloud_cen_instance_attachment: Added retry stragety for error code IncorrectStatus.VpcRouteTable. ([#6005](https://github.com/aliyun/terraform-provider-alicloud/issues/6005))
- resource/alicloud_ga_endpoint_group: Added retry stragety for error code NotActive.Listener. ([#6004](https://github.com/aliyun/terraform-provider-alicloud/issues/6004))
- doc/index: Optimize endpoints attribute description. ([#6025](https://github.com/aliyun/terraform-provider-alicloud/issues/6025))
- ci: supoorts integration test checking. ([#6041](https://github.com/aliyun/terraform-provider-alicloud/issues/6041))
- docs/db_database, docs/db_instance, docs/db_instance_classes, docs/db_instance_engines, docs/db_instances, docs/db_zones, docs/rds_clone_db_instance, docs/rds_upgrade_db_instance : RDS PPAS engine offline. ([#6017](https://github.com/aliyun/terraform-provider-alicloud/issues/6017))
- ci: Improves the consistency checking. ([#6068](https://github.com/aliyun/terraform-provider-alicloud/issues/6068))
- test: Improves the sweeper test by adding sweepAll function. ([#6073](https://github.com/aliyun/terraform-provider-alicloud/issues/6073))
- ci: Improves the integration test by using pull_request_target. ([#6074](https://github.com/aliyun/terraform-provider-alicloud/issues/6074))
- testcase: Added the resource alicloud_tag_policy region limit. ([#6063](https://github.com/aliyun/terraform-provider-alicloud/issues/6063))
- resource/alicloud_polardb_cluster: polardb support cluster category SENormal. ([#6000](https://github.com/aliyun/terraform-provider-alicloud/issues/6000))
- resource/alicloud_eip_address: Supported isp set to ChinaTelecom, ChinaUnicom, ChinaMobile, ChinaTelecom_L2, ChinaUnicom_L2, ChinaMobile_L2, BGP_FinanceCloud. ([#6076](https://github.com/aliyun/terraform-provider-alicloud/issues/6076))
- resource/alicloud_common_bandwidth_package: Supported isp set to ChinaTelecom, ChinaUnicom, ChinaMobile, ChinaTelecom_L2, ChinaUnicom_L2, ChinaMobile_L2, BGP_FinanceCloud. ([#6078](https://github.com/aliyun/terraform-provider-alicloud/issues/6078))
- resource/alicloud_eip_association: Adds new attribute vpc_id. ([#6065](https://github.com/aliyun/terraform-provider-alicloud/issues/6065))
- datasource/alicloud_instances: Supports the new field instance_name. ([#6077](https://github.com/aliyun/terraform-provider-alicloud/issues/6077))
- resource/alicloud_mongodb_instance: Adds new attribute parameters. ([#6072](https://github.com/aliyun/terraform-provider-alicloud/issues/6072))

BUG FIXES:

- resource/alicloud_nas_access_rule: Fixes the Throttling.User error when reading the resource. ([#6043](https://github.com/aliyun/terraform-provider-alicloud/issues/6043))
- resource/fc_function_async_invoke_config: Fix maximum_retry_attempts cannot be set to 0. ([#6048](https://github.com/aliyun/terraform-provider-alicloud/issues/6048))
- resource/alicloud_mongodb_instance: Fixed ssl_action invalid error. ([#6010](https://github.com/aliyun/terraform-provider-alicloud/issues/6010))
- testcase: Removed the resource cen_transit_route_table_aggregation region limit. ([#6030](https://github.com/aliyun/terraform-provider-alicloud/issues/6030))
- data source/alicloud_ram_users: Fixed the read error caused by filter bug; data source/alicloud_ram_groups: Fixed the read error caused by filter bug. ([#6018](https://github.com/aliyun/terraform-provider-alicloud/issues/6018))
- resource/alicloud_route_entry: Fixed the parse error caused by destination_cidrblock value. ([#6045](https://github.com/aliyun/terraform-provider-alicloud/issues/6045))
- resource/alicloud_nlb_load_balancer_security_group_attachment: Fixed the panic error caused by index out of range. ([#6052](https://github.com/aliyun/terraform-provider-alicloud/issues/6052))
- resource/alicloud_bastionhost_instance: Fixes the bastion host not found error when using intrenational account.  ([#6059](https://github.com/aliyun/terraform-provider-alicloud/issues/6059))
- resource/alicloud_ram_policy: Fixes the nil pointer error when getting policy versions. ([#6064](https://github.com/aliyun/terraform-provider-alicloud/issues/6064))
- docs/alicloud_amqp_instance: Removes the note for no supporting international account. ([#6066](https://github.com/aliyun/terraform-provider-alicloud/issues/6066))
- resource/alicloud_alidns_instance: Fixes the NotApplicable error when operating the resource using international account. ([#6070](https://github.com/aliyun/terraform-provider-alicloud/issues/6070))

## 1.202.0 (March 31, 2023)

- **New Resource:** `alicloud_rds_db_node` ([#6022](https://github.com/aliyun/terraform-provider-alicloud/issues/6022))
- **New Resource:** `alicloud_dbfs_auto_snap_shot_policy` ([#6023](https://github.com/aliyun/terraform-provider-alicloud/issues/6023))
- **New Resource:** `alicloud_cen_transit_route_table_aggregation` ([#5748](https://github.com/aliyun/terraform-provider-alicloud/issues/5748))
- **New Data Source:** `alicloud_cen_transit_route_table_aggregations` ([#5748](https://github.com/aliyun/terraform-provider-alicloud/issues/5748))
- **New Data Source:** `alicloud_dbfs_auto_snap_shot_policies` ([#6023](https://github.com/aliyun/terraform-provider-alicloud/issues/6023))

ENHANCEMENTS:

- resource/alicloud_log_store change max ttl back to 3650 ([#6046](https://github.com/aliyun/terraform-provider-alicloud/issues/6046))
- resource/alicloud_ecs_disk_attachment: Shortens the pending time after creating ([#6042](https://github.com/aliyun/terraform-provider-alicloud/issues/6042))
- resource/alicloud_ecs_disk: Remvoes the waiting after creating ([#6042](https://github.com/aliyun/terraform-provider-alicloud/issues/6042))
- resource/alicloud_hbase_instance: Enlarges the cold_storage_size max value to 100000000 ([#6029](https://github.com/aliyun/terraform-provider-alicloud/issues/6029))
- resource/alicloud_log_store add attribute hot_ttl and mode ([#5923](https://github.com/aliyun/terraform-provider-alicloud/issues/5923))
- resource/alicloud_cen_instance_attachment: Added retry stragety for error code IncorrectStatus.VpcRouteTable ([#6005](https://github.com/aliyun/terraform-provider-alicloud/issues/6005))
- resource/alicloud_rds_account:Add Query Instance Status ([#6013](https://github.com/aliyun/terraform-provider-alicloud/issues/6013))
- resource/alicloud_ga_endpoint_group: Added retry stragety for error code NotActive.Listener ([#6004](https://github.com/aliyun/terraform-provider-alicloud/issues/6004))
- datasource/alicloud_vpn_connections: Supports new output enable_dpd and enable_nat_traversal ([#6020](https://github.com/aliyun/terraform-provider-alicloud/issues/6020))
- ci: Improves the workflows bug when checking the consistency ([#6031](https://github.com/aliyun/terraform-provider-alicloud/issues/6031))
- testcase: Improves the resource alicloud_hbase_instance testcases ([#6034](https://github.com/aliyun/terraform-provider-alicloud/issues/6034))
- testcase: Removed the resource cen_transit_route_table_aggregation region limit ([#6030](https://github.com/aliyun/terraform-provider-alicloud/issues/6030))
- Function Compute supports proxy ([#6038](https://github.com/aliyun/terraform-provider-alicloud/issues/6038))

BUG FIXES:

- resource/alicloud_route_entry: Fixed the parse error caused by destination_cidrblock value ([#6045](https://github.com/aliyun/terraform-provider-alicloud/issues/6045))
- resource/alicloud_mongodb_instance: Fixed ssl_action invalid error ([#6010](https://github.com/aliyun/terraform-provider-alicloud/issues/6010))
- resource/alicloud_security_group_rule: Changed the Create SDK to common api to fix the read error caused by ipv6_cidr_ip value ([#5988](https://github.com/aliyun/terraform-provider-alicloud/issues/5988))
- resource/alicloud_cloud_connect_network_grant: Fixed the panic error caused by cen_uid type ([#6011](https://github.com/aliyun/terraform-provider-alicloud/issues/6011))
- data source/alicloud_ram_users: Fixed the read error caused by filter bug ([#6018](https://github.com/aliyun/terraform-provider-alicloud/issues/6018))
- data source/alicloud_ram_groups: Fixed the read error caused by filter bug ([#6018](https://github.com/aliyun/terraform-provider-alicloud/issues/6018))

## 1.201.2 (March 17, 2023)

BUG FIXES:

- resource/alicloud_nlb_server_group_server_attachment: Add retry error code IncorrectStatus.serverGroup when deleting. ([#5996](https://github.com/aliyun/terraform-provider-alicloud/issues/5996))
- resource/alicloud_db_instance:Fix RDS configuration change error. ([#6001](https://github.com/aliyun/terraform-provider-alicloud/issues/6001))
- resource/alicloud_nlb_server_group: setting the attribute http_check_method to computed, Fix an error with empty http_check_method attribute. ([#6003](https://github.com/aliyun/terraform-provider-alicloud/issues/6003))
- resource/alicloud_ga_bandwidth_package: Added retry stragety for error code BindExist.BandwidthPackage. ([#6006](https://github.com/aliyun/terraform-provider-alicloud/issues/6006))
- docs/db_database, db_instance, db_instances, rds_clone_db_instance : Update documents. ([#6009](https://github.com/aliyun/terraform-provider-alicloud/issues/6009))

## 1.201.1 (March 15, 2023)

BUG FIXES:

- resource/alicloud_vswitch: Repair the panic caused by the ipv6_cidr_block_mask value. ([#5993](https://github.com/aliyun/terraform-provider-alicloud/issues/5993))
- resource/alicloud_emrv2_cluster: Fixes the emr paymentType subscription cluster ([#5978](https://github.com/aliyun/terraform-provider-alicloud/issues/5978))

## 1.201.0 (March 15, 2023)

- **New Resource:** `alicloud_dcdn_er` ([#5934](https://github.com/aliyun/terraform-provider-alicloud/issues/5934))
- **New Resource:** `alicloud_eflo_vpd` ([#5963](https://github.com/aliyun/terraform-provider-alicloud/issues/5963))
- **New Resource:** `alicloud_dcdn_waf_rule` ([#5969](https://github.com/aliyun/terraform-provider-alicloud/issues/5969))
- **New Resource:** `alicloud_actiontrail_global_events_storage_region` ([#5969](https://github.com/aliyun/terraform-provider-alicloud/issues/5969))
- **New Data Source:** `alicloud_actiontrail_global_events_storage_region` ([#5969](https://github.com/aliyun/terraform-provider-alicloud/issues/5969))
- **New Data Source:** `alicloud_dcdn_waf_rules` ([#5969](https://github.com/aliyun/terraform-provider-alicloud/issues/5969))
- **New Data Source:** `alicloud_eflo_vpds` ([#5963](https://github.com/aliyun/terraform-provider-alicloud/issues/5963))

ENHANCEMENTS:

- resource/alicloud_vswitch: Adds new attribute enable_ipv6,ipv6_cidr_block_mask,ipv6_cidr_block ([#5714](https://github.com/aliyun/terraform-provider-alicloud/issues/5714))
- resource/alicloud_havip_attachment: Adds new attribute instance_type ([#5951](https://github.com/aliyun/terraform-provider-alicloud/issues/5951))
- resource/alicloud_resource_manager_resource_directory: Support new attribute member_deletion_status. ([#5985](https://github.com/aliyun/terraform-provider-alicloud/issues/5985))
- resource/alicloud_cen_transit_router_route_table: Added the field tags ([#5982](https://github.com/aliyun/terraform-provider-alicloud/issues/5982))
- resource/alicloud_rds_account:Add error code ([#5979](https://github.com/aliyun/terraform-provider-alicloud/issues/5979))
- resource/alicloud_db_readonly_instance : Read-only instance adaptation pay as you go. ([#5936](https://github.com/aliyun/terraform-provider-alicloud/issues/5936))
- resource/alicloud_drds_instance: Adds new attribute mysql_version ([#5953](https://github.com/aliyun/terraform-provider-alicloud/issues/5953))
- resource/alicloud_instance: Support new attribute dedicated_host_id. ([#5968](https://github.com/aliyun/terraform-provider-alicloud/issues/5968))
- resource/alicloud_db_instance : Update Document. ([#5970](https://github.com/aliyun/terraform-provider-alicloud/issues/5970))
- resource/alicloud_polardb_endpoint: polardb support endpoint db_endpoint_description ([#5964](https://github.com/aliyun/terraform-provider-alicloud/issues/5964))
- resource/alicloud_oos_patch_baseline: Adds the new attribute enumeration value AlmaLinux ([#5959](https://github.com/aliyun/terraform-provider-alicloud/issues/5959))
- resource/alicloud_alikafka_instance: Support new attribute io_max_spec. ([#5966](https://github.com/aliyun/terraform-provider-alicloud/issues/5966))
- docs: Improves the docs example ([#5967](https://github.com/aliyun/terraform-provider-alicloud/issues/5967))
- docs/forward_entry: Improves the docs example ([#5972](https://github.com/aliyun/terraform-provider-alicloud/issues/5972))
- testcase/alicloud_db_readonly_instance : Repair of automation test failure in Germany region ([#5987](https://github.com/aliyun/terraform-provider-alicloud/issues/5987))

BUG FIXES:

- resource/alicloud_instance: Fixes the user data diff error when using base64 encoding ([#5989](https://github.com/aliyun/terraform-provider-alicloud/issues/5989))
- resource/alicloud_cms_site_monitor: Fix English lower case bug. ([#5984](https://github.com/aliyun/terraform-provider-alicloud/issues/5984))
- resource/alicloud_nlb_server_group_server_attachment: fix test case TestAccAlicloudNLBServerGroupServerAttachment_basic0. Add retry error code Conflict.Lock when creating. ([#5980](https://github.com/aliyun/terraform-provider-alicloud/issues/5980))
- resource/alicloud_kvstore_instance: Fixes the InstanceType.NotSupport error when running terraform plan; Fixes the setting auto_renew does not work bug ([#5976](https://github.com/aliyun/terraform-provider-alicloud/issues/5976))
- resource/alicloud_waf_certificate: Fix Test Cases. resource_alicloud_waf_domain: Fix Test Cases. ([#5971](https://github.com/aliyun/terraform-provider-alicloud/issues/5971))
- resource_alicloud_waf_certificate_test: Fix Test Cases. ([#5971](https://github.com/aliyun/terraform-provider-alicloud/issues/5971))
- resource/alicloud_vpc_traffic_mirror_filter: Fix the verification error of traffic_mirror_filter_description and traffic_mirror_filter_name attribute. ([#5958](https://github.com/aliyun/terraform-provider-alicloud/issues/5958))
- resource/alicloud_dms_enterprise_instance: fixed the data_link_name to Computed. ([#5958](https://github.com/aliyun/terraform-provider-alicloud/issues/5958))
- datasource/alicloud_vpc_traffic_mirror_filter_egress_rules: Fix paging query errors. ([#5958](https://github.com/aliyun/terraform-provider-alicloud/issues/5958))
- datasource/alicloud_vpc_traffic_mirror_filter_ingress_rules: Fix paging query errors. ([#5958](https://github.com/aliyun/terraform-provider-alicloud/issues/5958))
- data_source_alicloud_waf_domains: Fix Test Cases. ([#5971](https://github.com/aliyun/terraform-provider-alicloud/issues/5971))
- data_source_alicloud_waf_certificates: Fix Test Cases. ([#5971](https://github.com/aliyun/terraform-provider-alicloud/issues/5971))
- data_source_alicloud_waf_instances: Fix Test Cases. ([#5971](https://github.com/aliyun/terraform-provider-alicloud/issues/5971))


## 1.200.0 (March 03, 2023)

- **New Resource:** `alicloud_wafv3_instance` ([#5919](https://github.com/aliyun/terraform-provider-alicloud/issues/5919))
- **New Resource:** `alicloud_wafv3_domain` ([#5947](https://github.com/aliyun/terraform-provider-alicloud/issues/5947))
- **New Resource:** `alicloud_alb_load_balancer_common_bandwidth_package_attachment` ([#5937](https://github.com/aliyun/terraform-provider-alicloud/issues/5937))
- **New Data Source:** `alicloud_wafv3_domains` ([#5947](https://github.com/aliyun/terraform-provider-alicloud/issues/5947))
- **New Data Source:** `alicloud_wafv3_instances` ([#5919](https://github.com/aliyun/terraform-provider-alicloud/issues/5919))

ENHANCEMENTS:

- resource/alicloud_cms_alarm: Removeed the statistics enums limitation ([#5950](https://github.com/aliyun/terraform-provider-alicloud/issues/5950))
- resource/alicloud_common_bandwidth_package_attachment: Support new attribute cancel_common_bandwidth_package_ip_bandwidth ([#5952](https://github.com/aliyun/terraform-provider-alicloud/issues/5952))
- datasource/alicloud_db_instances : Add query instance detailed information by engine as MariaDB. datasource/alicloud_rds_character_set_names : Add query RDS character set names by engine as MariaDB. ([#5943](https://github.com/aliyun/terraform-provider-alicloud/issues/5943))
- resource/alicloud_db_instance : Create serverless instance and update serverlessConfig params. resource/alicloud_rds_clone_db_instance : Clone serverless instance and update serverlessConfig params. datasource/alicloud_db_zones : Query serverless zones. datasource/alicloud_db_instance_classes : Query serverless instance classes. ([#5911](https://github.com/aliyun/terraform-provider-alicloud/issues/5911))
- resource/alicloud_route_entry: Added retry stragety for error code ([#5939](https://github.com/aliyun/terraform-provider-alicloud/issues/5939))
- resource/alicloud_cen_transit_router_grant_attachment: Added retry stragety for error code ([#5948](https://github.com/aliyun/terraform-provider-alicloud/issues/5948))
- resource/alicloud_kvstore_instance: Adds new attribute tde_status,encryption_name,encryption_key,role_arn ([#5870](https://github.com/aliyun/terraform-provider-alicloud/issues/5870))
- resource/alicloud_vpc_ipv4_gateway: Added retry stragety for error code ([#5938](https://github.com/aliyun/terraform-provider-alicloud/issues/5938))
- resource/alicloud_instance: Support output attribute os_type, os_name, memory, primary_ip_address, cpu. ([#5933](https://github.com/aliyun/terraform-provider-alicloud/issues/5933))
- resource/alicloud_havip_attachment: Added the field force ([#5925](https://github.com/aliyun/terraform-provider-alicloud/issues/5925))
- resource/alicloud_eip_address: Adds new attribute log_project,log_store ([#5917](https://github.com/aliyun/terraform-provider-alicloud/issues/5917))
- resource/alicloud_rds_db_instance_endpoint_address:add engine PostgreSQL ([#5928](https://github.com/aliyun/terraform-provider-alicloud/issues/5928))
- resource/alicloud_ddosbgp_instance: Removed the ForceNew for field period ([#5926](https://github.com/aliyun/terraform-provider-alicloud/issues/5926))
- resource/alicloud_polardb_cluster: polardb support encryption with CMK ([#5924](https://github.com/aliyun/terraform-provider-alicloud/issues/5924))
- docs: Improves the docs example ([#5921](https://github.com/aliyun/terraform-provider-alicloud/issues/5921))
- docs: Improves the docs example and Improves the resource testcases ([#5935](https://github.com/aliyun/terraform-provider-alicloud/issues/5935))
- docs/mhub_app: Improves the docs example ([#5941](https://github.com/aliyun/terraform-provider-alicloud/issues/5941))
- testcase: Modify the ECS instance specifications to support new VPC features ([#5942](https://github.com/aliyun/terraform-provider-alicloud/issues/5942))

BUG FIXES:

- resource/alicloud_lindorm_instance: Fixes the upgrading core_single_storage does not work bug; Enlarges the update default timeout to 180 mins ([#5956](https://github.com/aliyun/terraform-provider-alicloud/issues/5956))
- resource/alicloud_express_connect_router_interface: Fix a bug where the read function filter was not working ([#5954](https://github.com/aliyun/terraform-provider-alicloud/issues/5954))
- resource/alicloud_db_readonly_instance: Fixes the nil pointer error ([#5955](https://github.com/aliyun/terraform-provider-alicloud/issues/5955))
- resource/alicloud_db_instance:Fix the conflict between opening expansion and storage ([#5931](https://github.com/aliyun/terraform-provider-alicloud/issues/5931))
- testcase: Fix test cases for cen. ([#5946](https://github.com/aliyun/terraform-provider-alicloud/issues/5946))

## 1.199.0 (February 21, 2023)

- **New Resource:** `alicloud_threat_detection_instance` ([#5767](https://github.com/aliyun/terraform-provider-alicloud/issues/5767))
- **New Resource:** `alicloud_cr_vpc_endpoint_linked_vpc` ([#5894](https://github.com/aliyun/terraform-provider-alicloud/issues/5894))
- **New Resource:** `alicloud_express_connect_router_interface` ([#5831](https://github.com/aliyun/terraform-provider-alicloud/issues/5831))
- **New Resource:** `alicloud_emrv2_cluster` ([#5892](https://github.com/aliyun/terraform-provider-alicloud/issues/5892))
- **New Data Source:** `alicloud_emrv2_clusters` ([#5892](https://github.com/aliyun/terraform-provider-alicloud/issues/5892))
- **New Data Source:** `alicloud_router_interfaces` ([#5831](https://github.com/aliyun/terraform-provider-alicloud/issues/5831))
- **New Data Source:** `alicloud_threat_detection_instances` ([#5767](https://github.com/aliyun/terraform-provider-alicloud/issues/5767))
- **New Data Source:** `alicloud_cr_vpc_endpoint_linked_vpcs` ([#5894](https://github.com/aliyun/terraform-provider-alicloud/issues/5894))

ENHANCEMENTS:

- provider: Enlarges the session_expiration max value to 43200 ([#5920](https://github.com/aliyun/terraform-provider-alicloud/issues/5920))
- resource/alicloud_emr_cluster_new: Added new resource alicloud_emr_cluster_new which based on EMR's new version openAPI ([#5892](https://github.com/aliyun/terraform-provider-alicloud/issues/5892))
- resource/alicloud_click_house: Removes the validation for attribute db_cluster_class ([#5918](https://github.com/aliyun/terraform-provider-alicloud/issues/5918))
- resource/alicloud_nat_gateway: Added retry stragety for error code IncorrectStatus.NATGW, IncorrectStatus.NatGateway, DependencyViolation.EIPS ([#5916](https://github.com/aliyun/terraform-provider-alicloud/issues/5916))
- resource/alicloud_hbr_server_backup_plan: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5910](https://github.com/aliyun/terraform-provider-alicloud/issues/5910))
- resource/alicloud_cms_event_rule: Optimization type assertion. ([#5908](https://github.com/aliyun/terraform-provider-alicloud/issues/5908))
- resource/alicloud_cen_instance_attachment: Added retry stragety for error code IncorrectStatus.VpcSwitch ([#5903](https://github.com/aliyun/terraform-provider-alicloud/issues/5903))
- resource/alicloud_cen_transit_router_vpc_attachment: Added retry stragety for error code IncorrectStatus.VpcResource ([#5902](https://github.com/aliyun/terraform-provider-alicloud/issues/5902))
- resource/alicloud_bastionhost_instance: Added the field public_white_list; Supported for new action ConfigInstanceWhiteList ([#5890](https://github.com/aliyun/terraform-provider-alicloud/issues/5890))
- resource/alicloud_bastionhost_instance: Support output attribute plan_code ([#5901](https://github.com/aliyun/terraform-provider-alicloud/issues/5901))
- resource/alicloud_mongodb_instance: Support new attribute readonly_replicas, storage_type, hidden_zone_id, secondary_zone_id. ([#5860](https://github.com/aliyun/terraform-provider-alicloud/issues/5860))
- resource/alicloud_ess_scaling_configuration:update by common api & support system_disk_encrypted ([#5873](https://github.com/aliyun/terraform-provider-alicloud/issues/5873))
- resource/alicloud_bastionhost_user: Supported source set to AD and LDAP ([#5888](https://github.com/aliyun/terraform-provider-alicloud/issues/5888))
- doc/dcdn_kv: Optimize content. doc/dcdn_kv_namespace: Optimize content. ([#5886](https://github.com/aliyun/terraform-provider-alicloud/issues/5886))
- doc/nlb_security_policy: Optimize content. ([#5904](https://github.com/aliyun/terraform-provider-alicloud/issues/5904))
- doc/cms_alarm_contact: Optimize content. ([#5908](https://github.com/aliyun/terraform-provider-alicloud/issues/5908))
- doc/cms_metric_rule_black_list: Optimize content. ([#5908](https://github.com/aliyun/terraform-provider-alicloud/issues/5908))
- timeout: Improves the setting timeout when waiting for the resource is ready ([#5913](https://github.com/aliyun/terraform-provider-alicloud/issues/5913))

BUG FIXES:

- resource/alicloud_db_instance: fix rds bug when waiting for the resource is running ([#5909](https://github.com/aliyun/terraform-provider-alicloud/issues/5909))
- resource/alicloud_ram_policy: Fix errors that failed assertions. ([#5898](https://github.com/aliyun/terraform-provider-alicloud/issues/5898))
- resource/alicloud_cms_sls_group: Fix sls_group_config Attribute Reading Defect. ([#5908](https://github.com/aliyun/terraform-provider-alicloud/issues/5908))
- datasource/alicloud_cms_metric_rule_black_lists: Fix paging logic; Fix TestAccAlicloudCmsMetricRuleBlackListsDataSource. ([#5908](https://github.com/aliyun/terraform-provider-alicloud/issues/5908))

## 1.198.0 (February 8, 2023)

- **New Resource:** `alicloud_rds_ddr_db_instance` ([#5794](https://github.com/aliyun/terraform-provider-alicloud/issues/5794))
- **New Resource:** `alicloud_dts_instance` ([#5841](https://github.com/aliyun/terraform-provider-alicloud/issues/5841))
- **New Resource:** `alicloud_nlb_load_balancer_security_group_attachment` ([#5858](https://github.com/aliyun/terraform-provider-alicloud/issues/5858))
- **New Resource:** `alicloud_dcdn_kv_namespace` ([#5859](https://github.com/aliyun/terraform-provider-alicloud/issues/5859))
- **New Resource:** `alicloud_hbr_hana_backup_client` ([#5864](https://github.com/aliyun/terraform-provider-alicloud/issues/5864))
- **New Resource:** `alicloud_dcdn_kv` ([#5865](https://github.com/aliyun/terraform-provider-alicloud/issues/5865))
- **New Resource:** `alicloud_dcdn_kv_account` ([#5867](https://github.com/aliyun/terraform-provider-alicloud/issues/5867))
- **New Data Source:** `data_source_alicloud_rds_collation_time_zones` ([#5837](https://github.com/aliyun/terraform-provider-alicloud/issues/5837))
- **New Data Source:** `alicloud_rds_character_set_names` ([#5838](https://github.com/aliyun/terraform-provider-alicloud/issues/5838))
- **New Data Source:** `alicloud_dts_instances` ([#5841](https://github.com/aliyun/terraform-provider-alicloud/issues/5841))
- **New Data Source:** `alicloud_hbr_hana_backup_clients ` ([#5864](https://github.com/aliyun/terraform-provider-alicloud/issues/5864))

ENHANCEMENTS:

- resource/alicloud_sae_application: Support new attribute micro_registration. ([#5594](https://github.com/aliyun/terraform-provider-alicloud/issues/5594))
- resource/alicloud_rds_account : Resets permissions of the privileged account. ([#5836](https://github.com/aliyun/terraform-provider-alicloud/issues/5836))
- resource/alicloud_cen_transit_router_prefix_list_association: Added retry stragety for error code `ResourceNotFound.PrefixList`, `IncorrectStatus.RouteTable`, `IncorrectStatus.TransitRouter`, `InvalidStatus.Prefixlist`, `InvalidStatus.PrefixlistAssociation` ([#5851](https://github.com/aliyun/terraform-provider-alicloud/issues/5851))
- docs/cen_transit_router_vpn_attachment: Add an example of creating a Transit Router Vpn Attachment with Transit Router Cidr. ([#5853](https://github.com/aliyun/terraform-provider-alicloud/issues/5853))
- docs: Improves the docs missing parameters and incorrect referance. ([#5861](https://github.com/aliyun/terraform-provider-alicloud/issues/5861))
- resource/alicloud_dcdn_domain: Supports new attribute cname. ([#5863](https://github.com/aliyun/terraform-provider-alicloud/issues/5863))
- datasource/alicloud_log_projects add attribute policy. ([#5872](https://github.com/aliyun/terraform-provider-alicloud/issues/5872))
- resource/alicloud_gpdb_elastic_instance: Adds new document description;resource/alicloud_express_connect_physical_connection: Adds new change of attribute peer_location; ([#5877](https://github.com/aliyun/terraform-provider-alicloud/issues/5877))
- resource/alicloud_adb_db_cluster_lake_version: Added the field security_ips and db_cluster_description; Supported for new action ModifyClusterAccessWhiteList and ModifyDBClusterDescription. ([#5879](https://github.com/aliyun/terraform-provider-alicloud/issues/5879))
- supports new region rus-west-1. ([#5881](https://github.com/aliyun/terraform-provider-alicloud/issues/5881))
- resource/alicloud_hbr_hana_backup_client: Added null Update Func. ([#5882](https://github.com/aliyun/terraform-provider-alicloud/issues/5882))

BUG FIXES:

- resource/alicloud_db_instance:fix rds bugs. ([#5862](https://github.com/aliyun/terraform-provider-alicloud/issues/5862))
- resource/alicloud_ecs_launch_template: Fix VersionNumber attribute type error ([#5868](https://github.com/aliyun/terraform-provider-alicloud/issues/5868))
- resource/alicloud_vpc_dhcp_options_set: Fix UpdateDhcpOptionsSetAttribute operation status value verification. ([#5869](https://github.com/aliyun/terraform-provider-alicloud/issues/5869))
- docs: Fixed the title error of alb_listener_acl_attachment and api_gateway_vpc_access ([#5874](https://github.com/aliyun/terraform-provider-alicloud/issues/5874))
- resource/alicloud_event_bridge_rule: Fix the problem that push_retry_strategy does not take effect when creating. ([#5878](https://github.com/aliyun/terraform-provider-alicloud/issues/5878))
- testcase/alicloud_rds_account : Repair of automation test failure in Germany region. ([#5883](https://github.com/aliyun/terraform-provider-alicloud/issues/5883))

## 1.197.0 (January 19, 2023)

- **New Resource:** `alicloud_ga_custom_routing_endpoint_group` ([#5803](https://github.com/aliyun/terraform-provider-alicloud/issues/5803))
- **New Resource:** `alicloud_ga_custom_routing_endpoint_group_destination` ([#5827](https://github.com/aliyun/terraform-provider-alicloud/issues/5827))
- **New Resource:** `alicloud_ga_domain` ([#5830](https://github.com/aliyun/terraform-provider-alicloud/issues/5830))
- **New Resource:** `alicloud_ga_custom_routing_endpoint` ([#5834](https://github.com/aliyun/terraform-provider-alicloud/issues/5834))
- **New Resource:** `alicloud_ga_custom_routing_endpoint_traffic_policy` ([#5840](https://github.com/aliyun/terraform-provider-alicloud/issues/5840))
- **New Data Source:** `alicloud_ga_custom_routing_endpoint_groups` ([#5803](https://github.com/aliyun/terraform-provider-alicloud/issues/5803))
- **New Data Source:** `alicloud_ga_custom_routing_endpoint_group_destinations` ([#5827](https://github.com/aliyun/terraform-provider-alicloud/issues/5827))
- **New Data Source:** `alicloud_ga_domains` ([#5830](https://github.com/aliyun/terraform-provider-alicloud/issues/5830))
- **New Data Source:** `alicloud_service_catalog_end_user_products` ([#5833](https://github.com/aliyun/terraform-provider-alicloud/issues/5833))
- **New Data Source:** `alicloud_ga_custom_routing_endpoints` ([#5834](https://github.com/aliyun/terraform-provider-alicloud/issues/5834))
- **New Data Source:** `alicloud_ga_custom_routing_endpoint_traffic_policies` ([#5840](https://github.com/aliyun/terraform-provider-alicloud/issues/5840))
- **New Data Source:** `alicloud_ga_custom_routing_port_mappings` ([#5842](https://github.com/aliyun/terraform-provider-alicloud/issues/5842))

ENHANCEMENTS:

- resource/alicloud_alikafka_instance: Support to upgrade prepaid instances. ([#5344](https://github.com/aliyun/terraform-provider-alicloud/issues/5344))
- resource/alicloud_cen_transit_router_vpc_attachment: Added retry stragety for error code IncorrectStatus.VpcRouteEntry ([#5820](https://github.com/aliyun/terraform-provider-alicloud/issues/5820))
- resource/alicloud_log_project: Support new attribute policy ([#5826](https://github.com/aliyun/terraform-provider-alicloud/issues/5826))
- resource/alicloud_image: Removes the ValidateFunc for attribute platform to support more valid values ([#5828](https://github.com/aliyun/terraform-provider-alicloud/issues/5828))
- resource/alicloud_image_import: Removes the ValidateFunc for attribute platform to support more valid values ([#5828](https://github.com/aliyun/terraform-provider-alicloud/issues/5828))
- resource/alicloud_elasticsearch_instance: Supports two attribute public_domain and public_port ([#5829](https://github.com/aliyun/terraform-provider-alicloud/issues/5829))
- datasource/alicloud_eventbridge_service: Adds retry policy when checking status is UP ([#5832](https://github.com/aliyun/terraform-provider-alicloud/issues/5832))
- data_source/alicloud_service_catalog_launch_options: Adjust the export root attribute name; ([#5833](https://github.com/aliyun/terraform-provider-alicloud/issues/5833))
- data_source/alicloud_service_catalog_product_as_end_users: Add DEPRECATED identity; ([#5833](https://github.com/aliyun/terraform-provider-alicloud/issues/5833))
- data_source/alicloud_service_catalog_product_versions: Adjust the export root attribute name; ([#5833](https://github.com/aliyun/terraform-provider-alicloud/issues/5833))
- data_source/alicloud_service_catalog_provisioned_products: Adjust the export root attribute name. ([#5833](https://github.com/aliyun/terraform-provider-alicloud/issues/5833))
- resource/alicloud_route_entry: Adds retry for IncorrectStatus.VpcPeer error when creating.  ([#5835](https://github.com/aliyun/terraform-provider-alicloud/issues/5835))
- doc/vswitch: Add an example of creating a cidr switch. ([#5835](https://github.com/aliyun/terraform-provider-alicloud/issues/5835))
- resource/alicloud_route_entry: Added retry strategy for error code IncorrectStatus.VpcPeer,UnknownError ([#5839](https://github.com/aliyun/terraform-provider-alicloud/issues/5839))
- resource/alicloud_ecs_network_interface: Added retry strategy for error code IncorrectVSwitchStatus ([#5839](https://github.com/aliyun/terraform-provider-alicloud/issues/5839))
- resource/alicloud_vpc_peer_connection_accepter: Add retry error code. ([#5843](https://github.com/aliyun/terraform-provider-alicloud/issues/5843))
- resource/alicloud_db_instance: Supports new attribute db_instance_type ([#5846](https://github.com/aliyun/terraform-provider-alicloud/issues/5846))
- resource/alicloud_vpc_peer_connection: Added error code ResourceNotFound.InstanceId ([#5850](https://github.com/aliyun/terraform-provider-alicloud/issues/5850))
- resource/alicloud_nat_gateway: Checking the status to be Available after invoking ModifyNatGatewayAttribute ([#5848](https://github.com/aliyun/terraform-provider-alicloud/issues/5848))

BUG FIXES:

- resource/alicloud_instance: Fixed attribute spot_duration the bug ([#5839](https://github.com/aliyun/terraform-provider-alicloud/issues/5839))
- resource/alicloud_ecs_network_interface: Removes the limitation for private ip count ([#5844](https://github.com/aliyun/terraform-provider-alicloud/issues/5844))
- datasource/alicloud_service_catalog_end_user_products_test: fix test case TestAccAlicloudServiceCatalogEndUserProductDataSource; ([#5845](https://github.com/aliyun/terraform-provider-alicloud/issues/5845))
- resource/alicloud_route_entry_test: fix test case TestAccAlicloudVPCRouteEntryInstance. ([#5845](https://github.com/aliyun/terraform-provider-alicloud/issues/5845))
- docs/ga_custom_routing_endpoint_group_destination: Fixed values of protocols from tcp, udp, tcp, udp to TCP, UDP, TCP, UDP ([#5847](https://github.com/aliyun/terraform-provider-alicloud/issues/5847))

## 1.196.0 (January 11, 2023)

- **New Resource:** `alicloud_vpc_peer_connection_accepter` ([#5786](https://github.com/aliyun/terraform-provider-alicloud/issues/5786))
- **New Resource:** `alicloud_ebs_dedicated_block_storage_cluster` ([#5768](https://github.com/aliyun/terraform-provider-alicloud/issues/5768))
- **New Resource:** `alicloud_ecs_elasticity_assurance` ([#5733](https://github.com/aliyun/terraform-provider-alicloud/issues/5733))
- **New Resource:** `alicloud_service_catalog_provisioned_product` ([#5779](https://github.com/aliyun/terraform-provider-alicloud/issues/5779))
- **New Resource:** `alicloud_express_connect_grant_rule_to_cen` ([#5792](https://github.com/aliyun/terraform-provider-alicloud/issues/5792))
- **New Resource:** `alicloud_express_connect_virtual_physical_connection` ([#5793](https://github.com/aliyun/terraform-provider-alicloud/issues/5793))
- **New Resource:** `alicloud_express_connect_vbr_pconn_association` ([#5784](https://github.com/aliyun/terraform-provider-alicloud/issues/5784))
- **New Resource:** `alicloud_ebs_disk_replica_pair` ([#5758](https://github.com/aliyun/terraform-provider-alicloud/issues/5758))
- **New Data Source:** `alicloud_ebs_disk_replica_pairs` ([#5758](https://github.com/aliyun/terraform-provider-alicloud/issues/5758))
- **New Data Source:** `alicloud_express_connect_vbr_pconn_associations` ([#5784](https://github.com/aliyun/terraform-provider-alicloud/issues/5784))
- **New Data Source:** `alicloud_express_connect_virtual_physical_connections` ([#5793](https://github.com/aliyun/terraform-provider-alicloud/issues/5793))
- **New Data Source:** `alicloud_express_connect_grant_rule_to_cens` ([#5792](https://github.com/aliyun/terraform-provider-alicloud/issues/5792))
- **New Data Source:** `alicloud_ecs_elasticity_assurances` ([#5733](https://github.com/aliyun/terraform-provider-alicloud/issues/5733))
- **New Data Source:** `alicloud_ebs_dedicated_block_storage_clusters` ([#5768](https://github.com/aliyun/terraform-provider-alicloud/issues/5768))
- **New Data Source:** `alicloud_service_catalog_provisioned_products` ([#5779](https://github.com/aliyun/terraform-provider-alicloud/issues/5779))
- **New Data Source:** `alicloud_service_catalog_product_as_end_users` ([#5779](https://github.com/aliyun/terraform-provider-alicloud/issues/5779))
- **New Data Source:** `alicloud_service_catalog_product_versions` ([#5779](https://github.com/aliyun/terraform-provider-alicloud/issues/5779))
- **New Data Source:** `alicloud_service_catalog_launch_options` ([#5779](https://github.com/aliyun/terraform-provider-alicloud/issues/5779))
- **New Data Source:** `alicloud_maxcompute_projects` ([#5783](https://github.com/aliyun/terraform-provider-alicloud/issues/5783))
- **New Data Source:** `alicloud_db_instance_class_infos` ([#5774](https://github.com/aliyun/terraform-provider-alicloud/issues/5774))
- **New Data Source:** `alicloud_rds_cross_region_backups` ([#5762](https://github.com/aliyun/terraform-provider-alicloud/issues/5762))
- **New Data Source:** `alicloud_instance_keywords` ([#5785](https://github.com/aliyun/terraform-provider-alicloud/issues/5785))

ENHANCEMENTS:

- resource/alicloud_ga_listener: Added the field listener_type ([#5815](https://github.com/aliyun/terraform-provider-alicloud/issues/5815))
- resource/alicloud_db_readonly_instance: supports new attributes security_ips, db_instance_ip_array_name, db_instance_ip_array_attribute, security_ip_type and whitelist_network_type ([#5772](https://github.com/aliyun/terraform-provider-alicloud/issues/5772))
- resource/alicloud_gpdb_instance: Add new attributes connection_string and port ([#5812](https://github.com/aliyun/terraform-provider-alicloud/issues/5812))
- resource/alicloud_graph_database_db_instance: Adds retry for IncorrectDBInstanceState error when updating ([#5810](https://github.com/aliyun/terraform-provider-alicloud/issues/5810))
- resource/alicloud_polardb_cluster: Add new attributes connection_string and port  size/L ([#5808](https://github.com/aliyun/terraform-provider-alicloud/issues/5808))
- resource/alicloud_graph_database_db_instance: Add new attributes connection_string and port ([#5807](https://github.com/aliyun/terraform-provider-alicloud/issues/5807))
- resource/alicloud_drds_instance: Add new attributes connection_string and port ([#5806](https://github.com/aliyun/terraform-provider-alicloud/issues/5806))
- resource/alicloud_click_house_db_cluster: Add new attributes connection_string and port ([#5805](https://github.com/aliyun/terraform-provider-alicloud/issues/5805))
- resource/alicloud_adb_db_cluster：Add new attribute port ([#5802](https://github.com/aliyun/terraform-provider-alicloud/issues/5802))
- resource/alicloud_slb_load_balancer: Supports valid value locked for attribute status ([#5798](https://github.com/aliyun/terraform-provider-alicloud/issues/5798))
- resource/alicloud_oos_patch_baseline: Update attribute operation_system valid value Centos to CentOS ([#5797](https://github.com/aliyun/terraform-provider-alicloud/issues/5797))
- resource/alicloud_image: Supports image platform 'Windows Server 2022' ([#5796](https://github.com/aliyun/terraform-provider-alicloud/issues/5796))
- resource/alicloud_lindorm_instance: Adds new attribute service_type ([#5790](https://github.com/aliyun/terraform-provider-alicloud/issues/5790))
- resource/alicloud_maxcompute_project: Upgrade to a new version of OpenAPI ([#5783](https://github.com/aliyun/terraform-provider-alicloud/issues/5783))
- resource/alicloud_cen_transit_router_route_entry: Added retry stragety for error code InstanceStatus.NotSupport ([#5787](https://github.com/aliyun/terraform-provider-alicloud/issues/5787))
- resource/alicloud_instance,alicloud_ecs_instance_set,alicloud_ecs_disk: Supports valid value cloud_auto for attribute category ([#5789](https://github.com/aliyun/terraform-provider-alicloud/issues/5789))
- resource/alicloud_db_instance: Removes the validateFunc for attribute connection_string_prefix ([#5788](https://github.com/aliyun/terraform-provider-alicloud/issues/5788))
- resource/alicloud_edas_k8s_slb_attachment: allowes user to specify attribute slb_id ([#5771](https://github.com/aliyun/terraform-provider-alicloud/issues/5771))
- datasource/alicloud_event_bridge_service: Adds double checking for status by GetEventBridgeStatus ([#5799](https://github.com/aliyun/terraform-provider-alicloud/issues/5799))
- datasource/alicloud_db_instance_class_infos: Repair of automation test failure in Germany region ([#5811](https://github.com/aliyun/terraform-provider-alicloud/issues/5811))
- test: Improves the testing framework to support setting non-string value and additional attributes ([#5777](https://github.com/aliyun/terraform-provider-alicloud/issues/5777))
- docs/cen_transit_router_vpn_attachment: Improves the content ([#5814](https://github.com/aliyun/terraform-provider-alicloud/issues/5814))
- ci: update ci pipeline ([#5776](https://github.com/aliyun/terraform-provider-alicloud/issues/5776))

BUG FIXES:

- resource/alicloud_db_instance: Fixes the InvalidStorage.Malformed error when updating the db_instance_storage_type ([#5817](https://github.com/aliyun/terraform-provider-alicloud/issues/5817))
- resource/alicloud_image_import: Fixes the Creating broken error when waiting the resource is available ([#5800](https://github.com/aliyun/terraform-provider-alicloud/issues/5800))
- resource/alicloud_vpc_ipv4_gateway: Fixes the EnableVpcIpv4Gateway error when creating the resource([#5790](https://github.com/aliyun/terraform-provider-alicloud/issues/5790))
- resource/alicloud_vpc_prefix_list: Added the field status; Fixed the create error caused by state refresh ([#5780](https://github.com/aliyun/terraform-provider-alicloud/issues/5780))
- resource/alicloud_ots_instance: Fixes the 10min slow return of ValidationFailed for ots instance delete. ([#5782](https://github.com/aliyun/terraform-provider-alicloud/issues/5782))
- resource/alicloud_graph_database_db_instance: Fixes the IncorrectDBInstanceState when ModifyDBInstanceAccessWhiteList ([#5778](https://github.com/aliyun/terraform-provider-alicloud/issues/5778))
- datasource/alicloud_event_bridge_service: Fixes the waiting status ([#5819](https://github.com/aliyun/terraform-provider-alicloud/issues/5819))
- docs/alicloud_alb_ascript: fix subcategory ([#5781](https://github.com/aliyun/terraform-provider-alicloud/issues/5781))
- docs: fix link; changeLog: Optimize content. ([#5809](https://github.com/aliyun/terraform-provider-alicloud/issues/5809))
- doc/slb_load_balancer: fix content. ([#5813](https://github.com/aliyun/terraform-provider-alicloud/issues/5813))
- testcase: Improves the resource oos_patch_baseline testcases ([#5801](https://github.com/aliyun/terraform-provider-alicloud/issues/5801))

## 1.195.0 (December 30, 2022)

- **New Resource:** `alicloud_rds_instance_cross_backup_policy` ([#5701](https://github.com/aliyun/terraform-provider-alicloud/issues/5701))
- **New Resource:** `alicloud_threat_detection_web_lock_config` ([#5709](https://github.com/aliyun/terraform-provider-alicloud/issues/5709))
- **New Resource:** `alicloud_dms_enterprise_proxy_access` ([#5732](https://github.com/aliyun/terraform-provider-alicloud/issues/5732))
- **New Resource:** `alicloud_dms_enterprise_logic_database` ([#5736](https://github.com/aliyun/terraform-provider-alicloud/issues/5736))
- **New Resource:** `alicloud_amqp_static_account` ([#5721](https://github.com/aliyun/terraform-provider-alicloud/issues/5721))
- **New Resource:** `alicloud_adb_resource_group` ([#5724](https://github.com/aliyun/terraform-provider-alicloud/issues/5724))
- **New Resource:** `alicloud_threat_detection_vul_whitelist` ([#5711](https://github.com/aliyun/terraform-provider-alicloud/issues/5711))
- **New Resource:** `alicloud_threat_detection_backup_policy` ([#5684](https://github.com/aliyun/terraform-provider-alicloud/issues/5684))
- **New Resource:** `alicloud_alb_ascript` ([#5749](https://github.com/aliyun/terraform-provider-alicloud/issues/5749))
- **New Resource:** `alicloud_threat_detection_honeypot_node` ([#5738](https://github.com/aliyun/terraform-provider-alicloud/issues/5738))
- **New Resource:** `alicloud_cen_transit_router_multicast_domain` ([#5735](https://github.com/aliyun/terraform-provider-alicloud/issues/5735))
- **New Resource:** `alicloud_cen_inter_region_traffic_qos_policy` ([#5750](https://github.com/aliyun/terraform-provider-alicloud/issues/5750))
- **New Resource:** `alicloud_threat_detection_baseline_strategy` ([#5743](https://github.com/aliyun/terraform-provider-alicloud/issues/5743))
- **New Resource:** `alicloud_threat_detection_anti_brute_force_rule` ([#5744](https://github.com/aliyun/terraform-provider-alicloud/issues/5744))
- **New Resource:** `alicloud_threat_detection_honey_pot` ([#5739](https://github.com/aliyun/terraform-provider-alicloud/issues/5739))
- **New Resource:** `alicloud_threat_detection_honeypot_probe` ([#5742](https://github.com/aliyun/terraform-provider-alicloud/issues/5742))
- **New Resource:** `alicloud_ecs_capacity_reservation` ([#5667](https://github.com/aliyun/terraform-provider-alicloud/issues/5667))
- **New Resource:** `alicloud_cen_transit_router_multicast_domain_peer_member` ([#5745](https://github.com/aliyun/terraform-provider-alicloud/issues/5745))
- **New Resource:** `alicloud_cen_transit_router_multicast_domain_member` ([#5756](https://github.com/aliyun/terraform-provider-alicloud/issues/5756))
- **New Resource:** `alicloud_cen_inter_region_traffic_qos_queue` ([#5761](https://github.com/aliyun/terraform-provider-alicloud/issues/5761))
- **New Resource:** `alicloud_cen_child_instance_route_entry_to_attachment` ([#5731](https://github.com/aliyun/terraform-provider-alicloud/issues/5731))
- **New Resource:** `alicloud_cen_transit_router_multicast_domain_association` ([#5759](https://github.com/aliyun/terraform-provider-alicloud/issues/5759))
- **New Resource:** `alicloud_threat_detection_honeypot_preset` ([#5753](https://github.com/aliyun/terraform-provider-alicloud/issues/5753))
- **New Resource:** `alicloud_cen_transit_router_multicast_domain_source` ([#5751](https://github.com/aliyun/terraform-provider-alicloud/issues/5751))
- **New Data Source:** `alicloud_bss_openapi_products` ([#5769](https://github.com/aliyun/terraform-provider-alicloud/issues/5769))
- **New Data Source:** `alicloud_bss_openapi_pricing_modules` ([#5769](https://github.com/aliyun/terraform-provider-alicloud/issues/5769))
- **New Data Source:** `alicloud_cen_transit_router_multicast_domain_sources` ([#5751](https://github.com/aliyun/terraform-provider-alicloud/issues/5751))
- **New Data Source:** `alicloud_threat_detection_honeypot_presets` ([#5753](https://github.com/aliyun/terraform-provider-alicloud/issues/5753))
- **New Data Source:** `alicloud_cen_transit_router_multicast_domain_associations` ([#5759](https://github.com/aliyun/terraform-provider-alicloud/issues/5759))
- **New Data Source:** `alicloud_cen_child_instance_route_entry_to_attachments` ([#5731](https://github.com/aliyun/terraform-provider-alicloud/issues/5731))
- **New Data Source:** `alicloud_cen_inter_region_traffic_qos_queues` ([#5761](https://github.com/aliyun/terraform-provider-alicloud/issues/5761))
- **New Data Source:** `alicloud_cen_transit_router_multicast_domain_members` ([#5756](https://github.com/aliyun/terraform-provider-alicloud/issues/5756))
- **New Data Source:** `alicloud_cen_transit_router_multicast_domain_peer_members` ([#5745](https://github.com/aliyun/terraform-provider-alicloud/issues/5745))
- **New Data Source:** `alicloud_ecs_capacity_reservations` ([#5667](https://github.com/aliyun/terraform-provider-alicloud/issues/5667))
- **New Data Source:** `alicloud_threat_detection_honeypot_probes` ([#5742](https://github.com/aliyun/terraform-provider-alicloud/issues/5742))
- **New Data Source:** `alicloud_threat_detection_anti_brute_force_rules` ([#5744](https://github.com/aliyun/terraform-provider-alicloud/issues/5744))
- **New Data Source:** `alicloud_threat_detection_honey_pots` ([#5739](https://github.com/aliyun/terraform-provider-alicloud/issues/5739))
- **New Data Source:** `alicloud_threat_detection_baseline_strategies` ([#5743](https://github.com/aliyun/terraform-provider-alicloud/issues/5743))
- **New Data Source:** `alicloud_cen_inter_region_traffic_qos_policies` ([#5750](https://github.com/aliyun/terraform-provider-alicloud/issues/5750))
- **New Data Source:** `alicloud_cen_transit_router_multicast_domains` ([#5735](https://github.com/aliyun/terraform-provider-alicloud/issues/5735))
- **New Data Source:** `alicloud_threat_detection_honeypot_nodes` ([#5738](https://github.com/aliyun/terraform-provider-alicloud/issues/5738))
- **New Data Source:** `alicloud_alb_ascripts` ([#5749](https://github.com/aliyun/terraform-provider-alicloud/issues/5749))
- **New Data Source:** `alicloud_threat_detection_backup_policies` ([#5684](https://github.com/aliyun/terraform-provider-alicloud/issues/5684))
- **New Data Source:** `alicloud_threat_detection_vul_whitelists` ([#5711](https://github.com/aliyun/terraform-provider-alicloud/issues/5711))
- **New Data Source:** `alicloud_adb_resource_groups` ([#5724](https://github.com/aliyun/terraform-provider-alicloud/issues/5724))
- **New Data Source:** `alicloud_amqp_static_accounts` ([#5721](https://github.com/aliyun/terraform-provider-alicloud/issues/5721))
- **New Data Source:** `alicloud_dms_enterprise_logic_databases` ([#5736](https://github.com/aliyun/terraform-provider-alicloud/issues/5736))
- **New Data Source:** `alicloud_dms_enterprise_databases` ([#5736](https://github.com/aliyun/terraform-provider-alicloud/issues/5736))
- **New Data Source:** `alicloud_dms_enterprise_proxy_accesses` ([#5732](https://github.com/aliyun/terraform-provider-alicloud/issues/5732))
- **New Data Source:** `alicloud_threat_detection_web_lock_configs` ([#5709](https://github.com/aliyun/terraform-provider-alicloud/issues/5709))
- **New Data Source:** `alicloud_threat_detection_assets` ([#5757](https://github.com/aliyun/terraform-provider-alicloud/issues/5757))
- **New Data Source:** `alicloud_threat_detection_log_shipper` ([#5730](https://github.com/aliyun/terraform-provider-alicloud/issues/5730))
- **New Data Source:** `alicloud_threat_detection_honeypot_images` ([#5739](https://github.com/aliyun/terraform-provider-alicloud/issues/5739))

ENHANCEMENTS:

- resource/alicloud_cen_child_instance_route_entry_to_attachment: Repair the error reported by CI test ([#5766](https://github.com/aliyun/terraform-provider-alicloud/issues/5766))
- resource/alicloud_db_readwrite_splitting_connection : Repair of automation test failure in Germany region ([#5765](https://github.com/aliyun/terraform-provider-alicloud/issues/5765))
- resource/alicloud_instance: Adds new valid value Not-applicable for attribute stopped_mode ([#5760](https://github.com/aliyun/terraform-provider-alicloud/issues/5760))
- resource/alicloud_db_readwrite_splitting_connection : Repair create SQL Server read write splitting connection fail bug ([#5734](https://github.com/aliyun/terraform-provider-alicloud/issues/5734))
- resource/alicloud_alikafka_instance: Support new attribute selected_zones. ([#5752](https://github.com/aliyun/terraform-provider-alicloud/issues/5752))
- resource/alicloud_cen_transit_router: Added the field support_multicast ([#5737](https://github.com/aliyun/terraform-provider-alicloud/issues/5737))
- resource/alicloud_vpc_prefix_list: Added retry stragety for error code LastTokenProcessing, OperationFailed.LastTokenProcessing, DependencyViolation.ShareResource, IncorrectStatus.PrefixList, IncorrectStatus.SystemPrefixList, IncorrectStatus.%s ([#5710](https://github.com/aliyun/terraform-provider-alicloud/issues/5710))
- ci: Upgrades the go version to 1.18.9 ([#5741](https://github.com/aliyun/terraform-provider-alicloud/issues/5741))

BUG FIXES:

- resource/alicloud_slb_load_balancer: Fixes the ShareSlbHaltSales error when creating PayByCLUC balancer ([#5770](https://github.com/aliyun/terraform-provider-alicloud/issues/5770))
- resource/alicloud_slb_server_group_server_attachment: Fixes the ServiceIsConfiguring error when creating the resource ([#5755](https://github.com/aliyun/terraform-provider-alicloud/issues/5755))
- resource/alicloud_ess_eci_scaling_configuration: fix default integer value of livenessProbe and readinessProbe. ([#5727](https://github.com/aliyun/terraform-provider-alicloud/issues/5727))
- resource/alicloud_slb_rule: Fixes the ServiceIsConfiguring error when creating the resource ([#5740](https://github.com/aliyun/terraform-provider-alicloud/issues/5740))
- resource/alicloud_threat_detection_backup_policy: fix test case TestAccAlicloudThreatDetectionBackupPolicy_basic0 ([#5764](https://github.com/aliyun/terraform-provider-alicloud/issues/5764))
- resource/alicloud_threat_detection_web_lock_config: fix test case TestAccAlicloudThreatDetectionWebLockConfig_basic1875 ([#5764](https://github.com/aliyun/terraform-provider-alicloud/issues/5764))

## 1.194.1 (December 22, 2022)

ENHANCEMENTS:

- resource/alicloud_lindorm_instance: Removes the some attributes' enums limitation ([#5729](https://github.com/aliyun/terraform-provider-alicloud/issues/5729))
- resource/alicloud_cen_bandwidth_package: Document adding attribute description ([#5722](https://github.com/aliyun/terraform-provider-alicloud/issues/5722))
- resource/alicloud_resource_manager_shared_resource: The resource_type attribute supports the option of PublicIpAddressPool. ([#5720](https://github.com/aliyun/terraform-provider-alicloud/issues/5720))
- resource/alicloud_cen_transit_router_vpn_attachment: Added retry stragety for error code OperationFailed.AllocateCidrFailed ([#5713](https://github.com/aliyun/terraform-provider-alicloud/issues/5713))
- resource/alicloud_alb_server_group: Removes the attribute servers Computed setting ([#5718](https://github.com/aliyun/terraform-provider-alicloud/issues/5718))
- resource/alicloud_express_connect_virtual_border_router: setting the attribute bandwidth to computed ([#5715](https://github.com/aliyun/terraform-provider-alicloud/issues/5715))
- resource/alicloud_resource_manager_account: Improves the deleting action by setting deleting to success stauts ([#5708](https://github.com/aliyun/terraform-provider-alicloud/issues/5708))
- resource/alicloud_eip_association: Added retry stragety for error code TaskConflict, OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, IncorrectEipStatus, InvalidBindingStatus, IncorrectInstanceStatus, IncorrectHaVipStatus, IncorrectStatus.NatGateway, IncorrectStatus.ResourceStatus, InvalidStatus.EcsStatusNotSupport, InvalidStatus.InstanceHasBandWidth, InvalidStatus.EniStatusNotSupport, InvalidIpStatus.HasBeenUsedBySnatTable, InvalidIpStatus.HasBeenUsedByForwardEntry, InvalidStatus.EniStatusNotSupport, InvalidStatus.EcsStatusNotSupport, InvalidStatus.NotAllow, InvalidStatus.SnatOrDnat, FrequentPurchase.EIP ([#5694](https://github.com/aliyun/terraform-provider-alicloud/issues/5694))
- data_source/alicloud_vpn_connections: Support new attribute vco_health_check, vpn_bgp_config ([#5728](https://github.com/aliyun/terraform-provider-alicloud/issues/5728))
- data_source/alicloud_vpn_gateways: Support new attribute auto_propagate ([#5728](https://github.com/aliyun/terraform-provider-alicloud/issues/5728))
- testcase: supports to set more args when invoking the Get method ([#5726](https://github.com/aliyun/terraform-provider-alicloud/issues/5726))

BUG FIXES:

- resource/alicloud_cloud_firewall_instance: Fixed the import error caused by ProductCode, ProductType incorrect value ([#5725](https://github.com/aliyun/terraform-provider-alicloud/issues/5725))
- resource/alicloud_eci_container_group: Fixed word spelling bugs ([#5719](https://github.com/aliyun/terraform-provider-alicloud/issues/5719))
- resource/alicloud_slb_load_balancer: Fixes the attribute instance_charge_type diff error ([#5717](https://github.com/aliyun/terraform-provider-alicloud/issues/5717))
- resource/alicloud_dcdn_domain: Fixes the CertName.MissingParameter error when updating the certificate ([#5716](https://github.com/aliyun/terraform-provider-alicloud/issues/5716))
- resource/alicloud_lindorm_instance: Fixes the instance_storage and core_spec diff error when using multi-zone; Removes the ForceNew tag for arch_version ([#5712](https://github.com/aliyun/terraform-provider-alicloud/issues/5712))
- datasource/alicloud_vpn_gateways: Fixes the nil pointer error when setting end_time ([#5707](https://github.com/aliyun/terraform-provider-alicloud/issues/5707))
- data_source/alicloud_vpn_gateways: Fixed word spelling bugs ([#5728](https://github.com/aliyun/terraform-provider-alicloud/issues/5728))

## 1.194.0 (December 12, 2022)

- **New Resource:** `alicloud_vpc_gateway_route_table_attachment` ([#5646](https://github.com/aliyun/terraform-provider-alicloud/issues/5646))
- **New Resource:** `alicloud_ga_basic_endpoint_group` ([#5609](https://github.com/aliyun/terraform-provider-alicloud/issues/5609))
- **New Resource:** `alicloud_cms_metric_rule_black_list` ([#5670](https://github.com/aliyun/terraform-provider-alicloud/issues/5670))
- **New Resource:** `alicloud_ga_basic_ip_set` ([#5626](https://github.com/aliyun/terraform-provider-alicloud/issues/5626))
- **New Resource:** `alicloud_cloud_firewall_vpc_firewall_cen` ([#5678](https://github.com/aliyun/terraform-provider-alicloud/issues/5678))
- **New Resource:** `alicloud_cloud_firewall_vpc_firewall` ([#5668](https://github.com/aliyun/terraform-provider-alicloud/issues/5668))
- **New Resource:** `alicloud_cloud_firewall_instance_member` ([#5677](https://github.com/aliyun/terraform-provider-alicloud/issues/5677))
- **New Resource:** `alicloud_ga_basic_accelerate_ip` ([#5634](https://github.com/aliyun/terraform-provider-alicloud/issues/5634))
- **New Resource:** `alicloud_ga_basic_endpoint` ([#5676](https://github.com/aliyun/terraform-provider-alicloud/issues/5676))
- **New Resource:** `alicloud_cloud_firewall_vpc_firewall_control_policy` ([#5683](https://github.com/aliyun/terraform-provider-alicloud/issues/5683))
- **New Resource:** `alicloud_ga_basic_accelerate_ip_endpoint_relation` ([#5680](https://github.com/aliyun/terraform-provider-alicloud/issues/5680))
- **New Data Source:** `alicloud_ga_basic_accelerate_ip_endpoint_relationsENHANCEMENTS` ([#5680](https://github.com/aliyun/terraform-provider-alicloud/issues/5680))
- **New Data Source:** `alicloud_cloud_firewall_vpc_firewall_control_policies` ([#5683](https://github.com/aliyun/terraform-provider-alicloud/issues/5683))
- **New Data Source:** `alicloud_ga_basic_endpoints` ([#5676](https://github.com/aliyun/terraform-provider-alicloud/issues/5676))
- **New Data Source:** `alicloud_ga_basic_accelerate_ips` ([#5634](https://github.com/aliyun/terraform-provider-alicloud/issues/5634))
- **New Data Source:** `alicloud_cloud_firewall_instance_members` ([#5677](https://github.com/aliyun/terraform-provider-alicloud/issues/5677))
- **New Data Source:** `alicloud_cloud_firewall_vpc_firewalls` ([#5668](https://github.com/aliyun/terraform-provider-alicloud/issues/5668))
- **New Data Source:** `alicloud_cloud_firewall_vpc_firewall_cens` ([#5678](https://github.com/aliyun/terraform-provider-alicloud/issues/5678))
- **New Data Source:** `alicloud_cms_metric_rule_black_lists` ([#5670](https://github.com/aliyun/terraform-provider-alicloud/issues/5670))

ENHANCEMENTS:

- resource/alicloud_slb_listener: Added retry strategy for error code OperationFailed.ListenerStatusNotSupport. ([#5705](https://github.com/aliyun/terraform-provider-alicloud/issues/5705))
- resource/alicloud_lindorm_instance: Fixes the instance_storage parsing bug when upgrading its value ([#5702](https://github.com/aliyun/terraform-provider-alicloud/issues/5702))
- resource/alicloud_alb_server_group: Support new attribute remote_ip_enabled; Add optional Ip and Fc for server_type ([#5645](https://github.com/aliyun/terraform-provider-alicloud/issues/5645))
- resource/alicloud_vpc_traffic_mirror_filter_ingress_rule: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, OperationFailed.LastTokenProcessing, IncorrectStatus.TrafficMirrorSession, IncorrectStatus.TrafficMirrorFilter, IncorrectStatus.TrafficMirrorRule ([#5699](https://github.com/aliyun/terraform-provider-alicloud/issues/5699))
- resource/alicloud_vpc_traffic_mirror_filter_egress_rule: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, OperationFailed.LastTokenProcessing, IncorrectStatus.TrafficMirrorSession, IncorrectStatus.TrafficMirrorFilter, IncorrectStatus.TrafficMirrorRule ([#5698](https://github.com/aliyun/terraform-provider-alicloud/issues/5698))
- resource/alicloud_slb_load_balancer: Remove the ConflictsWith setting from attribute payment_type;resource/alicloud_vpn_gateway_vpn_attachment: Update document information;resource/alicloud_vpn_gateway: Update document information; ([#5674](https://github.com/aliyun/terraform-provider-alicloud/issues/5674))
- resource/alicloud_vpc_traffic_mirror_filter: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy ([#5697](https://github.com/aliyun/terraform-provider-alicloud/issues/5697))
- resource/alicloud_havip_attachment: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, OperationFailed.LastTokenProcessing, IncorrectHaVipStatus, IncorrectInstanceStatus ([#5696](https://github.com/aliyun/terraform-provider-alicloud/issues/5696))
- resource/alicloud_havip: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, IncorrectStatus ([#5695](https://github.com/aliyun/terraform-provider-alicloud/issues/5695))
- resource/alicloud_eip_address: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, IncorrectEipStatus, IncorrectStatus.ResourceStatus, FrequentPurchase.EIP ([#5692](https://github.com/aliyun/terraform-provider-alicloud/issues/5692))
- resource/alicloud_common_bandwidth_package: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, BandwidthPackageOperation.conflict ([#5690](https://github.com/aliyun/terraform-provider-alicloud/issues/5690))
- resource/alicloud_vpc_traffic_mirror_session: Added retry stragety for error code OperationConflict, IncorrectStatus.%s, ServiceUnavailable, SystemBusy, LastTokenProcessing, OperationFailed.LastTokenProcessing, IncorrectStatus.TrafficMirrorSession, IncorrectStatus.TrafficMirrorFilter ([#5653](https://github.com/aliyun/terraform-provider-alicloud/issues/5653))
- resource/alicloud_common_bandwidth_package_attachment: Added the field bandwidth_package_bandwidth; Supported for new action ModifyCommonBandwidthPackageIpBandwidth ([#5691](https://github.com/aliyun/terraform-provider-alicloud/issues/5691))
- resource/alicloud_nat_gateway: Removed the ForceNew for field eip_bind_mode, supports modifying them online ([#5693](https://github.com/aliyun/terraform-provider-alicloud/issues/5693))
- resource_alicloud_vpn_gateway_vco_route: Add retry error code. resource_alicloud_vpn_connection: Add retry error code. resource_alicloud_vpn_pbr_route_entry: Add retry error code. resource_alicloud_vpn_route_entry: Add retry error code. ([#5689](https://github.com/aliyun/terraform-provider-alicloud/issues/5689))
- resource/alicloud_cloud_firewall_vpc_firewall_cen: Field vpc_region add ForceNew setting and add constraints to the test. ([#5687](https://github.com/aliyun/terraform-provider-alicloud/issues/5687))
- resource_alicloud_security_group_rule: The 'ForceNew' attribute of input parameter 'prefix_list_id' is set 'True' ([#5593](https://github.com/aliyun/terraform-provider-alicloud/issues/5593))
- resource/alicloud_reserved_instance: Support new attribute auto_renew, auto_renew_period, tags, reserved_instance_name. Supports new output allocation_status, create_time, expired_time, operation_locks, start_time, status. ([#5618](https://github.com/aliyun/terraform-provider-alicloud/issues/5618))
- resource/alicloud_alikafka_instance: add double checking when deleting the resource; Improves the testcases ([#5682](https://github.com/aliyun/terraform-provider-alicloud/issues/5682))
- resource/alicloud_db_backup_policy:support RDS configure backup frequency ([#5672](https://github.com/aliyun/terraform-provider-alicloud/issues/5672))
- resource/alicloud_alikafka_instance: Adds new attribute parition_num and deprecate topic_quota; Adds API DeleteInstance to delete the resource ([#5681](https://github.com/aliyun/terraform-provider-alicloud/issues/5681))
- docs: normalize the resource subcategory ([#5688](https://github.com/aliyun/terraform-provider-alicloud/issues/5688))

BUG FIXES:

- resource/alicloud_alb_rule: Fix errors when the weight attribute is not configured. ([#5706](https://github.com/aliyun/terraform-provider-alicloud/issues/5706))
- resource/alicloud_lindorm_instance: Fixes the MissingUpgradeType error when updating the resource ([#5704](https://github.com/aliyun/terraform-provider-alicloud/issues/5704))
- resource/alicloud_resource_manager_account: Fixes the deleting account can not work bug ([#5686](https://github.com/aliyun/terraform-provider-alicloud/issues/5686))
- resource/alicloud_alb_rule: Fix errors when the weight attribute is not configured. ([#5644](https://github.com/aliyun/terraform-provider-alicloud/issues/5644))
- testcase: Fixes the resource alicloud_alikafka_instance testcase error ([#5700](https://github.com/aliyun/terraform-provider-alicloud/issues/5700))
- testcase: fix resource alicloud_db_backup_policy testcase bug ([#5679](https://github.com/aliyun/terraform-provider-alicloud/issues/5679))

## 1.193.1 (December 06, 2022)

ENHANCEMENTS:

- resource/alicloud_ess_eci_scalingconfiguration: Add acr_registry_infos and container liveness_probe, readiness_probe. ([#5666](https://github.com/aliyun/terraform-provider-alicloud/issues/5666))
- resource/alicloud_cen_transit_router_vbr_attachment: Added the field tags ([#5662](https://github.com/aliyun/terraform-provider-alicloud/issues/5662))
- resource/alicloud_cen_transit_router_vpn_attachment: Added the field tags ([#5663](https://github.com/aliyun/terraform-provider-alicloud/issues/5663))
- resource/alicloud_cen_transit_router: Added the field tags ([#5640](https://github.com/aliyun/terraform-provider-alicloud/issues/5640))
- resource/alicloud_vpn_connection: Add retry error code. ([#5657](https://github.com/aliyun/terraform-provider-alicloud/issues/5657))
- resource/alicloud_alb_load_balancer: Removed the ForceNew for field address_type, supports modifying them online; Supported for new action UpdateLoadBalancerAddressTypeConfig ([#5648](https://github.com/aliyun/terraform-provider-alicloud/issues/5648))
- resource/alicloud_cen_transit_router_vpc_attachment: Added the field tags ([#5660](https://github.com/aliyun/terraform-provider-alicloud/issues/5660))
- resource/alicloud_route_table: Adds new attribute associate_type ([#5656](https://github.com/aliyun/terraform-provider-alicloud/issues/5656))
- resource/alicloud_vpc_ipv4_gateway : Adds new attribute enabled ([#5656](https://github.com/aliyun/terraform-provider-alicloud/issues/5656))
- resource/alicloud_vpn_gateway: Added retry stragety for error code ([#5656](https://github.com/aliyun/terraform-provider-alicloud/issues/5656))
- resource/alicloud_route_entry: Added retry stragety for error code ([#5656](https://github.com/aliyun/terraform-provider-alicloud/issues/5656))
- resource/alicloud_alb_load_balancer: Support new attribute address_ip_version; Add optional StandardWithWaf for load_balancer_edition. ([#5651](https://github.com/aliyun/terraform-provider-alicloud/issues/5651))
- resource/alicloud_vpn_gateway_vco_route: Add retry error code. ([#5647](https://github.com/aliyun/terraform-provider-alicloud/issues/5647))
- resource/alicloud_vpn_pbr_route_entry: Added retry strategy for errorcode TaskConflict. ([#5632](https://github.com/aliyun/terraform-provider-alicloud/issues/5632))
- resource_alicloud_vpn_route_entry: Added retry strategy for error code TaskConflict. ([#5632](https://github.com/aliyun/terraform-provider-alicloud/issues/5632))
- resource/alicloud_kvstore_instance: Setting attribute security_ips to computed to fix the diff error ([#5650](https://github.com/aliyun/terraform-provider-alicloud/issues/5650))
- resource/alicloud_db_instance: Adds checking connection string to meet some instance class without connection issue ([#5649](https://github.com/aliyun/terraform-provider-alicloud/issues/5649))
- resource/alicloud_vpc_nat_ip_cidr: Add retry error code. ([#5639](https://github.com/aliyun/terraform-provider-alicloud/issues/5639))
- resource/alicloud_forward_entry: Add retry error code. ([#5639](https://github.com/aliyun/terraform-provider-alicloud/issues/5639))
- resource/alicloud_nat_gateway: Add retry error code. ([#5639](https://github.com/aliyun/terraform-provider-alicloud/issues/5639))
- resource/alicloud_snat_entry: Add retry error code. ([#5639](https://github.com/aliyun/terraform-provider-alicloud/issues/5639))
- resource/alicloud_vpc_nat_ip: Add retry error code. ([#5639](https://github.com/aliyun/terraform-provider-alicloud/issues/5639))
- resource/alicloud_kvstore_instance: Setting config to computed to avoid diff error; Removes the useless classic testcases ([#5642](https://github.com/aliyun/terraform-provider-alicloud/issues/5642))
- resource/alicloud_ess_scheduled_task: max_value & min_value support set zero value ([#5637](https://github.com/aliyun/terraform-provider-alicloud/issues/5637))
- resource/alicloud_vpn_gateway: Add default value for network_type and fix document ([#5636](https://github.com/aliyun/terraform-provider-alicloud/issues/5636))
- resource/alicloud_kvstore_instance: Corrects the creating timeout to 20min ([#5643](https://github.com/aliyun/terraform-provider-alicloud/issues/5643))
- docs/alicloud_slb_server_group_attachment: Adds notes to avoid conflict error ([#5665](https://github.com/aliyun/terraform-provider-alicloud/issues/5665))

BUG FIXES:

- resource/alicloud_drds_instance: Fixes the InternalError error ([#5643](https://github.com/aliyun/terraform-provider-alicloud/issues/5643))
- resource/alicloud_db_instance:fix RDS bugs ([#5659](https://github.com/aliyun/terraform-provider-alicloud/issues/5659))

## 1.193.0 (November 29, 2022)

- **New Resource:** `alicloud_das_switch_das_pro` ([#5612](https://github.com/aliyun/terraform-provider-alicloud/issues/5612))
- **New Resource:** `alicloud_rds_db_proxy` ([#5596](https://github.com/aliyun/terraform-provider-alicloud/issues/5596))
- **New Resource:** `alicloud_vpc_network_acl_attachment` ([#5598](https://github.com/aliyun/terraform-provider-alicloud/issues/5598))
- **New Resource:** `alicloud_cen_transit_router_cidr` ([#5607](https://github.com/aliyun/terraform-provider-alicloud/issues/5607))
- **New Data Source:** `alicloud_cen_transit_router_cidrs` ([#5607](https://github.com/aliyun/terraform-provider-alicloud/issues/5607))
- **New Data Source:** `alicloud_cloud_sso_access_assignments` ([#5597](https://github.com/aliyun/terraform-provider-alicloud/issues/5597))
- **New Data Source:** `alicloud_rds_cross_regions` ([#5615](https://github.com/aliyun/terraform-provider-alicloud/issues/5615))

ENHANCEMENTS:

- resource/alicloud_vpn_gateway_vpn_attachment: Add update asynchronous wait status ([#5631](https://github.com/aliyun/terraform-provider-alicloud/issues/5631))
- resource/alicloud_vpn_gateway: Added retry stragety for error code ([#5630](https://github.com/aliyun/terraform-provider-alicloud/issues/5630))
- resource/alicloud_vpn_gateway_vpn_attachment: Add update asynchronous wait logic ([#5629](https://github.com/aliyun/terraform-provider-alicloud/issues/5629))
- resource/alicloud_instance: Support new attribute ipv6_address_count and ipv6_addresses. ([#5605](https://github.com/aliyun/terraform-provider-alicloud/issues/5605))
- resource/alicloud_ecs_network_interface: Support new attribute ipv6_address_count and ipv6_addresses ([#5622](https://github.com/aliyun/terraform-provider-alicloud/issues/5622))
- resource/alicloud_vpn_gateway: supports new attribute network_type ([#5627](https://github.com/aliyun/terraform-provider-alicloud/issues/5627))
- resource/alicloud_bastionhost_instance: Added the field plan_code, storage and bandwidth; Supported for new action SetRenewal ([#5595](https://github.com/aliyun/terraform-provider-alicloud/issues/5595))
- resource/resource_alicloud_db_instance_test: Repair automated testing ([#5603](https://github.com/aliyun/terraform-provider-alicloud/issues/5603))
- resource/resource_alicloud_db_instance: Added retry stragety and Instance status verification ([#5603](https://github.com/aliyun/terraform-provider-alicloud/issues/5603))
- resource/alicloud_slb_load_balance: Attribute instance_charge_type is no longer alias of payment_type. ([#5623](https://github.com/aliyun/terraform-provider-alicloud/issues/5623))
- resource/alicloud_ess_scaling_group:support health_check_type ([#5616](https://github.com/aliyun/terraform-provider-alicloud/issues/5616))
- resource/alicloud_vpc_ipv4_cidr_block: Added retry stragety for error code ([#5617](https://github.com/aliyun/terraform-provider-alicloud/issues/5617))
- resource/alicloud_cs_kubernetes_addon: Optimize components uninstall logic ([#5611](https://github.com/aliyun/terraform-provider-alicloud/issues/5611))
- resource/alicloud_route_entry: New enumeration values for documents ([#5602](https://github.com/aliyun/terraform-provider-alicloud/issues/5602))
- resource/alicloud_vpc_peer_connection: Added update api for AcceptVpcPeerConnection,RejectVpcPeerConnection ([#5602](https://github.com/aliyun/terraform-provider-alicloud/issues/5602))
- resource/alicloud_vpc_ipv4_gateway: Added retry stragety for error code OperationConflict ([#5602](https://github.com/aliyun/terraform-provider-alicloud/issues/5602))
- resource/alicloud_dbs_backup_plan: Increase resource creation timeout. ([#5604](https://github.com/aliyun/terraform-provider-alicloud/issues/5604))
- resource/alicloud_alb_server_group: Support new attribute server_group_type. ([#5581](https://github.com/aliyun/terraform-provider-alicloud/issues/5581))
- data_source/alicloud_instance_types: Support new attribute minimum_eni_ipv6_address_quantity. ([#5605](https://github.com/aliyun/terraform-provider-alicloud/issues/5605))
- data_source/alicloud_vswitches: Supports new output ipv6_cidr_block. ([#5605](https://github.com/aliyun/terraform-provider-alicloud/issues/5605))
- docs: Improves the resource docs subcategory ([#5599](https://github.com/aliyun/terraform-provider-alicloud/issues/5599))

BUG FIXES:

- resource/alicloud_vpn_connection: fixed the ike_local_id and ike_remote_id to Computed ([#5624](https://github.com/aliyun/terraform-provider-alicloud/issues/5624))
- resource/alicloud_db_instance_test: fix RDS test bug ([#5625](https://github.com/aliyun/terraform-provider-alicloud/issues/5625))
- resource/alicloud_kvstore_instance: Fixed test case parameters ([#5621](https://github.com/aliyun/terraform-provider-alicloud/issues/5621))
- resource/resource_alicloud_db_instance: Fix payment type conversion ([#5603](https://github.com/aliyun/terraform-provider-alicloud/issues/5603))
- resource/alicloud_kvstore_instance: Fixed problems with importing no values ([#5617](https://github.com/aliyun/terraform-provider-alicloud/issues/5617))
- resource/alicloud_express_connect_virtual_border_router: Fixed import of attributes bandwidth ([#5602](https://github.com/aliyun/terraform-provider-alicloud/issues/5602))
- datasource/alicloud_vpn_gateways: fix problems with testing ([#5628](https://github.com/aliyun/terraform-provider-alicloud/issues/5628))
- data_source/alicloud_instances_test: fix test case TestAccAlicloudECSInstancesDataSourceBasic ([#5620](https://github.com/aliyun/terraform-provider-alicloud/issues/5620))

## 1.192.0 (November 15, 2022)

- **New Resource:** `alicloud_nlb_server_group_server_attachment` ([#5576](https://github.com/aliyun/terraform-provider-alicloud/issues/5576))
- **New Resource:** `alicloud_bp_studio_application` ([#5475](https://github.com/aliyun/terraform-provider-alicloud/issues/5475))
- **New Data Source:** `alicloud_bp_studio_applications` ([#5475](https://github.com/aliyun/terraform-provider-alicloud/issues/5475))
- **New Data Source:** `alicloud_nlb_server_group_server_attachments` ([#5576](https://github.com/aliyun/terraform-provider-alicloud/issues/5576))

ENHANCEMENTS:

- resource/alicloud_db_instance: Enlarges the db instance creating timeout ([#5591](https://github.com/aliyun/terraform-provider-alicloud/issues/5591))
- resource/alicloud_lindorm_instance: Adds new attribute primary_zone_id,primary_vswitch_id ([#5587](https://github.com/aliyun/terraform-provider-alicloud/issues/5587))
- resource/alicloud_cen_transit_router_vpc_attachment: Removed the field route_table_association_enabled and route_table_propagation_enable ([#5588](https://github.com/aliyun/terraform-provider-alicloud/issues/5588))
- resource/alicloud_instance: Support new attribute http_tokens, http_endpoint, http_put_response_hop_limit. ([#5586](https://github.com/aliyun/terraform-provider-alicloud/issues/5586))
- resource/alicloud_resource_manager_shared_resource: The resource_type attribute supports the option of PrefixList and Image. ([#5589](https://github.com/aliyun/terraform-provider-alicloud/issues/5589))
- resource/alicloud_vpc_prefix_list: Added retry stragety for error code SystemBusy, OperationConflict, LastTokenProcessing, IncorrectStatus.PrefixList, IncorrectStatus.%s ([#5579](https://github.com/aliyun/terraform-provider-alicloud/issues/5579))
- resource/alicloud_vswitch: Added retry strategy for error code CreateVSwitch.IncorrectStatus.cbnStatus, IncorrectStatus.%s, IncorrectVSwitchStatus, OperationConflict, OperationFailed.LastTokenProcessing,OperationFailed.DistibuteLock, IncorrectStatus.VSwitch, IncorrectStatus.VpcRouteEntry, ServiceUnavailable, DependencyViolation.SnatEntry, DependencyViolation.MulticastDomain, DependencyViolation, IncorrectRouteEntryStatus, InternalError, TaskConflict, DependencyViolation.EnhancedNatgw, DependencyViolation.RouteTable, DependencyViolation.HaVip, DeleteVSwitch.IncorrectStatus.cbnStatus, LastTokenProcessing, OperationDenied.OtherSubnetProcessing, DependencyViolation.SNAT, DependencyViolation.NetworkAcl ([#5585](https://github.com/aliyun/terraform-provider-alicloud/issues/5585))
- resource/alicloud_vpc_prefix_list: Add notfound error determination ([#5548](https://github.com/aliyun/terraform-provider-alicloud/issues/5548))
- resource/alicloud_ga_bandwidth_package_attachment: Removed the ForceNew for field bandwidth_package_id, supports modifying them online; Supported for new action ReplaceBandwidthPackage ([#5571](https://github.com/aliyun/terraform-provider-alicloud/issues/5571))
- resource/alicloud_ga_listener: Added retry stragety for error code NotExist.BasicBandwidthPackage, NotActive.Listener, Exist.ForwardingRule, Exist.EndpointGroup ([#5575](https://github.com/aliyun/terraform-provider-alicloud/issues/5575))
- resource/alicloud_instance: Add error retry code ([#5582](https://github.com/aliyun/terraform-provider-alicloud/issues/5582))
- resource/alicloud_db_instance: Increase status wait when updating payment type. ([#5574](https://github.com/aliyun/terraform-provider-alicloud/issues/5574))
- Resource:alicloud_express_connect_virtual_border_router.The parameter ([#5578](https://github.com/aliyun/terraform-provider-alicloud/issues/5578))
- docs: Remove incorrect area restriction description. ([#5580](https://github.com/aliyun/terraform-provider-alicloud/issues/5580))

BUG FIXES:

- resource/alicloud_cen_transit_router_prefix_list_association: Fixed the read error caused by next_hop error value ([#5577](https://github.com/aliyun/terraform-provider-alicloud/issues/5577))
- resource/alicloud_nlb_server_group: fix test case TestAccAlicloudNLBServerGroup_basic1. ([#5572](https://github.com/aliyun/terraform-provider-alicloud/issues/5572))
- resource/alicloud_vpc_prefix_list: Fix bugs at creation ([#5582](https://github.com/aliyun/terraform-provider-alicloud/issues/5582))

## 1.191.0 (November 08, 2022)

- **New Resource:** `alicloud_nlb_load_balancer` ([#5561](https://github.com/aliyun/terraform-provider-alicloud/issues/5561))
- **New Resource:** `alicloud_service_mesh_extension_provider` ([#5560](https://github.com/aliyun/terraform-provider-alicloud/issues/5560))
- **New Resource:** `alicloud_nlb_listener` ([#5562](https://github.com/aliyun/terraform-provider-alicloud/issues/5562))
- **New Data Source:** `alicloud_nlb_listeners` ([#5562](https://github.com/aliyun/terraform-provider-alicloud/issues/5562))
- **New Data Source:** `alicloud_service_mesh_extension_providers` ([#5560](https://github.com/aliyun/terraform-provider-alicloud/issues/5560))
- **New Data Source:** `alicloud_nlb_load_balancers` ([#5561](https://github.com/aliyun/terraform-provider-alicloud/issues/5561))

ENHANCEMENTS:

- resource/alicloud_nat_gateway: Added retry strategy for error code IncorrectStatus.VSWITCH ([#5567](https://github.com/aliyun/terraform-provider-alicloud/issues/5567))
- resource/alicloud_vswitch: Added retry strategy for error code CreateVSwitch.IncorrectStatus.cbnStatus ([#5566](https://github.com/aliyun/terraform-provider-alicloud/issues/5566))
- resource/alicloud_click_house_db_cluster: Supported db_cluster_version set to 22.8.5.29 ([#5557](https://github.com/aliyun/terraform-provider-alicloud/issues/5557))
- resource/alicloud_lindorm_instance: Adds new multiple availability zone instance related attribute ([#5568](https://github.com/aliyun/terraform-provider-alicloud/issues/5568))
- resource:resource_alicloud_express_connect_virtual_border_router add attribute include_cross_account_vbr ([#5558](https://github.com/aliyun/terraform-provider-alicloud/issues/5558))
- resource/alicloud_db_instance：Add RDS MySQL large version upgrade ([#5553](https://github.com/aliyun/terraform-provider-alicloud/issues/5553))
- docs: Improves the docs tag of the terraform import command and the docs tag of the template example ([#5563](https://github.com/aliyun/terraform-provider-alicloud/issues/5563))

BUG FIXES:

- resource/alicloud_cms_group_metric_rule: Fixed the create error by targets no value ([#5564](https://github.com/aliyun/terraform-provider-alicloud/issues/5564))

## 1.190.0 (October 31, 2022)

- **New Resource:** `alicloud_ga_acl_entry_attachment` ([#5546](https://github.com/aliyun/terraform-provider-alicloud/issues/5546))
- **New Resource:** `alicloud_adb_db_cluster_lake_version` ([#5541](https://github.com/aliyun/terraform-provider-alicloud/issues/5541))
- **New Data Source:** `alicloud_adb_db_cluster_lake_versions` ([#5541](https://github.com/aliyun/terraform-provider-alicloud/issues/5541))

ENHANCEMENTS:

- resource/alicloud_ga_acl_attachment: Added retry strategy for error code StateError.Acl, StateError.Accelerator, NotActive.Listener ([#5551](https://github.com/aliyun/terraform-provider-alicloud/issues/5551))
- resource/alicloud_ga_ip_set: Added retry strategy for error code NotExist.BasicBandwidthPackage, NotSuitable.RegionSelection ([#5549](https://github.com/aliyun/terraform-provider-alicloud/issues/5549))
- resource/alicloud_ga_bandwidth_package_attachment: Added retry strategy for error code Great erThanGa.IpSetBandwidth, BandwidthIllegal.BandwidthPackage, BindExist.CrossDomain, Exist.EndpointGroup, Exist.IpSet ,BandwidthPackageCannotUnbind.HasCrossRegion, BandwidthPackageCannotUnbind.IpSet, BandwidthPackageCannotUnbind.EndpointGroup, StateError.Accelerator, NotExist.BasicBandwidthPackage ([#5535](https://github.com/aliyun/terraform-provider-alicloud/issues/5535))
- resource/alicloud_ecs_key_pair: Remove the public_key ForceNew attribute ([#5552](https://github.com/aliyun/terraform-provider-alicloud/issues/5552))
- alicloud/alicloud_log_etl: restart etl jobs after update etl config ([#5517](https://github.com/aliyun/terraform-provider-alicloud/issues/5517))
- resource/alicloud_db_backup_policy: RDS backup policy support Category ([#5547](https://github.com/aliyun/terraform-provider-alicloud/issues/5547))
- resource/alicloud_ess_lifecyclehook:support default_result is ROLLBACK ([#5560](https://github.com/aliyun/terraform-provider-alicloud/issues/5560))
- resource/alicloud_eci_container_group: Adds new attribute liveness_probe,readiness_probe,acr_registry_info ([#5548](https://github.com/aliyun/terraform-provider-alicloud/issues/5548))
- data source/alicloud_hbr_backup_jobs: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5536](https://github.com/aliyun/terraform-provider-alicloud/issues/5536))
- docs: Improves the docs tag for terraform import command ([#5556](https://github.com/aliyun/terraform-provider-alicloud/issues/5556))

BUG FIXES:

- resource/alicloud_instance_test: fix test case TestAccAlicloudECSInstanceTypeUpdate and TestAccAlicloudECSInstancSecondaryIps. ([#5453](https://github.com/aliyun/terraform-provider-alicloud/issues/5453))
- resource/alicloud_ga_endpoint_group: Fixed the import error caused by accelerator_id, endpoint_group_type and endpoint_request_protocol no value; Removes the endpoint_configurations.enable_clientip_preservation, endpoint_group_type default value and adds computed ([#5527](https://github.com/aliyun/terraform-provider-alicloud/issues/5527))
- resource/alicloud_ga_bandwidth_package: Fixed the import error caused by billing_type and ratio no value; Removes the cbn_geographic_region_ida, cbn_geographic_region_idb default value and adds computed; Added retry strategy for error code StateError.Accelerator, StateError.BandwidthPackage, BandwidthIllegal.BandwidthPackage ([#5526](https://github.com/aliyun/terraform-provider-alicloud/issues/5526))

## 1.189.0 (October 25, 2022)

- **New Resource:** `alicloud_vpc_public_ip_address_pool_cidr_block` ([#5509](https://github.com/aliyun/terraform-provider-alicloud/issues/5509))
- **New Resource:** `alicloud_gpdb_db_instance_plan` ([#5522](https://github.com/aliyun/terraform-provider-alicloud/issues/5522))
- **New Resource:** `alicloud_rds_service_linked_role` ([#5518](https://github.com/aliyun/terraform-provider-alicloud/issues/5518))
- **New Data Source:** `alicloud_gpdb_db_instance_plans` ([#5522](https://github.com/aliyun/terraform-provider-alicloud/issues/5522))
- **New Data Source:** `alicloud_vpc_public_ip_address_pool_cidr_blocks` ([#5509](https://github.com/aliyun/terraform-provider-alicloud/issues/5509))

ENHANCEMENTS:

- resource/alicloud_rds_upgrade_db_instance:Repair pg major version upgrade ([#5506](https://github.com/aliyun/terraform-provider-alicloud/issues/5506))
- resource/alicloud_ecd_policy_group: Adds new attribute recording_expires ([#5439](https://github.com/aliyun/terraform-provider-alicloud/issues/5439))
- resource/alicloud_cms_group_metric_rule: Adds new attribute targets ([#5539](https://github.com/aliyun/terraform-provider-alicloud/issues/5539))
- resource/alicloud_instance: Supports attribute system_disk_name, system_disk_description import and update. ([#5534](https://github.com/aliyun/terraform-provider-alicloud/issues/5534))
- resource/alicloud_hbr_restore_job: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5504](https://github.com/aliyun/terraform-provider-alicloud/issues/5504))
- resource/alicloud_hbr_ecs_backup_plan: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5532](https://github.com/aliyun/terraform-provider-alicloud/issues/5532))
- resource/alicloud_hbr_ots_backup_plan: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5531](https://github.com/aliyun/terraform-provider-alicloud/issues/5531))
- resource/alicloud_hbr_oss_backup_plan: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5530](https://github.com/aliyun/terraform-provider-alicloud/issues/5530))
- resource/alicloud_hbr_nas_backup_plan: Added the field cross_account_type, cross_account_user_id and cross_account_role_name ([#5503](https://github.com/aliyun/terraform-provider-alicloud/issues/5503))
- resource/alicloud_sae_application: Support new attribute acr_instance_id, acr_assume_role_arn. ([#5511](https://github.com/aliyun/terraform-provider-alicloud/issues/5511))
- resource/alicloud_eip_address: Added the field public_ip_address_pool_id ([#5525](https://github.com/aliyun/terraform-provider-alicloud/issues/5525))
- provider: Supports new environment parameter ALIBABACLOUD_ACCESS_KEY_SECRET and ALIBABACLOUD_ACCESS_KEY_ID ([#5529](https://github.com/aliyun/terraform-provider-alicloud/issues/5529))
- ci: add pipeline debug ([#5528](https://github.com/aliyun/terraform-provider-alicloud/issues/5528))

## 1.188.0 (October 15, 2022)

- **New Resource:** `alicloud_message_service_queue` ([#5444](https://github.com/aliyun/terraform-provider-alicloud/issues/5444))
- **New Resource:** `alicloud_message_service_topic` ([#5446](https://github.com/aliyun/terraform-provider-alicloud/issues/5446))
- **New Resource:** `alicloud_message_service_subscription` ([#5491](https://github.com/aliyun/terraform-provider-alicloud/issues/5491))
- **New Resource:** `alicloud_cen_transit_router_prefix_list_association` ([#5361](https://github.com/aliyun/terraform-provider-alicloud/issues/5361))
- **New Resource:** `alicloud_dms_enterprise_proxy` ([#5479](https://github.com/aliyun/terraform-provider-alicloud/issues/5479))
- **New Data Source:** `alicloud_dms_enterprise_proxies` ([#5479](https://github.com/aliyun/terraform-provider-alicloud/issues/5479))
- **New Data Source:** `alicloud_cen_transit_router_prefix_list_associations` ([#5361](https://github.com/aliyun/terraform-provider-alicloud/issues/5361))
- **New Data Source:** `alicloud_message_service_subscriptions` ([#5491](https://github.com/aliyun/terraform-provider-alicloud/issues/5491))
- **New Data Source:** `alicloud_message_service_topics` ([#5446](https://github.com/aliyun/terraform-provider-alicloud/issues/5446))
- **New Data Source:** `alicloud_message_service_queues` ([#5444](https://github.com/aliyun/terraform-provider-alicloud/issues/5444))

ENHANCEMENTS:

- resource/alicloud_slb_backend_server: Add error retry code ([#5521](https://github.com/aliyun/terraform-provider-alicloud/issues/5521))
- resource/alicloud_mse_cluster: Removed the forceNew for field 'cluster_specification' and instance_count, supports modifying them online; Supported for new action UpdateClusterSpec ([#5501](https://github.com/aliyun/terraform-provider-alicloud/issues/5501))
- resource/alicloud_gpdb_instance: Adds new attribute ssl_enabled ([#5508](https://github.com/aliyun/terraform-provider-alicloud/issues/5508))
- resource/alicloud_instance: Adds new attribute spot_duration ([#5501](https://github.com/aliyun/terraform-provider-alicloud/issues/5501))
- resource/alicloud_lindorm_instance: Remove the discarded fields core_num and core_spec ([#5512](https://github.com/aliyun/terraform-provider-alicloud/issues/5512))
- resource_alicloud_vpn_gateway_vpn_attachment: Corrected field ike_config.local_id, ike_config.remote_id to Computed ([#5493](https://github.com/aliyun/terraform-provider-alicloud/issues/5493))
- resource/alicloud_log_oss_export: adds log_read_role_arn field ([#5498](https://github.com/aliyun/terraform-provider-alicloud/issues/5498))
- resource/alicloud_polardb_cluster: Supported creation_category set to NormalMultimaster ([#5502](https://github.com/aliyun/terraform-provider-alicloud/issues/5502))
- resource/alicloud_cs_kubernetes_node_pool: Add polardb ip whitelist support ([#5495](https://github.com/aliyun/terraform-provider-alicloud/issues/5495))
- resource/alicloud_gpdb_instance: Adds new unit test case and test sweeper. ([#5494](https://github.com/aliyun/terraform-provider-alicloud/issues/5494))
- resource/alicloud_resource_manager_account: Added the field abandon_able_check_id; Supported for new action DeleteAccount ([#5454](https://github.com/aliyun/terraform-provider-alicloud/issues/5454))
- resource/alicloud_instance: Add return value judgment restriction ([#5523](https://github.com/aliyun/terraform-provider-alicloud/issues/5523))
- Resource alicloud_log_store support updating encrypt_conf ([#5507](https://github.com/aliyun/terraform-provider-alicloud/issues/5507))

BUG FIXES:

- resource/alicloud_ecs_launch_template: Fixed InvalidParameter error ([#5496](https://github.com/aliyun/terraform-provider-alicloud/issues/5496))

## 1.187.0 (September 30, 2022)

- **New Resource:** `alicloud_cen_transit_router_grant_attachment` ([#5466](https://github.com/aliyun/terraform-provider-alicloud/issues/5466))
- **New Resource:** `alicloud_vod_editing_project` ([#5443](https://github.com/aliyun/terraform-provider-alicloud/issues/5443))
- **New Resource:** `alicloud_ga_access_log` ([#5434](https://github.com/aliyun/terraform-provider-alicloud/issues/5434))
- **New Resource:** `alicloud_log_oss_export` ([#5440](https://github.com/aliyun/terraform-provider-alicloud/issues/5440))
- **New Resource:** `alicloud_ebs_disk_replica_group` ([#5450](https://github.com/aliyun/terraform-provider-alicloud/issues/5450))
- **New Resource:** `alicloud_nlb_security_policy` ([#5441](https://github.com/aliyun/terraform-provider-alicloud/issues/5441))
- **New Resource:** `alicloud_api_gateway_model` ([#5447](https://github.com/aliyun/terraform-provider-alicloud/issues/5447))
- **New Resource:** `alicloud_api_gateway_plugin` ([#5471](https://github.com/aliyun/terraform-provider-alicloud/issues/5471))
- **New Resource:** `alicloud_ots_secondary_index` ([#5476](https://github.com/aliyun/terraform-provider-alicloud/issues/5476))
- **New Resource:** `alicloud_ots_search_index` ([#5476](https://github.com/aliyun/terraform-provider-alicloud/issues/5476))
- **New Data Source:** `alicloud_ots_search_indexes` ([#5476](https://github.com/aliyun/terraform-provider-alicloud/issues/5476))
- **New Data Source:** `alicloud_ots_secondary_indexes` ([#5476](https://github.com/aliyun/terraform-provider-alicloud/issues/5476))
- **New Data Source:** `alicloud_api_gateway_plugins` ([#5471](https://github.com/aliyun/terraform-provider-alicloud/issues/5471))
- **New Data Source:** `alicloud_api_gateway_models` ([#5447](https://github.com/aliyun/terraform-provider-alicloud/issues/5447))
- **New Data Source:** `alicloud_nlb_security_policies` ([#5441](https://github.com/aliyun/terraform-provider-alicloud/issues/5441))
- **New Data Source:** `alicloud_ebs_regions` ([#5450](https://github.com/aliyun/terraform-provider-alicloud/issues/5450))
- **New Data Source:** `alicloud_ebs_disk_replica_groups` ([#5450](https://github.com/aliyun/terraform-provider-alicloud/issues/5450))
- **New Data Source:** `alicloud_resource_manager_account_deletion_check_task` ([#5418](https://github.com/aliyun/terraform-provider-alicloud/issues/5418))
- **New Data Source:** `alicloud_cs_cluster_credential` ([#5486](https://github.com/aliyun/terraform-provider-alicloud/issues/5486))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes: Failed to get cluster kubeconfig, do not block cluster operation ([#5482](https://github.com/aliyun/terraform-provider-alicloud/issues/5482))
- resource/alicloud_gpdb_instance: Refactoring resources. ([#5474](https://github.com/aliyun/terraform-provider-alicloud/issues/5474))
- resource/alicloud_adb_db_cluster: Supporting to modify db_node_class and db_node_storage at the same time ([#5481](https://github.com/aliyun/terraform-provider-alicloud/issues/5481))
- resource/alicloud_db_instance: Support new attribute Category ([#5480](https://github.com/aliyun/terraform-provider-alicloud/issues/5480))
- resource/alicloud_slb_listener: Adds new attribute proxy_protocol_v2_enabled ([#5469](https://github.com/aliyun/terraform-provider-alicloud/issues/5469))
- resource/alicloud_bastionhost_instance: support for renewal_status renew_period. ([#5342](https://github.com/aliyun/terraform-provider-alicloud/issues/5342))
- resource/alicloud_cen_transit_router_vpn_attachment: Added retry strategy for error code IncorrectStatus.Status ([#5461](https://github.com/aliyun/terraform-provider-alicloud/issues/5461))
- resource/alicloud_cen_transit_router_route_entry: Added retry strategy for error code IncorrectStatus.Status ([#5459](https://github.com/aliyun/terraform-provider-alicloud/issues/5459))
- resource/alicloud_cen_transit_router_route_table_association: Added retry strategy for error code IncorrectStatus.Status ([#5464](https://github.com/aliyun/terraform-provider-alicloud/issues/5464))
- resource/alicloud_cen_transit_router_route_table_propagation: Added retry strategy for error code IncorrectStatus.Status ([#5463](https://github.com/aliyun/terraform-provider-alicloud/issues/5463))
- resource/alicloud_cen_transit_router_vbr_attachment: Added retry strategy for error code IncorrectStatus.Status ([#5462](https://github.com/aliyun/terraform-provider-alicloud/issues/5462))
- resource/alicloud_cen_transit_router_route_table: Added retry strategy for error code IncorrectStatus.Status ([#5460](https://github.com/aliyun/terraform-provider-alicloud/issues/5460))
- resource/alicloud_cen_transit_router_peer_attachment: Added retry strategy for error code IncorrectStatus.Status ([#5458](https://github.com/aliyun/terraform-provider-alicloud/issues/5458))
- resource/alicloud_cen_transit_router: Added retry strategy for error code IncorrectStatus.Status ([#5456](https://github.com/aliyun/terraform-provider-alicloud/issues/5456))
- resource/alicloud_fc_function: add layer attribute ([#5449](https://github.com/aliyun/terraform-provider-alicloud/issues/5449))
- data/alicloud_instance_types: substring match for gpu_spec ([#5433](https://github.com/aliyun/terraform-provider-alicloud/issues/5433))
- client: Replace raw map with sync Map ([#5436](https://github.com/aliyun/terraform-provider-alicloud/issues/5436))
- Support OTS/Tablestore defined column, secondary index and search index. ([#5476](https://github.com/aliyun/terraform-provider-alicloud/issues/5476))
- ci: Improves the ci configure ([#5483](https://github.com/aliyun/terraform-provider-alicloud/issues/5483))

BUG FIXES:

- alicloud_ess_alb_server_group_attachment: support fail retry ([#5485](https://github.com/aliyun/terraform-provider-alicloud/issues/5485))
- resource/alicloud_vpn_gateway_vpn_attachment: Fix error ModifyVpnAttachmentAttribute Api missing RegionId parameters. ([#5477](https://github.com/aliyun/terraform-provider-alicloud/issues/5477))
- resource/alicloud_vpc_peer_connection: fix Vpcpeer endpoint. ([#5472](https://github.com/aliyun/terraform-provider-alicloud/issues/5472))
- resource/alicloud_mse_cluster: Fix unit test panic ([#5487](https://github.com/aliyun/terraform-provider-alicloud/issues/5487))
- testcases: Fix ci test error for ebs ([#5455](https://github.com/aliyun/terraform-provider-alicloud/issues/5455))
- testcases: Fix resource/alicloud_log_alert_test error ([#5457](https://github.com/aliyun/terraform-provider-alicloud/issues/5457))
- testcases: Fix resource/alicloud_log_oss_export_test error ([#5465](https://github.com/aliyun/terraform-provider-alicloud/issues/5465))
- testcase: Fixes the ots_search_indexes testcase error ([#5489](https://github.com/aliyun/terraform-provider-alicloud/issues/5489))

## 1.186.0 (September 19, 2022)

- **New Resource:** `alicloud_vpc_peer_connection` ([#5432](https://github.com/aliyun/terraform-provider-alicloud/issues/5432))
- **New Resource:** `alicloud_vpc_public_ip_address_pool` ([#5396](https://github.com/aliyun/terraform-provider-alicloud/issues/5396))
- **New Resource:** `alicloud_nas_smb_acl_attachment` ([#5353](https://github.com/aliyun/terraform-provider-alicloud/issues/5353))
- **New Resource:** `alicloud_dcdn_waf_policy_domain_attachment` ([#5414](https://github.com/aliyun/terraform-provider-alicloud/issues/5414))
- **New Resource:** `alicloud_nlb_server_group` ([#5425](https://github.com/aliyun/terraform-provider-alicloud/issues/5425))
- **New Data Source:** `alicloud_vpc_peer_connections` ([#5432](https://github.com/aliyun/terraform-provider-alicloud/issues/5432))
- **New Data Source:** `alicloud_nlb_server_groups` ([#5425](https://github.com/aliyun/terraform-provider-alicloud/issues/5425))
- **New Data Source:** `alicloud_vpc_public_ip_address_pools` ([#5396](https://github.com/aliyun/terraform-provider-alicloud/issues/5396))

ENHANCEMENTS:

- resource/alicloud_vpn_gateway_vpn_attachment: Add new attribute internet_ip. ([#5430](https://github.com/aliyun/terraform-provider-alicloud/issues/5430))
- resource/alicloud_cen_transit_router_vpc_attachment: Added retry stragety for error code IncorrectStatus.VpcOrVswitch ([#5421](https://github.com/aliyun/terraform-provider-alicloud/issues/5421))
- resource/alicloud_alidns_record: Added retry stragety for error code LastOperationNotFinished ([#5400](https://github.com/aliyun/terraform-provider-alicloud/issues/5400))
- resource/alicloud_reserved_instance: Remove default value ([#5420](https://github.com/aliyun/terraform-provider-alicloud/issues/5420))
- resource/alicloud_hbr_restore_job: Added the field ots_detail ([#538](https://github.com/aliyun/terraform-provider-alicloud/issues/538))
- resource/alicloud_elasticsearch_instance: Add DescribeInstance action retry;Reduce StateChangeConf delay time to 60*time.Second ([#5419](https://github.com/aliyun/terraform-provider-alicloud/issues/5419))
- resource/alicloud_nas_file_system: Supporting to update attribute capacity ([#5423](https://github.com/aliyun/terraform-provider-alicloud/issues/5423))
- resource/alicloud_vpc: Removes the forceNew for dry_run ([#5424](https://github.com/aliyun/terraform-provider-alicloud/issues/5424))
- resource/alicloud_dns_record: Add retryable error content to dns record creation, modification, and deletion. ([#5412](https://github.com/aliyun/terraform-provider-alicloud/issues/5412))
- testcase: Adds new unit test case for resource alicloud_slb_acl alicloud_sddp_instance alicloud_scdn_domain_config ([#5364](https://github.com/aliyun/terraform-provider-alicloud/issues/5364))
- provider: Improves the skip_region_validation error message ([#5427](https://github.com/aliyun/terraform-provider-alicloud/issues/5427))
- doc/polardb_node_classes: Optimize test cases in documentation. ([#5438](https://github.com/aliyun/terraform-provider-alicloud/issues/5438))

BUG FIXES:

- resource/alicloud_ga_forwarding_rule: fix panic error ([#5410](https://github.com/aliyun/terraform-provider-alicloud/issues/5410))
- resource/alicloud_ga_listener: fixed the security_policy_id to Computed ([#5411](https://github.com/aliyun/terraform-provider-alicloud/issues/5411))
- datasource/alicloud_cs_managed_kubernetes_clusters: Fix attributes bug caused by enable_details ([#5405](https://github.com/aliyun/terraform-provider-alicloud/issues/5405))
- doc/cen_transit_router_vpc_attachment: fix doc example. doc/vpn_gateway_vco_route: Adjust doc subcategory. ([#5426](https://github.com/aliyun/terraform-provider-alicloud/issues/5426))

## 1.185.0 (September 13, 2022)

- **New Resource:** `alicloud_vpc_ipv4_cidr_block` ([#5391](https://github.com/aliyun/terraform-provider-alicloud/issues/5391))
- **New Resource:** `alicloud_api_gateway_log_config` ([#5379](https://github.com/aliyun/terraform-provider-alicloud/issues/5379))
- **New Resource:** `alicloud_dbs_backup_plan` ([#5341](https://github.com/aliyun/terraform-provider-alicloud/issues/5341))
- **New Resource:** `alicloud_dcdn_waf_domain` ([#5386](https://github.com/aliyun/terraform-provider-alicloud/issues/5386))
- **New Data Source:** `alicloud_dcdn_waf_domains` ([#5386](https://github.com/aliyun/terraform-provider-alicloud/issues/5386))
- **New Data Source:** `alicloud_dbs_backup_plans` ([#5341](https://github.com/aliyun/terraform-provider-alicloud/issues/5341))
- **New Data Source:** `alicloud_api_gateway_log_configs` ([#5379](https://github.com/aliyun/terraform-provider-alicloud/issues/5379))

ENHANCEMENTS:

- resource/alicloud_cms_alarm: Fixes the panic error when setting prometheus ([#5417](https://github.com/aliyun/terraform-provider-alicloud/issues/5417))
- resource/alicloud_privatelink_vpc_endpoint: Fixes the panic error when setting security_groups ([#5416](https://github.com/aliyun/terraform-provider-alicloud/issues/5416))
- resource/alicloud_fc_trigger: Fixes the panic error when validating the config ([#5415](https://github.com/aliyun/terraform-provider-alicloud/issues/5415))
- resource/alicloud_ecs_instance_set: Save the instance ids when an error occurs ([#5413](https://github.com/aliyun/terraform-provider-alicloud/issues/5413))
- resource/alicloud_slb_server_group_server_attachment: Add retry error code ([#5409](https://github.com/aliyun/terraform-provider-alicloud/issues/5409))
- resource/alicloud_pvtz_endpoint: Add retry error code ([#5408](https://github.com/aliyun/terraform-provider-alicloud/issues/5408))
- resource/alicloud_edge_kubernetes: add new fields cluster_spec,runtime and load_balancer_spec ([#5355](https://github.com/aliyun/terraform-provider-alicloud/issues/5355))
- resource/alicloud_cs_kubernetes_node_pool: change api for nodepool kubelet config ([#5356](https://github.com/aliyun/terraform-provider-alicloud/issues/5356))
- resource/alicloud_express_connect_physical_connection: supported for 100GBase-LR and 40GBase-LR ([#5394](https://github.com/aliyun/terraform-provider-alicloud/issues/5394))
- resource/alicloud_lindorm_instance: Adds new attribute vpc_id expose the vpc_id parameter ([#5373](https://github.com/aliyun/terraform-provider-alicloud/issues/5373))
- resource/alicloud_route_table: Add retry code IncorrectStatus.cbnStatus ([#5385](https://github.com/aliyun/terraform-provider-alicloud/issues/5385))
- resource/alicloud_network_acl: Added retry stragety for error code NetworkAclExistBinding ([#5374](https://github.com/aliyun/terraform-provider-alicloud/issues/5374))
- resource/alicloud_service_mesh_service_mesh: Change TypeSet to TypeList to avoid resource recreated. ([#5378](https://github.com/aliyun/terraform-provider-alicloud/issues/5378))
- resource/alicloud_polardb_cluster alicloud_hbase_instance alicloud_alikafka_instance alicloud_click_house_db_cluster alicloud_db_instance alicloud_drds_instance alicloud_mse_cluster: Adds new attribute vpc_id expose the vpc_id parameter ([#5384](https://github.com/aliyun/terraform-provider-alicloud/issues/5384))
- resource/alicloud_graph_database_db_instance: Enlarges the creating and deleting default timeout ([#5389](https://github.com/aliyun/terraform-provider-alicloud/issues/5389))
- resource/{alicloud_cs_managed_kubernetes,alicloud_cs_serverless_kubernetes}: Export a new attribute rrsa_metadata ([#5375](https://github.com/aliyun/terraform-provider-alicloud/issues/5375))
- doc/alicloud_cs_edge_kubernetes: add new usage example ([#5403](https://github.com/aliyun/terraform-provider-alicloud/issues/5403))

BUG FIXES:

- resource/alicloud_cs_managed_kubernetes: Fix attributes bug caused by rrsa_metadata ([#5406](https://github.com/aliyun/terraform-provider-alicloud/issues/5406))
- resource/alicloud_cs_managed_kubernetes: Fix migrate bug ([#5371](https://github.com/aliyun/terraform-provider-alicloud/issues/5371))
- resource/alicloud_dcdn_waf_domain: fix test case TestAccAlicloudDCDNWafDomain_basic1 ([#5398](https://github.com/aliyun/terraform-provider-alicloud/issues/5398))
- resource/alicloud_polardb_cluster: Fixes the setting attribute zone_id failed error ([#5387](https://github.com/aliyun/terraform-provider-alicloud/issues/5387))
- testcases: Fix ci test error for ack ([#5399](https://github.com/aliyun/terraform-provider-alicloud/issues/5399))

## 1.184.0 (September 05, 2022)

- **New Resource:** `alicloud_dcdn_waf_policy` ([#5349](https://github.com/aliyun/terraform-provider-alicloud/issues/5349))
- **New Data Source:** `alicloud_dcdn_waf_policies` ([#5349](https://github.com/aliyun/terraform-provider-alicloud/issues/5349))
- **New Data Source:** `alicloud_ram_policy_document` ([#5317](https://github.com/aliyun/terraform-provider-alicloud/issues/5317))
- **New Data Source:** `alicloud_hbr_service` ([#5368](https://github.com/aliyun/terraform-provider-alicloud/issues/5368))

ENHANCEMENTS:

- resource/alicloud_cen_transit_router_vpc_attachment: Removes the field zone_mappings forceNew and supports modifying it online. ([#5362](https://github.com/aliyun/terraform-provider-alicloud/issues/5362))
- resource/alicloud_nat_gateway: Added the field eip_bind_mode ([#5324](https://github.com/aliyun/terraform-provider-alicloud/issues/5324))
- resource/alicloud_kms_key: Supported pending_window_in_days set to 366 ([#5365](https://github.com/aliyun/terraform-provider-alicloud/issues/5365))
- resource/alicloud_vpn_gateway: Added the field auto_propagate ([#5359](https://github.com/aliyun/terraform-provider-alicloud/issues/5359))
- resource/alicloud_eip_address: Removes state refresh after resource creation ([#5350](https://github.com/aliyun/terraform-provider-alicloud/issues/5350))
- resource/alicloud_instance: The Attribute system_disk_category add enumeration value cloud_auto ([#5357](https://github.com/aliyun/terraform-provider-alicloud/issues/5357))
- resource/alicloud_oss_bucket: Adjust to configure Acl during creation. ([#5354](https://github.com/aliyun/terraform-provider-alicloud/issues/5354))
- resource/alicloud_cs_kubernetes_node_pool: soc/cis support AliyunLinux3 platform ([#5360](https://github.com/aliyun/terraform-provider-alicloud/issues/5360))
- resource/alicloud_event_bridge_rule: Added the field push_retry_strategy and dead_letter_queue ([#5336](https://github.com/aliyun/terraform-provider-alicloud/issues/5336))
- resource/alicloud_common_bandwidth_package: Added the field security_protection_types ([#5318](https://github.com/aliyun/terraform-provider-alicloud/issues/5318))
- resource/alicloud_eip_address: Added the field security_protection_types ([#5282](https://github.com/aliyun/terraform-provider-alicloud/issues/5282))

BUG FIXES:

- resource/alicloud_route_entry: Fixed user flow control ([#5367](https://github.com/aliyun/terraform-provider-alicloud/issues/5367))
- resource/alicloud_eip_association: Fix the problem of waiting when associating ECS ([#5350](https://github.com/aliyun/terraform-provider-alicloud/issues/5350))
- resource/alicloud_kubernetes: Fix panic by master_vswitch_ids ([#5352](https://github.com/aliyun/terraform-provider-alicloud/issues/5352))

## 1.183.0 (August 29, 2022)

- **New Resource:** `alicloud_ddos_basic_threshold` ([#5332](https://github.com/aliyun/terraform-provider-alicloud/issues/5332))
- **New Resource:** `alicloud_cen_transit_router_vpn_attachment` ([#5309](https://github.com/aliyun/terraform-provider-alicloud/issues/5309))
- **New Resource:** `alicloud_polardb_parameter_group` ([#5334](https://github.com/aliyun/terraform-provider-alicloud/issues/5334))
- **New Resource:** `alicloud_vpn_gateway_vco_route` ([#5321](https://github.com/aliyun/terraform-provider-alicloud/issues/5321))
- **New Data Source:** `alicloud_vpn_gateway_vco_routes` ([#5321](https://github.com/aliyun/terraform-provider-alicloud/issues/5321))
- **New Data Source:** `alicloud_polardb_parameter_groups` ([#5334](https://github.com/aliyun/terraform-provider-alicloud/issues/5334))	
- **New Data Source:** `alicloud_alb_system_security_policies` ([#5305](https://github.com/aliyun/terraform-provider-alicloud/issues/5305))	
- **New Data Source:** `alicloud_cen_transit_router_vpn_attachments` ([#5309](https://github.com/aliyun/terraform-provider-alicloud/issues/5309))

ENHANCEMENTS:

- resource/alicloud_mse_cluster: Supports new attribute connection_type and request_pars ([#5348](https://github.com/aliyun/terraform-provider-alicloud/issues/5348))
- resource/alicloud_cs_managed_kubernetes: field worker_number and worker_nodes enhancement for outdated version cluster ([#5220](https://github.com/aliyun/terraform-provider-alicloud/issues/5220))
- resource/alicloud_kms_key: support for dkms_instance_id resource/alicloud_kms_secret: support for dkms_instance_id ([#5329](https://github.com/aliyun/terraform-provider-alicloud/issues/5329))
- resource/alicloud_lindorm_instance: Set the user-defined retry time ([#5337](https://github.com/aliyun/terraform-provider-alicloud/issues/5337))
- resource/alicloud_fc_service: support for instance metrics and tracing config ([#5340](https://github.com/aliyun/terraform-provider-alicloud/issues/5340))
- resource/alicloud_ddosbgp_instance: Adds new attribute normal_bandwidth, Remove Api of Destroyed Resources ([#5270](https://github.com/aliyun/terraform-provider-alicloud/issues/5270))
- resource/alicloud_ga_additional_certificate: Added retry stragety for error code NotActive.Listener ([#5338](https://github.com/aliyun/terraform-provider-alicloud/issues/5338))
- resource/alicloud_ga_listener: Added the field security_policy_id ([#5307](https://github.com/aliyun/terraform-provider-alicloud/issues/5307))
- resource/alicloud_instance: Added the field data_disks.device ([#5290](https://github.com/aliyun/terraform-provider-alicloud/issues/5290))
- resource/alicloud_slb_load_balancer: Enlarges the attribute bandwidth maximum value to 5120 ([#5333](https://github.com/aliyun/terraform-provider-alicloud/issues/5333))
- resource/alicloud_log_dashboard: Add field attribute ([#5313](https://github.com/aliyun/terraform-provider-alicloud/issues/5313))
- resource/alicloud_lindorm_instance: Add new enumeration values local_ssd_pro , local_hdd_pro to field disk_category. ([#5331](https://github.com/aliyun/terraform-provider-alicloud/issues/5331))
- resource/alicloud_ga_additional_certificate: Added retry stragety forerror code StateError.Listener, StateError.Accelerator ([#5310](https://github.com/aliyun/terraform-provider-alicloud/issues/5310))
- testcase: Adds new unit test case for resource alicloud_ros_stack_group alicloud_graph_database_db_instance alicloud_rds_account ([#5328](https://github.com/aliyun/terraform-provider-alicloud/issues/5328))

BUG FIXES:

- resource/alicloud_cs_kubernetes: Fix check vpc logic by worker_vswitch_ids ([#5285](https://github.com/aliyun/terraform-provider-alicloud/issues/5285))
- resource/alicloud_eip_association: Fixed problem with tag throttling.user ([#5345](https://github.com/aliyun/terraform-provider-alicloud/issues/5345))
- resource/alicloud_reserved_instance: Supported period_unit set to Month, and period set to 5; Fixed the field offering_type from Required to Optional, and instance_type from Optional to Required ([#5303](https://github.com/aliyun/terraform-provider-alicloud/issues/5303))
- testcase: fix issue for acc test of alb system security policies ([#5330](https://github.com/aliyun/terraform-provider-alicloud/issues/5330))
- testcase: fix resource/alicloud_cs_serverless_kubernetes ci test error ([#5296](https://github.com/aliyun/terraform-provider-alicloud/issues/5296))

## 1.182.0 (August 23, 2022)

- **New Resource:** `alicloud_vpc_prefix_list` ([#5306](https://github.com/aliyun/terraform-provider-alicloud/issues/5306))
- **New Resource:** `alicloud_cms_event_rule` ([#5268](https://github.com/aliyun/terraform-provider-alicloud/issues/5268))
- **New Data Source:** `alicloud_cms_event_rules` ([#5268](https://github.com/aliyun/terraform-provider-alicloud/issues/5268))	
- **New Data Source:** `alicloud_vpc_prefix_lists` ([#5306](https://github.com/aliyun/terraform-provider-alicloud/issues/5306))

ENHANCEMENTS:

- resource/alicloud_lindorm_instance: Field time_serires_engine_specification deprecated and instead by time_series_engine_specification ([#5327](https://github.com/aliyun/terraform-provider-alicloud/issues/5327))
- resource/alicloud_cr_endpoint_acl_policy: Add the second check of the request ([#5319](https://github.com/aliyun/terraform-provider-alicloud/issues/5319))
- resource/lindorm_instace: Removes the useless updateing after creating a new resource ([#5325](https://github.com/aliyun/terraform-provider-alicloud/issues/5325))
- resource/alicloud_polardb_global_database_network: Enlarges the default waiting timeout for deleting the PolarDB Global Database Network ([#5320](https://github.com/aliyun/terraform-provider-alicloud/issues/5320))
- resource/alicloud_ecs_instance_set: exclude instances due to instance creation failure ([#5277](https://github.com/aliyun/terraform-provider-alicloud/issues/5277))
- resource/alicloud_emr_cluster: support modify cluster service config ([#5292](https://github.com/aliyun/terraform-provider-alicloud/issues/5292))
- resource/alicloud_ess_scaling_group: Add support for protected_instances ([#5301](https://github.com/aliyun/terraform-provider-alicloud/issues/5301))
- datasource/alicloud_instances: supported for disk_id, disk_name. ([#5277](https://github.com/aliyun/terraform-provider-alicloud/issues/5277))

BUG FIXES:

- resource/alicloud_alb_rule: Fix verification rules for some attributes. ([#5311](https://github.com/aliyun/terraform-provider-alicloud/issues/5311))
- resource/alicloud_ecs_instance_set: Fix state wait logic error after creation, fix test case. ([#5326](https://github.com/aliyun/terraform-provider-alicloud/issues/5326))
- resource/alicloud_emr_cluster: fix test case testAccAlicloudEmrCluste ([#5315](https://github.com/aliyun/terraform-provider-alicloud/issues/5315))
- doc/cms_namespace: fix example error. ([#5306](https://github.com/aliyun/terraform-provider-alicloud/issues/5306))

## 1.181.0 (August 15, 2022)

- **New Resource:** `alicloud_vpn_gateway_vpn_attachment` ([#5284](https://github.com/aliyun/terraform-provider-alicloud/issues/5284))
- **New Resource:** `alicloud_resource_manager_delegated_administrator` ([#5288](https://github.com/aliyun/terraform-provider-alicloud/issues/5288))
- **New Resource:** `alicloud_polardb_global_database_network` ([#5294](https://github.com/aliyun/terraform-provider-alicloud/issues/5294))
- **New Resource:** `alicloud_vpc_ipv4_gateway` ([#5295](https://github.com/aliyun/terraform-provider-alicloud/issues/5295))
- **New Resource:** `alicloud_api_gateway_backend` ([#5280](https://github.com/aliyun/terraform-provider-alicloud/issues/5280))
- **New Data Source:** `alicloud_api_gateway_backends` ([#5280](https://github.com/aliyun/terraform-provider-alicloud/issues/5280))	
- **New Data Source:** `alicloud_vpc_ipv4_gateways` ([#5295](https://github.com/aliyun/terraform-provider-alicloud/issues/5295))
- **New Data Source:** `Datasourcealicloud_polardb_global_database_networks` ([#5294](https://github.com/aliyun/terraform-provider-alicloud/issues/5294))
- **New Data Source:** `alicloud_resource_manager_delegated_administrators` ([#5288](https://github.com/aliyun/terraform-provider-alicloud/issues/5288))
- **New Data Source:** `alicloud_vpn_gateway_vpn_attachments` ([#5284](https://github.com/aliyun/terraform-provider-alicloud/issues/5284))

ENHANCEMENTS:

- resource/alicloud_vpc_ipv4_gateway: After creation and deletion, the new status waits for judgment. ([#5302](https://github.com/aliyun/terraform-provider-alicloud/issues/5302))
- resource/alicloud_instance: Added the field maintenance_time, maintenance_action and maintenance_notify; Supported for new action ModifyInstanceMaintenanceAttributes ([#5289](https://github.com/aliyun/terraform-provider-alicloud/issues/5289))
- resource/alicloud_resource_manager_account: Added the field tag ([#5278](https://github.com/aliyun/terraform-provider-alicloud/issues/5278))
- resource/alicloud_oos_execution: Remove the status wait after the resource is created. ([#5286](https://github.com/aliyun/terraform-provider-alicloud/issues/5286))
- testcase: Adds new unit test case for resource alicloud_ga_listener alicloud_ga_endpoint_group alicloud_ga_bandwidth_package ([#5283](https://github.com/aliyun/terraform-provider-alicloud/issues/5283))
- doc/fc_layer_version: Update Test Examples ([#5300](https://github.com/aliyun/terraform-provider-alicloud/issues/5300))
- region: add the available region: cn-fuzhou ([#5291](https://github.com/aliyun/terraform-provider-alicloud/issues/5291))
- ci: Imprvoes the auto-trigger ci pipeline ([#5297](https://github.com/aliyun/terraform-provider-alicloud/issues/5297))

BUG FIXES:

- resource/alicloud_instance: Fixed the issue of updating VSwitch timeout ([#5287](https://github.com/aliyun/terraform-provider-alicloud/issues/5287))

## 1.180.0 (August 07, 2022)

- **New Resource:** `alicloud_fc_layer_version` ([#5245](https://github.com/aliyun/terraform-provider-alicloud/issues/5245))
- **New Resource:** `alicloud_ddos_bgp_ip` ([#5265](https://github.com/aliyun/terraform-provider-alicloud/issues/5265))
- **New Data Source:** `alicloud_ddos_bgp_ips` ([#5365](https://github.com/aliyun/terraform-provider-alicloud/issues/5365))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool: support customized kubelet params ([#5257](https://github.com/aliyun/terraform-provider-alicloud/issues/5257))
- resource/alicloud_alikafka_instance: Changed sdk to common api; Supported for new parameter kms_key_id ([#5261](https://github.com/aliyun/terraform-provider-alicloud/issues/5261))
- resource_alicloud_cms_alarm: Adds new attribute tags. ([#5256](https://github.com/aliyun/terraform-provider-alicloud/issues/5256))
- resource_alicloud_cms_alarm: Removed the field 'prometheus' forceNew and supports modifying it online. ([#5252](https://github.com/aliyun/terraform-provider-alicloud/issues/5252))
- resource/alicloud_adb_db_cluster: Improves its waiting time after invoking the create api ([#5263](https://github.com/aliyun/terraform-provider-alicloud/issues/5263))
- resource/alicloud_vpc_nat_ip: Optimizing attribute definition ([#5262](https://github.com/aliyun/terraform-provider-alicloud/issues/5262))
- docs/fc_function_async_invoke_config: update description ([#5242](https://github.com/aliyun/terraform-provider-alicloud/issues/5242))
- testcase: Adds new unit test case for resource alicloud_direct_mail_tag alicloud_direct_mail_receivers ([#5254](https://github.com/aliyun/terraform-provider-alicloud/issues/5254))
- doc/route_entry: add VpcPeer to acceptable values for nexthop_type ([#5170](https://github.com/aliyun/terraform-provider-alicloud/issues/5170))

BUG FIXES:

- resource/alicloud_adb_db_cluster: Fixes the waiting error after modifying its attributes; Enlarges the default waiting timeout for creating the cluster ([#5276](https://github.com/aliyun/terraform-provider-alicloud/issues/5276))
- resource/alicloud_adb_db_cluster: Fixes the waiting error after modifying its attributes; Enlarges the default waiting timeout for deleting the cluster attributes ([#5274](https://github.com/aliyun/terraform-provider-alicloud/issues/5274))
- resource/alicloud_adb_db_cluster: Fixes the IncorrectDBInstanceState error while deleting the cluster; Enlarges the default waiting timeout for updating the cluster attributes ([#5273](https://github.com/aliyun/terraform-provider-alicloud/issues/5273))
- resource/alicloud_ecs_disk: Fixes the size diff bug when setting snapshot_id ([#5272](https://github.com/aliyun/terraform-provider-alicloud/issues/5272))
- resource/alicloud_adb_db_cluster: Fixes the waiting error after modifying its attributes; Enlarges the default waiting timeout for creating the cluster ([#5276](https://github.com/aliyun/terraform-provider-alicloud/issues/5276))
- resource/alicloud_adb_db_cluster: Fixes the waiting error after modifying its attributes; Enlarges the default waiting timeout for deleting the cluster attributes ([#5274](https://github.com/aliyun/terraform-provider-alicloud/issues/5274))
- resource/alicloud_adb_db_cluster: Fixes the IncorrectDBInstanceState error while deleting the cluster; Enlarges the default waiting timeout for updating the cluster attributes ([#5273](https://github.com/aliyun/terraform-provider-alicloud/issues/5273))
- resource/alicloud_ecs_disk: Fixes the size diff bug when setting snapshot_id ([#5272](https://github.com/aliyun/terraform-provider-alicloud/issues/5272))
- resource/alicloud_vpc: Fixed the bug of adding additional network segments to VPC ([#5267](https://github.com/aliyun/terraform-provider-alicloud/issues/5267))
- resource/alicloud_alb_rule: Fix testcase panic error ([#5258](https://github.com/aliyun/terraform-provider-alicloud/issues/5258))
- data/alicloud_alb_rules: Fix panic error ([#5253](https://github.com/aliyun/terraform-provider-alicloud/issues/5253))
- testcase: Fix ci error for resource/alicloud_alb_rule ([#5260](https://github.com/aliyun/terraform-provider-alicloud/issues/5260))
- testcase: fix hbr test case errors. ([#5264](https://github.com/aliyun/terraform-provider-alicloud/issues/5264))
- testcase: fix ci test error for resource/alicloud_cs_managed_kubernetes ([#5249](https://github.com/aliyun/terraform-provider-alicloud/issues/5249))

## 1.179.0 (July 31, 2022)

- **New Resource:** `alicloud_cms_hybrid_monitor_sls_task` ([#5221](https://github.com/aliyun/terraform-provider-alicloud/issues/5221))
- **New Resource:** `alicloud_hbr_hana_backup_plan` ([#5244](https://github.com/aliyun/terraform-provider-alicloud/issues/5244))
- **New Resource:** `alicloud_cms_hybrid_monitor_fc_task` ([#5240](https://github.com/aliyun/terraform-provider-alicloud/issues/5240))
- **New Data Source:** `alicloud_cms_hybrid_monitor_fc_tasks` ([#5240](https://github.com/aliyun/terraform-provider-alicloud/issues/5240))
- **New Data Source:** `alicloud_hbr_hana_backup_plans` ([#5244](https://github.com/aliyun/terraform-provider-alicloud/issues/5244))	
- **New Data Source:** `alicloud_cms_hybrid_monitor_sls_tasks` ([#5221](https://github.com/aliyun/terraform-provider-alicloud/issues/5221))

ENHANCEMENTS:

- resource/alicloud_cms_alarm: Removes the useless error and improves its docs ([#5248](https://github.com/aliyun/terraform-provider-alicloud/issues/5248))
- resource_alicloud_cms_alarm: Adds new attribute prometheus ([#5246](https://github.com/aliyun/terraform-provider-alicloud/issues/5246))
- resource/alicloud_api_gateway_group: Added the field instance_id ([#5214](https://github.com/aliyun/terraform-provider-alicloud/issues/5214))
- resource/resource_alicloud_log_store: support metric store ([#5233](https://github.com/aliyun/terraform-provider-alicloud/issues/5233))
- resource/alicloud_alikafka_instance_allowed_ip_attachment: Added internet to the allowed_type and added "9093/9093" to the port_range. ([#5235](https://github.com/aliyun/terraform-provider-alicloud/issues/5235))
- resource/alicloud_polardb_cluster: Adds new attribute creation_category and creation_option ([#5243](https://github.com/aliyun/terraform-provider-alicloud/issues/5243))
- resource/alicloud_alb_rule: support for server_group_sticky_session ([#5239](https://github.com/aliyun/terraform-provider-alicloud/issues/5239))
- testcase: Adds new unit test case for resource alicloud_privatelink_vpc_endpoint_zone alicloud_kms_secret alicloud_mse_cluster ([#5234](https://github.com/aliyun/terraform-provider-alicloud/issues/5234))
- docs/alicloud_cms_hybrid_monitor_datas: Optimize document format. ([#5215](https://github.com/aliyun/terraform-provider-alicloud/issues/5215))
- docs/alicloud_ecs_activation: Optimize document format. ([#5223](https://github.com/aliyun/terraform-provider-alicloud/issues/5223))

BUG FIXES:

- testcase: fix ci error for resource/alicloud_cs_managed_kubernetes ([#5241](https://github.com/aliyun/terraform-provider-alicloud/issues/5241))

## 1.178.0 (July 27, 2022)

- **New Resource:** `alicloud_cloud_firewall_address_book` ([#5186](https://github.com/aliyun/terraform-provider-alicloud/issues/5186))
- **New Resource:** `alicloud_sms_short_url` ([#5200](https://github.com/aliyun/terraform-provider-alicloud/issues/5200))	
- **New Resource:** `alicloud_hbr_hana_instance` ([#5192](https://github.com/aliyun/terraform-provider-alicloud/issues/5192))
- **New Data Source:** `alicloud_hbr_hana_instances` ([#5192](https://github.com/aliyun/terraform-provider-alicloud/issues/5192))	
- **New Data Source:** `alicloud_cloud_firewall_address_books` ([#5186](https://github.com/aliyun/terraform-provider-alicloud/issues/5186))

ENHANCEMENTS:

- resource_alicloud_adb_db_cluster: Support for new parameters vpc_id, Optimize elastic_io_resource attribute configuration logic. ([#5225](https://github.com/aliyun/terraform-provider-alicloud/issues/5225))
- resource/alicloud_amqp_instance：supports enterprise edtion for rabbitmq ([#5218](https://github.com/aliyun/terraform-provider-alicloud/issues/5218))
- resource/alicloud_actiontrail_trail: Remove restrictions on trail_region attributes, removes the default value and adds computed ([#5216](https://github.com/aliyun/terraform-provider-alicloud/issues/5216))
- testcase: Adds sweeper test for lindorm_instance ([#5217](https://github.com/aliyun/terraform-provider-alicloud/issues/5217))
- testcase: Adds new unit test case for resource alicloud_hbr_server_backup_plan alicloud_hbr_restore_job alicloud_hbr_ots_backup_plan ([#5198](https://github.com/aliyun/terraform-provider-alicloud/issues/5198))
- doc/alicloud_cs_kubernetes_node_pool: enhance doc for field node_name_mode ([#5195](https://github.com/aliyun/terraform-provider-alicloud/issues/5195))
- doc/alicloud_cs_kubernetes: update doc for field api_audiences and service_account_issuer ([#5196](https://github.com/aliyun/terraform-provider-alicloud/issues/5196))

BUG FIXES:

- resource/alicloud_instance: Fixed data_disk error. ([#5237](https://github.com/aliyun/terraform-provider-alicloud/issues/5237))
- testcase: fix ci for datasource/alicloud_cs_kubernetes_clusters and resource/alicloud_cs_kubernetes ([#5232](https://github.com/aliyun/terraform-provider-alicloud/issues/5232))
- testcase: fix unit test case errors ([#5210](https://github.com/aliyun/terraform-provider-alicloud/issues/5210))
- Fixed github action error: go build signal: killed ([#5211](https://github.com/aliyun/terraform-provider-alicloud/issues/5211))

## 1.177.0 (July 21, 2022)

- **New Resource:** `alicloud_ecs_activation` ([#5174](https://github.com/aliyun/terraform-provider-alicloud/issues/5174))
- **New Data Source:** `alicloud_ecs_activations` ([#5174](https://github.com/aliyun/terraform-provider-alicloud/issues/5174))
- **New Data Source:** `alicloud_cms_hybrid_monitor_datas` ([#5165](https://github.com/aliyun/terraform-provider-alicloud/issues/5165))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool: support spot_strategy SpotAsPriceGo and NoSpot ([#5188](https://github.com/aliyun/terraform-provider-alicloud/issues/5188))
- resource/alicloud_cs_kubernetes_node_pool: update sdk and optimize resource update logic ([#5177](https://github.com/aliyun/terraform-provider-alicloud/issues/5177))
- resource/alicloud_polardb_cluster: Adds new attribute sub_category ([#5144](https://github.com/aliyun/terraform-provider-alicloud/issues/5144))
- resource/ess_scaling_configuration:support instance_pattern_info ([#5136](https://github.com/aliyun/terraform-provider-alicloud/issues/5136))
- resource/alicloud_ecs_instance_set: Supports new parameter boot_check_os_with_assistant to choose health check when booting. Check Ecs to Running or cloud assistant to ready. Default by checking cloud assistant, means OS ready. ([#5182](https://github.com/aliyun/terraform-provider-alicloud/issues/5182))
- resource/alicloud_cloud_firewall_control_policy: Add Support for the international site. ([#5173](https://github.com/aliyun/terraform-provider-alicloud/issues/5173))
- resource/alicloud_lindorm_instance: Added the field resource_group_id and tags ([#5175](https://github.com/aliyun/terraform-provider-alicloud/issues/5175))
- resource/alicloud_cen_route_map: Partial update to full update ([#5183](https://github.com/aliyun/terraform-provider-alicloud/issues/5183))
- resource/alicloud_mse_cluster: Add support for new parameter mse_version ([#5167](https://github.com/aliyun/terraform-provider-alicloud/issues/5167))
- resource/alicloud_oos_template: Added the field resource_group_id ([#5163](https://github.com/aliyun/terraform-provider-alicloud/issues/5163))
- resource/alicloud_instance: Refactored resourceAliyunInstanceCreate and added support for new parameter system_disk ([#5151](https://github.com/aliyun/terraform-provider-alicloud/issues/5151))
- resource/alicloud_eci_container_group: Delete default values for memory and cpu. ([#5160](https://github.com/aliyun/terraform-provider-alicloud/issues/5160))
- data/alicloud_cs_kubernetes_clusters, alicloud_cs_managed_kubernetes_clusters, alicloud_cs_serverless_kubernetes_clusters: support exporting kube config file ([#5090](https://github.com/aliyun/terraform-provider-alicloud/issues/5090))
- testcase: Adds new unit test case for resource alicloud_config_aggregate_compliance_pack alicloud_ga_forwarding_rule ([#5142](https://github.com/aliyun/terraform-provider-alicloud/issues/5142))
- testcase: update unit test case name ([#5201](https://github.com/aliyun/terraform-provider-alicloud/issues/5201))
- ci/unit: Adds pipeline job for unit test ([#5203](https://github.com/aliyun/terraform-provider-alicloud/issues/5203))
- ci: Adds sweeper and unit test job ([#5204](https://github.com/aliyun/terraform-provider-alicloud/issues/5204))
- Update gpg image for release workflow ([#5206](https://github.com/aliyun/terraform-provider-alicloud/issues/5206))
- Update gpg image for release workflow ([#5207](https://github.com/aliyun/terraform-provider-alicloud/issues/5207))

BUG FIXES:

- resource/alicloud_db_readonly_instance: method invoke error bug fix. ([#5202](https://github.com/aliyun/terraform-provider-alicloud/issues/5202))
- resource/alicloud_instance: Fixes the describing system disk failed when setting the resource_group_id ([#5194](https://github.com/aliyun/terraform-provider-alicloud/issues/5194))
- resource/alicloud_click_house_db_cluster: Fixed value of payment_type from Prepay to Prepaid ([#5152](https://github.com/aliyun/terraform-provider-alicloud/issues/5152))
- provider: fixes the missing security token error when using assume_role ([#5166](https://github.com/aliyun/terraform-provider-alicloud/issues/5166))

## 1.176.0 (July 12, 2022)

- **New Resource:** `alicloud_ecd_custom_property` ([#5133](https://github.com/aliyun/terraform-provider-alicloud/pull/5133))
- **New Resource:** `alicloud_ecd_ad_connector_office_site` ([#5155](https://github.com/aliyun/terraform-provider-alicloud/pull/5155))
- **New Data Source:** `alicloud_ecd_custom_properties` ([#5133](https://github.com/aliyun/terraform-provider-alicloud/pull/5133))
- **New Data Source:** `alicloud_ecd_ad_connector_office_sites` ([#5155](https://github.com/aliyun/terraform-provider-alicloud/pull/5155))

ENHANCEMENTS:

- resource/resource_alicloud_log_alert: Replace schedule_type, schedule_intervsl with schedule ([#5131](https://github.com/aliyun/terraform-provider-alicloud/pull/5131))
- resource/alicloud_ecs_instance_set: support for exclude_instance_filter ([#5134](https://github.com/aliyun/terraform-provider-alicloud/pull/5134))
- resource/alicloud_alikafka_instance: Supports new output status, upgrade_service_detail_info, allowed_list, domain_endpoint, ssl_domain_endpoint, sasl_domain_endpoint, create_time, msg_retain, expired_time, ssl_end_point ([#5141](https://github.com/aliyun/terraform-provider-alicloud/pull/5141))
- resource/alicloud_alikafka_topic: Supports new output create_time, status and status_name ([#5141](https://github.com/aliyun/terraform-provider-alicloud/pull/5141))
- resource/alicloud_common_bandwidth_package: support for PayByDominantTraffic ([#5149](https://github.com/aliyun/terraform-provider-alicloud/pull/5149))

BUG FIXES:

- datasource/alicloud_alikafka_instances: Fixes the paid_type incorrect value when it is PrePaid ([#5137](https://github.com/aliyun/terraform-provider-alicloud/pull/5137))
- resource/alicloud_alikafka_instance: Fixes alikafka paid_type ([#5140](https://github.com/aliyun/terraform-provider-alicloud/pull/5140))
- testcase: fix ci test error for ack datasource and resource ([#5146](https://github.com/aliyun/terraform-provider-alicloud/pull/5146))
- resource/alicloud_cs_node_pool: fix image_type export error ([#5156](https://github.com/aliyun/terraform-provider-alicloud/pull/5156))

## 1.175.0 (July 10, 2022)

- **NOTE:** This version is not available and using the next version v1.176.0 instead.

## 1.174.0 (July 03, 2022)

- **New Resource:** `alicloud_ecd_ram_directory` ([#5108](https://github.com/aliyun/terraform-provider-alicloud/issues/5108))
- **New Resource:** `alicloud_service_mesh_user_permission` ([#4996](https://github.com/aliyun/terraform-provider-alicloud/issues/4996))	
- **New Resource:** `alicloud_ecd_ad_connector_directory` ([#5122](https://github.com/aliyun/terraform-provider-alicloud/issues/5122))
- **New Data Source:** `alicloud_ecd_ad_connector_directories` ([#5122](https://github.com/aliyun/terraform-provider-alicloud/issues/5122))	
- **New Data Source:** `alicloud_ecd_ram_directories` ([#5108](https://github.com/aliyun/terraform-provider-alicloud/issues/5108))
- **New Data Source:** `alicloud_rds_modify_parameter_logs` ([#5036](https://github.com/aliyun/terraform-provider-alicloud/issues/5036))
- **New Data Source:** `alicloud_ecd_zones` ([#5108](https://github.com/aliyun/terraform-provider-alicloud/issues/5108))

ENHANCEMENTS:

- resource/alicloud_service_mesh_service_mesh: Adds new attribute control_plane_log_enabled,control_plane_log_project,access_log_project ([#5124](https://github.com/aliyun/terraform-provider-alicloud/issues/5124))
- resource/alicloud_security_group_rule: Add support for new parameter ipv6_cidr_ip ([#5120](https://github.com/aliyun/terraform-provider-alicloud/issues/5120))
- resource/alicloud_cms_alarm: Update attribute metric_dimensions ([#5115](https://github.com/aliyun/terraform-provider-alicloud/issues/5115))
- testcase: Adds new unit test case for resource alicloud_ga_additional_certificate alicloud_ecs_dedicated_host alicloud_ecs_disk ([#5107](https://github.com/aliyun/terraform-provider-alicloud/issues/5107))
- docs/alicloud_click_house_regions: Optimize document format ([#5126](https://github.com/aliyun/terraform-provider-alicloud/issues/5126))
- docs/alicloud_ecd_bundles: Optimize document format ([#5126](https://github.com/aliyun/terraform-provider-alicloud/issues/5126))
- docs/alicloud_ess_eci_scaling_configuration: Optimize document format ([#5126](https://github.com/aliyun/terraform-provider-alicloud/issues/5126))
- docs/alicloud_cdn_domain: Delete the cdn_domain.html.markdown file ([#5126](https://github.com/aliyun/terraform-provider-alicloud/issues/5126))

BUG FIXES:

- resource/alicloud_cms_alarm: Fix diff caused by metric_dimensions property ([#5129](https://github.com/aliyun/terraform-provider-alicloud/issues/5129))
- testcase: fixes the kubernetes resource's testcase error ([#5114](https://github.com/aliyun/terraform-provider-alicloud/issues/5114))
- docs: Fix errors in link addresses in documents ([#5062](https://github.com/aliyun/terraform-provider-alicloud/issues/5062))
- doc/cs_kubernetes_version: fix doc field error ([#5113](https://github.com/aliyun/terraform-provider-alicloud/issues/5113))	
- ci/field_check: fix the error ([#5128](https://github.com/aliyun/terraform-provider-alicloud/issues/5128))

## 1.173.0 (June 26, 2022)

- **New Resource:** `alicloud_edas_namespace` ([#5064](https://github.com/aliyun/terraform-provider-alicloud/issues/5064))
- **New Resource:** `alicloud_schedulerx_namespace` ([#5094](https://github.com/aliyun/terraform-provider-alicloud/issues/5094))
- **New Resource:** `alicloud_ehpc_cluster` ([#5086](https://github.com/aliyun/terraform-provider-alicloud/issues/5086))
- **New Resource:** `alicloud_cen_traffic_marking_policy` ([#5100](https://github.com/aliyun/terraform-provider-alicloud/issues/5100))
- **New Resource:** `alicloud_ecs_instance_set` ([#5063](https://github.com/aliyun/terraform-provider-alicloud/issues/5063))  
- **New Data Source:** `alicloud_cen_traffic_marking_policies` ([#5100](https://github.com/aliyun/terraform-provider-alicloud/issues/5100))
- **New Data Source:** `alicloud_ehpc_clusters` ([#5086](https://github.com/aliyun/terraform-provider-alicloud/issues/5086))
- **New Data Source:** `alicloud_schedulerx_namespaces` ([#5094](https://github.com/aliyun/terraform-provider-alicloud/issues/5094))	
- **New Data Source:** `alicloud_edas_namespaces` ([#5064](https://github.com/aliyun/terraform-provider-alicloud/issues/5064))
- **New Data Source:** `alicloud_cdn_blocked_regions` ([#5084](https://github.com/aliyun/terraform-provider-alicloud/issues/5084))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool: support cis/soc security reinforcement ([#5061](https://github.com/aliyun/terraform-provider-alicloud/issues/5061))
- resource/alicloud_cs_kubernetes: add apiserver slb id output ([#5060](https://github.com/aliyun/terraform-provider-alicloud/issues/5060))
- resource/alicloud_polardb_cluster: Adds new attribute imci_switch ([#5087](https://github.com/aliyun/terraform-provider-alicloud/issues/5087))
- resource/resource_alicloud_dts_synchronization_job: Removed the field 'db_list' forceNew and supports modifying it online ([#5103](https://github.com/aliyun/terraform-provider-alicloud/issues/5103))
- resource/resource_alicloud_hbr_vault: Added support for new parameter encrypt_type and kms_key_id ([#5085](https://github.com/aliyun/terraform-provider-alicloud/issues/5085))
- resource/alicloud_cms_alarm: Adds new attribute metric_dimensions ([#5012](https://github.com/aliyun/terraform-provider-alicloud/issues/5012))
- resource/alicloud_resource_manager_shared_resource: The resource_type attribute supports the option of ROSTemplate and ServiceCatalogPortfolio ([#5095](https://github.com/aliyun/terraform-provider-alicloud/issues/5095))
- resource_alicloud_mse_cluster: Modify the parameter pub_network_flow as required; Adds DiffSuppressFunc for acl_entry_list ([#5083](https://github.com/aliyun/terraform-provider-alicloud/issues/5083))
- resource/alicloud_fc_trigger,data_source/alicloud_fc_trigger: support eventbridge trigger type ([#5092](https://github.com/aliyun/terraform-provider-alicloud/issues/5092))
- resource/alicloud_graph_database_db_instance: The db_instance_category attribute supports the option of SINGLE. ([#5091](https://github.com/aliyun/terraform-provider-alicloud/issues/5091))
- resource/alicloud_eci_container_group: Adds the enumeration value of the attribute restart_polic ([#5066](https://github.com/aliyun/terraform-provider-alicloud/issues/5066))
- resource/alicloud_emr_cluster: support bootstrap action specify execution strategy ([#5071](https://github.com/aliyun/terraform-provider-alicloud/issues/5071))
- datasource/alicloud_ecd_network_packages: Supports new output eip_addresses. ([#5080](https://github.com/aliyun/terraform-provider-alicloud/issues/5080))
- doc/config_delivery_channels: Add DEPRECATED identity; docs_website: Remove the link address of the alicloud_cdn_domain. ([#5105](https://github.com/aliyun/terraform-provider-alicloud/issues/5105))	
- provider: Supports setting source_ip while invoking assumeRole ([#5098](https://github.com/aliyun/terraform-provider-alicloud/issues/5098))
- connectivity/client: fix the sdk region in WithEcsClient ([#5093](https://github.com/aliyun/terraform-provider-alicloud/issues/5093))

BUG FIXES:

- resource/alicloud_cs_managed_kubernetes: Fix regx compile bug, update doc and error message. ([#5072](https://github.com/aliyun/terraform-provider-alicloud/issues/5072))
- resource/alicloud_ots_instance: fix validate ots instance name ([#5104](https://github.com/aliyun/terraform-provider-alicloud/issues/5104))
- resource/alicloud_cs_kubernetes_node_pool: fix-bug nodepool labels and taints cannot be annotated ([#5059](https://github.com/aliyun/terraform-provider-alicloud/issues/5059))
- resource/resource_alicloud_slb_backend_server: Fixed ci test error ([#5076](https://github.com/aliyun/terraform-provider-alicloud/issues/5076))
- resource/alicloud_fc_trigger: fix timer trigger payload diff func ([#5099](https://github.com/aliyun/terraform-provider-alicloud/issues/5099))	
- data source/alicloud_kvstore_instances: Fixed ci test error ([#5073](https://github.com/aliyun/terraform-provider-alicloud/issues/5073))
- data source/alicloud_kvstore_connections: Fixed ci test error ([#5074](https://github.com/aliyun/terraform-provider-alicloud/issues/5074))
- doc/alicloud_cs_kubernetes_node_pool: fix import doc error ([#5082](https://github.com/aliyun/terraform-provider-alicloud/issues/5082))

## 1.172.0 (June 19, 2022)

- **New Resource:** `alicloud_config_aggregate_delivery` ([#5077](https://github.com/aliyun/terraform-provider-alicloud/issues/5077))
- **New Resource:** `alicloud_ots_tunnel` ([#5051](https://github.com/aliyun/terraform-provider-alicloud/issues/5051))
- **New Data Source:** `alicloud_ots_tunnels` ([#5051](https://github.com/aliyun/terraform-provider-alicloud/issues/5051))	
- **New Data Source:** `alicloud_config_aggregate_deliveries` ([#5077](https://github.com/aliyun/terraform-provider-alicloud/issues/5077))

ENHANCEMENTS:

- resource/alicloud_ots_table: Support server side encryption ([#5051](https://github.com/aliyun/terraform-provider-alicloud/issues/5051))
- testcase: Adds new unit test case for resource alicloud_ddoscoo_scheduler_rule alicloud_config_configuration_recorder alicloud_data_works_folder ([#5070](https://github.com/aliyun/terraform-provider-alicloud/issues/5070))

BUG FIXES:

- resource/alicloud_vpn_connection: Fix attribute ike_config update error. ([#5078](https://github.com/aliyun/terraform-provider-alicloud/issues/5078))
- docs: Fix errors in link addresses in documents ([#5062](https://github.com/aliyun/terraform-provider-alicloud/issues/5062))

## 1.171.0 (June 12, 2022)

- **New Resource:** `alicloud_config_delivery` ([#5046](https://github.com/aliyun/terraform-provider-alicloud/issues/5046))
- **New Resource:** `alicloud_cms_namespace` ([#5050](https://github.com/aliyun/terraform-provider-alicloud/issues/5050))
- **New Resource:** `alicloud_cms_sls_group` ([#5055](https://github.com/aliyun/terraform-provider-alicloud/issues/5055))
- **New Data Source:** `alicloud_cms_sls_groups` ([#5055](https://github.com/aliyun/terraform-provider-alicloud/issues/5055))	
- **New Data Source:** `alicloud_cms_namespaces` ([#5050](https://github.com/aliyun/terraform-provider-alicloud/issues/5050))	
- **New Data Source:** `alicloud_config_deliveries` ([#5046](https://github.com/aliyun/terraform-provider-alicloud/issues/5046))

ENHANCEMENTS:

- resource/alicloud_cs_managed_kubernetes, alicloud_cs_serverless_kubernetes: ACK and ASK support rrsa ([#5009](https://github.com/aliyun/terraform-provider-alicloud/issues/5009))
- resource/alicloud_mongodb_sharding_network_private_address:Added retry stragety for error code OperationDenied.DBInstanceStatus ([#5033](https://github.com/aliyun/terraform-provider-alicloud/issues/5033))
- resource/alicloud_mongodb_instance:Added retry stragety for error code OperationDenied.DBInstanceStatus ([#5030](https://github.com/aliyun/terraform-provider-alicloud/issues/5030))
- resource/alicloud_ecd_policy_group: Adds new attribute recording recording_start_time recording_end_time recording_fps camera_redirect ([#5048](https://github.com/aliyun/terraform-provider-alicloud/issues/5048))
- resource alicloud_db_instance, alicloud_rds_clone_db_instance,alicloud_rds_upgrade_db_instance add attribute tcp_connection_type to support changing the availability check method of the instance ([#5037](https://github.com/aliyun/terraform-provider-alicloud/issues/5037))
- resource/alicloud_scdn_domain: Field biz_name has been deprecated from provider. ([#5040](https://github.com/aliyun/terraform-provider-alicloud/issues/5040))
- resource/alicloud_graph_database_db_instance: Add support for new parameter vpc_id, vswitch_id and zone_id ([#4975](https://github.com/aliyun/terraform-provider-alicloud/issues/4975))	
- region: add the available regions: cn-beijing-finance-1,cn-beijing-finance-1-pub,cn-szfinance,cn-hzfinance,cn-hzjbp,cn-shenzhen-finance ([#5043](https://github.com/aliyun/terraform-provider-alicloud/issues/5043))
- testcase: Adds new unit test case for resource alicloud_cms_dynamic_tag_group alicloud_cms_monitor_group_instances alicloud_cms_monitor_group ([#5039](https://github.com/aliyun/terraform-provider-alicloud/issues/5039))

BUG FIXES:

- resource/alicloud_sae_application:Fixed ci test error ([#5038](https://github.com/aliyun/terraform-provider-alicloud/issues/5038))
- resource/alicloud_ess_scaling_group:Fixed ci test error ([#5041](https://github.com/aliyun/terraform-provider-alicloud/issues/5041))

## 1.170.0 (June 05, 2022)

- **New Resource:** `alicloud_ecd_bundle` ([#5029](https://github.com/aliyun/terraform-provider-alicloud/issues/5029))	
- **New Data Source:** `alicloud_ecd_desktop_types` ([#5021](https://github.com/aliyun/terraform-provider-alicloud/issues/5021))

ENHANCEMENTS:

- resource/alicloud_service_mesh_service_mesh: support updating the field version ([#5034](https://github.com/aliyun/terraform-provider-alicloud/issues/5034))
- resource_alicloud_eci_container_group: Add support for new parameter auto_create_eip, eip_bandwidth, eip_instance_id ([#5011](https://github.com/aliyun/terraform-provider-alicloud/issues/5011))
- resource/alicloud_ons_topic: perm attribute no longer supports updates. ([#5019](https://github.com/aliyun/terraform-provider-alicloud/issues/5019))
- resource/alicloud_slb_backend_server: Supports adding eci backend servers resource/alicloud_eci_container_group: add the field internet_ip and intranet_ip ([#5018](https://github.com/aliyun/terraform-provider-alicloud/issues/5018))
- resource/alicloud_eci_container_group: Adds new attribute plain_http_registry insecure_registry ([#5020](https://github.com/aliyun/terraform-provider-alicloud/issues/5020))
- resource/alicloud_instance: add the field stopped_mode ([#5012](https://github.com/aliyun/terraform-provider-alicloud/issues/5012))
- resource/alicloud_polardb_backup_policy: Adds new attribute backup_retention_policy_on_cluster_deletion ([#4997](https://github.com/aliyun/terraform-provider-alicloud/issues/4997))
- datasource/alicloud_hbr_vaults: removed the vault_type's default value ([#5013](https://github.com/aliyun/terraform-provider-alicloud/issues/5013))
- datasource/alicloud_ecd_images: add the query field os_type and desktop_instance_type. ([#5029](https://github.com/aliyun/terraform-provider-alicloud/issues/5029))
- testcase: Adds new unit test case for resource alicloud_simple_application_server_snapshot alicloud_simple_application_server_firewall_rule alicloud_simple_application_server_custom_image ([#5015](https://github.com/aliyun/terraform-provider-alicloud/issues/5015))
- testcase: Adds new unit test case for resource alicloud_dms_enterprise_instance alicloud_bastionhost_host_share_key alicloud_simple_application_server_instance ([#5026](https://github.com/aliyun/terraform-provider-alicloud/issues/5026))	
- CS client supports header security_transport ([#5024](https://github.com/aliyun/terraform-provider-alicloud/issues/5024))
- region: add the available regions: cn-hangzhou-finance,ap-northeast-2 ([#5028](https://github.com/aliyun/terraform-provider-alicloud/issues/5028))

BUG FIXES:

- resource/alicloud_service_mesh_service_mesh: fix the issue when cr_aggregation_enabled is empty ([#5014](https://github.com/aliyun/terraform-provider-alicloud/issues/5014))
- data source/alicloud_nas_filesets: Fixed the attribute name of the field from UpdateTiem to UpdateTime ([#5017](https://github.com/aliyun/terraform-provider-alicloud/issues/5017))
- data source/alicloud_bastionhost_instances_test: Fixed ci test error ([#5023](https://github.com/aliyun/terraform-provider-alicloud/issues/5023))

## 1.169.0 (May 29, 2022)

- **New Resource:** `alicloud_ecd_snapshot` ([#4981](https://github.com/aliyun/terraform-provider-alicloud/issues/4981))
- **New Data Source:** `alicloud_ecd_snapshots` ([#4981](https://github.com/aliyun/terraform-provider-alicloud/issues/4981))
- **New Data Source:** `data_source_alicloud_cs_kubernetes_version` ([#4981](https://github.com/aliyun/terraform-provider-alicloud/issues/4981))
- **New Data Source:** `alicloud_tag_meta_tags` ([#5000](https://github.com/aliyun/terraform-provider-alicloud/issues/5000))

ENHANCEMENTS:

- resource/resource_alicloud_polardb_cluster:Add new attribute deletion_lock ([#4985](https://github.com/aliyun/terraform-provider-alicloud/issues/4985))
- resource/alicloud_ga_bandwidth_package: Add support for new parameter auto_renew_duration and renewal_status ([#4978](https://github.com/aliyun/terraform-provider-alicloud/issues/4978))
- resource/alicloud_bastionhost_instance: Support for new parameters ad_auth_server and ldap_auth_server. ([#4904](https://github.com/aliyun/terraform-provider-alicloud/issues/4904))
- resource/alicloud_emr_cluster:support graceful decommission of hadoop ([#4972](https://github.com/aliyun/terraform-provider-alicloud/issues/4972))
- resource/alicloud_service_mesh_service_mesh: add the field extra_configuration ([#4989](https://github.com/aliyun/terraform-provider-alicloud/issues/4989))	
- testcase: Adds new unit test case for alicloud_ecp_instance alicloud_kms_key_version alicloud_kms_alias ([#4993](https://github.com/aliyun/terraform-provider-alicloud/issues/4993))
- CS client support header x-acs-source-ip and x-acs-secure-transport ([#4954](https://github.com/aliyun/terraform-provider-alicloud/issues/4954))

BUG FIXES:

- resource/alicloud_nas_mount_target: Fixes Invalid param mount target domain for nas mount target ([#5005](https://github.com/aliyun/terraform-provider-alicloud/issues/5005))
- resource/alicloud_eci_container_group_test: Fixed region not support errors for ECI ([#5001](https://github.com/aliyun/terraform-provider-alicloud/issues/5001))
- resource/alicloud_smartag_flow_log_test: fix ci test error. ([#4991](https://github.com/aliyun/terraform-provider-alicloud/issues/4991))
- resource/alicloud_slb_listener: Fix errors bandwidth missing Computed ([#4992](https://github.com/aliyun/terraform-provider-alicloud/issues/4992))
- resource/alicloud_instance: Fixed an issue where updating the property system_disk_auto_snapshot_policy_id caused the instance to be recreated ([#5003](https://github.com/aliyun/terraform-provider-alicloud/issues/5003))
- resource/alicloud_click_house_account: Fix the value range of the dml_authority attribute. ([#5008](https://github.com/aliyun/terraform-provider-alicloud/issues/5008))
- resource/alicloud_ecd_user: Fix error setting default password ([#4988](https://github.com/aliyun/terraform-provider-alicloud/issues/4988))
- resource/alicloud_msc_sub_contact: fix email regex ([#5004](https://github.com/aliyun/terraform-provider-alicloud/issues/5004))

## 1.168.0 (May 22, 2022)

- **New Resource:** `alicloud_ecs_invocation` ([#4971](https://github.com/aliyun/terraform-provider-alicloud/issues/4971))
- **New Resource:** `alicloud_ddos_basic_defense_threshold` ([#4973](https://github.com/aliyun/terraform-provider-alicloud/issues/4973))	
- **New Resource:** `alicloud_smartag_flow_log` ([#4982](https://github.com/aliyun/terraform-provider-alicloud/issues/4982))
- **New Data Source:** `alicloud_smartag_flow_logs` ([#4982](https://github.com/aliyun/terraform-provider-alicloud/issues/4982))	
- **New Data Source:** `alicloud_ecs_invocations` ([#4971](https://github.com/aliyun/terraform-provider-alicloud/issues/4971))

ENHANCEMENTS:

- resource/alicloud_db_instance: add the field ([#4932](https://github.com/aliyun/terraform-provider-alicloud/issues/4932))
- resource/alicloud_cen_transit_router_vpc_attachment: Add support for new parameter payment_type. ([#4968](https://github.com/aliyun/terraform-provider-alicloud/issues/4968))
- testcase: Adds new unit test case for alicloud_mhub_product alicloud_mhub_app alicloud_database_gateway_gateway ([#4977](https://github.com/aliyun/terraform-provider-alicloud/issues/4977))

BUG FIXES:

- resource/alicloud_hbr_ots_backup_plan: fix the field type ([#4955](https://github.com/aliyun/terraform-provider-alicloud/issues/4955))
- resource/alicloud_click_house_account: Fixes updating the attribute ddl_authority is not working bug ([#4979](https://github.com/aliyun/terraform-provider-alicloud/issues/4979))
- resource/alicloud_fc_function_async_invoke_config:add field statefullnvocation bug fix ([#4965](https://github.com/aliyun/terraform-provider-alicloud/issues/4965))
- resource/alicloud_ess_scaling_group: Fix desired_capacity ([#4967](https://github.com/aliyun/terraform-provider-alicloud/issues/4967))

## 1.167.0 (May 15, 2022)

- **New Resource:** `alicloud_ga_accelerator_spare_ip_attachment` ([#4944](https://github.com/aliyun/terraform-provider-alicloud/issues/4944))
- **New Data Source:** `alicloud_ga_accelerator_spare_ip_attachments` ([#4944](https://github.com/aliyun/terraform-provider-alicloud/issues/4944))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool:update nodepool document ([#4959](https://github.com/aliyun/terraform-provider-alicloud/issues/4959))
- resource/alicloud_cen_route_map: Add support for new parameter transit_router_route_table_id. ([#4957](https://github.com/aliyun/terraform-provider-alicloud/issues/4957))
- resource/alicloud_db_readonly_instance、alicloud_rds_clone_db_instance、alicloud_rds_upgrade_db_instance add deletion protection function. ([#4936](https://github.com/aliyun/terraform-provider-alicloud/issues/4936))
- resource/alicloud_sae_application: Add support for new parameter tags. ([#4953](https://github.com/aliyun/terraform-provider-alicloud/issues/4953))
- resource/alicloud_fc_function_async_invoke_config:add field statefulInvocation and update docs ([#4945](https://github.com/aliyun/terraform-provider-alicloud/issues/4945))
- resource/alicloud_msc_sub_contact：modify email validate regex ([#4933](https://github.com/aliyun/terraform-provider-alicloud/issues/4933))
- resource/alicloud_network_acl: request UpdateEgressAclEntries parameter error ([#4940](https://github.com/aliyun/terraform-provider-alicloud/issues/4940))
- datasource/alicloud_instance_types: Supports new output nvme_support ([#4963](https://github.com/aliyun/terraform-provider-alicloud/issues/4963))
- testcase: Improves the vbr testcases ([#4942](https://github.com/aliyun/terraform-provider-alicloud/issues/4942))
- testcase: Adds new unit test case for resource alicloud_privatelink_vpc_endpoint alicloud_privatelink_vpc_endpoint_service alicloud_privatelink_vpc_endpoint_service_user ([#4926](https://github.com/aliyun/terraform-provider-alicloud/issues/4926))
- testcase: Adds new unit test case for resource alicloud_quick_bi_user alicloud_quotas_quota_alarm alicloud_quotas_quota_application ([#4931](https://github.com/aliyun/terraform-provider-alicloud/issues/4931))
- testcase: Adds new unit test case for resource alicloud_resource_manager_account alicloud_rds_parameter_group alicloud_rdc_organization ([#4935](https://github.com/aliyun/terraform-provider-alicloud/issues/4935))
- testcase: Adds new unit test case for resource alicloud_resource_manager_policy_version alicloud_resource_manager_control_policy alicloud_resource_manager_control_policy_attachment ([#4941](https://github.com/aliyun/terraform-provider-alicloud/issues/4941))
- testcase: Adds new unit test case for resource alicloud_resource_manager_resource_share alicloud_resource_manager_resource_directory alicloud_resource_manager_resource_group ([#4946](https://github.com/aliyun/terraform-provider-alicloud/issues/4946))
- testcase: Adds new unit test case for resource alicloud_resource_manager_shared_target alicloud_resource_manager_shared_resource alicloud_resource_manager_role ([#4951](https://github.com/aliyun/terraform-provider-alicloud/issues/4951))
- testcase: Adds new unit test case for resource alicloud_ros_stack alicloud_ros_template alicloud_ros_change_set ([#4958](https://github.com/aliyun/terraform-provider-alicloud/issues/4958))
- testcase: Adds new unit test case for resource alicloud_brain_industr ial_pid_organization alicloud_brain_industrial_pid_project alicloud_cassandra_backup_plan ([#4961](https://github.com/aliyun/terraform-provider-alicloud/issues/4961))

BUG FIXES:

- resource/alicloud_sae_application_scaling_rule: Fix scaling_rule_timer.schedules have default values. ([#4937](https://github.com/aliyun/terraform-provider-alicloud/issues/4937))
- resource /alicloud_dts_synchronization_job: Fixed uppercase conversion error and resource /alicloud_mongodb_instance: Removed verification of db_instance_storage ([#4949](https://github.com/aliyun/terraform-provider-alicloud/issues/4949))
- resource/alicloud_slb_backend_server: Fix bugs that do not carry serverIp when updating. ([#4948](https://github.com/aliyun/terraform-provider-alicloud/issues/4948))
- resource/alicloud_db_instance：deletion_protection bug fix. ([#4960](https://github.com/aliyun/terraform-provider-alicloud/issues/4960))

## 1.166.0 (May 07, 2022)

- **New Resource:** `alb_acl_entry_attachment` ([#4913](https://github.com/aliyun/terraform-provider-alicloud/issues/4913))
- **New Resource:** `alicloud_ecs_network_interface_permission` ([#4912](https://github.com/aliyun/terraform-provider-alicloud/issues/4912))
- **New Resource:** `alicloud_mse_engine_namespace` ([#4920](https://github.com/aliyun/terraform-provider-alicloud/issues/4920))
- **New Data Source:** `alicloud_mse_engine_namespaces` ([#4920](https://github.com/aliyun/terraform-provider-alicloud/issues/4920))	
- **New Data Source:** `alicloud_ecs_network_interface_permissions` ([#4912](https://github.com/aliyun/terraform-provider-alicloud/issues/4912))

ENHANCEMENTS:

- resource/alicloud_eci_container: Support field auto_match_image_cache ([#4918](https://github.com/aliyun/terraform-provider-alicloud/issues/4918))
- resource/alicloud_adb_db_cluster: support converting the and 'pay_type' ([#4916](https://github.com/aliyun/terraform-provider-alicloud/issues/4916))
- resource/alicloud_service_mesh_service_mesh: add the field 'cluster_spec' and 'cluster_ids' ([#4921](https://github.com/aliyun/terraform-provider-alicloud/issues/4921))
- resource/alicloud_cs_kubernetes_node_pool: ACK nodepool support system disk BYOK ([#4898](https://github.com/aliyun/terraform-provider-alicloud/issues/4898))
- resource/alicloud_cs_kubernetes_addon: Support to modify the custom configuration of the kubernetes cluster addon ([#4875](https://github.com/aliyun/terraform-provider-alicloud/issues/4875))
- resource/alicloud_express_connect_virtual_border_router: add support for new filed route_table_id ([#4908](https://github.com/aliyun/terraform-provider-alicloud/issues/4908))
- data source/alicloud_db_instance_classes: add commodity_code attribute to support filtered by commodity_code ([#4887](https://github.com/aliyun/terraform-provider-alicloud/issues/4887))
- testcase: Adds new unit test case for resource alicloud_msc_sub_contact alicloud_mongodb_sharding_network_public_address alicloud_msc_sub_webhook ([#4900](https://github.com/aliyun/terraform-provider-alicloud/issues/4900))
- testcase: Adds new unit test case for resource alicloud_mse_cluster alicloud_ons_group alicloud_ons_instance ([#4915](https://github.com/aliyun/terraform-provider-alicloud/issues/4915))
- testcase: Adds new unit test case for resource alicloud_hbr_replication_vault alicloud_hbr_vault alicloud_msc_sub_subscription ([#4919](https://github.com/aliyun/terraform-provider-alicloud/issues/4919))
- testcase: Adds new unit test case for resource alicloud_mongodb_serverless_instance alicloud_mongodb_audit_policy alicloud_mongodb_account ([#4897](https://github.com/aliyun/terraform-provider-alicloud/issues/4897))
- testcase: Adds new unit test case for resource alicloud_ons_topic alicloud_privatelink_vpc_endpoint_connection alicloud_privatelink_vpc_endpoint_service_resource ([#4922](https://github.com/aliyun/terraform-provider-alicloud/issues/4922))
- testcases: Improves the alicloud_imp_app_template testcases ([#4897](https://github.com/aliyun/terraform-provider-alicloud/issues/4897))	
- ci: checkout the oss bucket name ([#4668](https://github.com/aliyun/terraform-provider-alicloud/issues/4668))

BUG FIXES:

- resource/alicloud_slb_acl: Fix bugs that cannot create ipv6. ([#4925](https://github.com/aliyun/terraform-provider-alicloud/issues/4925))
- datasource/alicloud_ram_roles: Fixed user flow control ([#4917](https://github.com/aliyun/terraform-provider-alicloud/issues/4917))

## 1.165.0 (April 24, 2022)

- **New Resource:** `alicloud_bastionhost_host_share_key` ([#4879](https://github.com/aliyun/terraform-provider-alicloud/issues/4879))
- **New Resource:** `alicloud_cdn_fc_trigger` ([#4882](https://github.com/aliyun/terraform-provider-alicloud/issues/4882))	
- **New Resource:** `alicloud_sae_load_balancer_intranet` ([#4894](https://github.com/aliyun/terraform-provider-alicloud/issues/4894))
- **New Resource:** `alicloud_bastionhost_host_account_share_key_attachment` ([#4895](https://github.com/aliyun/terraform-provider-alicloud/issues/4895))	
- **New Data Source:** `alicloud_bastionhost_host_share_keys` ([#4879](https://github.com/aliyun/terraform-provider-alicloud/issues/4879)) 

ENHANCEMENTS:

- Supports new region ap-southeast-7 ([#4903](https://github.com/aliyun/terraform-provider-alicloud/issues/4903))
- client/alicloud_ssl_xxx: Improves the ssl resources endpoint setting while invoking its openapi; Improves the testcases name ([#4902](https://github.com/aliyun/terraform-provider-alicloud/issues/4902))
- resource/alicloud_vpc_flow_log: Adds retry stragety for error code OperationConflict ([#4891](https://github.com/aliyun/terraform-provider-alicloud/issues/4891))
- resource/alicloud_db_instance: connection_prefix code location adjust. ([#4886](https://github.com/aliyun/terraform-provider-alicloud/issues/4886))
- resource/alicloud_ga_bandwidth_package_attachment: Enlarges the default timeout for creating and deleting ([#4884](https://github.com/aliyun/terraform-provider-alicloud/issues/4884))
- resource/alicloud_instance: remove the status's default value ([#4873](https://github.com/aliyun/terraform-provider-alicloud/issues/4873))
- resource/alicloud_polardb_cluster: Improves setting the attribute db_cluster_ip_array ([#4880](https://github.com/aliyun/terraform-provider-alicloud/issues/4880))
- resource/alicloud_db_instance: add attribute deletion_protection to support switch delete protect. ([#4829](https://github.com/aliyun/terraform-provider-alicloud/issues/4829))
- resource/alicloud_route_table_attachment.: Adds retry stragety for error code OperationConflict ([#4877](https://github.com/aliyun/terraform-provider-alicloud/issues/4877))
- resource/alicloud_express_connect_virtual_border_router: Adds retry stragety for error code TaskConflict ([#4878](https://github.com/aliyun/terraform-provider-alicloud/issues/4878))
- resource/alicloud_cen_transit_vbr_atachment: Enlarges the default timeout for creating, updateing and deleting ([#4878](https://github.com/aliyun/terraform-provider-alicloud/issues/4878))
- resource/alicloud_config_aggregate_compliance_pack，alicloud_config_compliance_pack： Added error code Invalid.ConfigRuleId.Value while detach rule in config compliance pack ([#4725](https://github.com/aliyun/terraform-provider-alicloud/issues/4725))	
- datasource/alicloud_images: add the query field image_owner_id ([#4892](https://github.com/aliyun/terraform-provider-alicloud/issues/4892))	
- testcase: Improves the fc resources testcases ([#4881](https://github.com/aliyun/terraform-provider-alicloud/issues/4881))
- testcase: Improves the ecs launchTemplate testcases ([#4893](https://github.com/aliyun/terraform-provider-alicloud/issues/4893))

BUG FIXES:

- docs: Fixes the docs example bug in fc resources ([#4905](https://github.com/aliyun/terraform-provider-alicloud/issues/4905))
- resource/alicloud_cms_alarm : Fixes the empty pointer error ([#4885](https://github.com/aliyun/terraform-provider-alicloud/issues/4885))
- resource/alicloud_polardb_cluster: Fixes updating the attribute db_cluster_ip_array is not working bug ([#4883](https://github.com/aliyun/terraform-provider-alicloud/issues/4883))

## 1.164.0 (April 17, 2022)

- **New Resource:** `alicloud_sae_load_balancer_internet` ([#4868](https://github.com/aliyun/terraform-provider-alicloud/issues/4868))
- **New Resource:** `alicloud_ess_eci_scaling_configuration` ([#4855](https://github.com/aliyun/terraform-provider-alicloud/issues/4855))
- **New Data Source:** `alicloud_hbr_ots_snapshots` ([#4861](https://github.com/aliyun/terraform-provider-alicloud/issues/4861))

ENHANCEMENTS:

- resource/alicloud_ess_alb_server_group_attachment: support force_attach is false ([#4824](https://github.com/aliyun/terraform-provider-alicloud/issues/4824))
- resource/load_balancer_internet: update the field internet_slb_id from required to optional ([#4871](https://github.com/aliyun/terraform-provider-alicloud/issues/4871))
- resource/alicloud_r_kvstore: Filter out the security ip generated by the system ([#4869](https://github.com/aliyun/terraform-provider-alicloud/issues/4869))
- resource/alicloud_instance: Support field operator_type. ([#4851](https://github.com/aliyun/terraform-provider-alicloud/issues/4851))
- resource/alicloud_cs_autoscaling_config: Support scale_down_enabled and expander parameter ([#4844](https://github.com/aliyun/terraform-provider-alicloud/issues/4844))
- resource/alicloud_log_dashboard: update dashboard to support action in char_list ([#4860](https://github.com/aliyun/terraform-provider-alicloud/issues/4860))
- resource/alicloud_cen_transit_vbr_atachment: Enlarges the default timeout for creating, updateing and deleting ([#4865](https://github.com/aliyun/terraform-provider-alicloud/issues/4865))
- resource/alicloud_kvstore_instance: Added error retry code Task.Conflict ([#4848](https://github.com/aliyun/terraform-provider-alicloud/issues/4848))
- resource/alicloud_mse_cluster: Improves the throwing error message implementation while invoking the OpenAPI ([#4846](https://github.com/aliyun/terraform-provider-alicloud/issues/4846))
- datasource/alicloud_bastionhost_instances: Updates its dependence SDK ([#4853](https://github.com/aliyun/terraform-provider-alicloud/issues/4853))
- datasource/alicloud_sae_applications: Support new field oss_mount_details ([#4858](https://github.com/aliyun/terraform-provider-alicloud/issues/4858))	
- datasource/hbr_backup_jobs: add the field ots_detail && alicoud/hbr_backup_plan: add the field rule	
- testcase: Adds new unit test case for resource alicloud_dms_enterprise_user alicloud_dts_consumer_channel alicloud_dts_job_monitor_rule ([#4821](https://github.com/aliyun/terraform-provider-alicloud/issues/4821))
- testcase: Adds new unit test case for resource alicloud_eci_virtual_node alicloud_dts_synchronization_instance alicloud_eais_instance ([#4822](https://github.com/aliyun/terraform-provider-alicloud/issues/4822))
- testcase: Adds new unit test case for resource alicloud_eip_address alicloud_eipanycast_anycast_eip_address alicloud_ehpc_job_template ([#4830](https://github.com/aliyun/terraform-provider-alicloud/issues/4830))
- testcase: Adds new unit test case for resource alicloud_event_bridge_event_bus alicloud_event_bridge_event_source alicloud_ens_key_pair ([#4839](https://github.com/aliyun/terraform-provider-alicloud/issues/4839))
- testcase: Adds new unit test case for resource alicloud_event_bridge_service_linked_role alicloud_express_connect_physical_connection alicloud_express_connect_virtual_border_router ([#4850](https://github.com/aliyun/terraform-provider-alicloud/issues/4850))
- testcase: Improves the alicloud_common_bandwidth_attachment testcase ([#4859](https://github.com/aliyun/terraform-provider-alicloud/issues/4859))
- testcase: Adds new unit test case for resource alicloud_fnf_schedule alicloud_fnf_flow alicloud_fnf_execution ([#4856](https://github.com/aliyun/terraform-provider-alicloud/issues/4856))
- testcase: Adds new unit test case for resource alicloud_iot_device_group alicloud_imm_project alicloud_imp_app_template ([#4867](https://github.com/aliyun/terraform-provider-alicloud/issues/4867))
- testcase: Adds new unit test case for resource alicloud_hbr_oss_backup_plan alicloud_gpdb_account alicloud_hbr_ecs_backup_plan ([#4863](https://github.com/aliyun/terraform-provider-alicloud/issues/4863))
- testcases: Improves the alicloud_hbr_ecs_backup_plan testcases ([#4870](https://github.com/aliyun/terraform-provider-alicloud/issues/4870))
- GithubWorkFlow: pause the misspell workflow because of the different ownerships ([#4864](https://github.com/aliyun/terraform-provider-alicloud/issues/4864))

BUG FIXES:

- resource/alicloud_ess_alb_server_group_attachment: Fixes the resource not found error ([#4872](https://github.com/aliyun/terraform-provider-alicloud/issues/4872))
- resource/alicloud_cms_contact_group: Fixes the connection failed error; client: Fixes the SDK.CanNotResolveEndpoint error for CMS client and its resources ([#4852](https://github.com/aliyun/terraform-provider-alicloud/issues/4852))
- resource/alicloud_cms_alarm : Fixes the empty pointer error ([#4862](https://github.com/aliyun/terraform-provider-alicloud/issues/4862))
- resource/alicloud_elasticsearch_instance: fix the type convert error ([#4845](https://github.com/aliyun/terraform-provider-alicloud/issues/4845))
- testcase: Fixes cs kubernetes resource testcases ([#4849](https://github.com/aliyun/terraform-provider-alicloud/issues/4849))

## 1.163.0 (April 10, 2022)

- **New Resource:** `alicloud_alb_listener_acl_attachment` ([#4816](https://github.com/aliyun/terraform-provider-alicloud/issues/4816))
- **New Resource:** `alicloud_alikafka_instance_allowed_ip_attachment` ([#4781](https://github.com/aliyun/terraform-provider-alicloud/issues/4781))
- **New Resource:** `alicloud_ecs_image_pipeline` ([#4798](https://github.com/aliyun/terraform-provider-alicloud/issues/4798))
- **New Resource:** `alicloud_slb_server_group_server_attachment` ([#4814](https://github.com/aliyun/terraform-provider-alicloud/issues/4814))
- **New Resource:** `alicloud_hbr_ots_backup_plan` ([#4831](https://github.com/aliyun/terraform-provider-alicloud/issues/4831))
- **New Data Source:** `alicloud_hbr_ots_backup_plans` ([#4831](https://github.com/aliyun/terraform-provider-alicloud/issues/4831))	
- **New Data Source:** `alicloud_ecs_image_pipelines` ([#4798](https://github.com/aliyun/terraform-provider-alicloud/issues/4798))
- **New Data Source:** `alicloud_cen_transit_router_available_resources` ([#4800](https://github.com/aliyun/terraform-provider-alicloud/issues/4800))
- **New Data Source:** `alicloud_ecs_image_support_instance_types` ([#4798](https://github.com/aliyun/terraform-provider-alicloud/issues/4798))

ENHANCEMENTS:

- Updates the go dependence packages ([#4843](https://github.com/aliyun/terraform-provider-alicloud/issues/4843))
- datasource/alicloud_kvstore_instances: Fix auto_renew return value is incorrect ([#4842](https://github.com/aliyun/terraform-provider-alicloud/issues/4842))
- sdk/alibaba-cloud-go-sdk: Upgrades the sdk to v1.61.1538 ([#4840](https://github.com/aliyun/terraform-provider-alicloud/issues/4840))
- resource/alicloud_emr_cluster: Updates its dependence SDK. ([#4836](https://github.com/aliyun/terraform-provider-alicloud/issues/4836))
- resource/alicloud_config_aggregator: reset the correct http method ([#4838](https://github.com/aliyun/terraform-provider-alicloud/issues/4838))
- resource/alicloud_elasticsearch_instance:support for updating kibana node specifications with kibana_node_spec ([#4591](https://github.com/aliyun/terraform-provider-alicloud/issues/4591))
- resource/alicloud_ess_scalinggroup_vserver_groups : Updates its dependence SDK ([#4833](https://github.com/aliyun/terraform-provider-alicloud/issues/4833))
- resource/alicloud_ddoscoo_instance: Updates its dependence SDK. ([#4834](https://github.com/aliyun/terraform-provider-alicloud/issues/4834))
- resource/alicloud_click_house_account: Support updating the account authority configuration ([#4809](https://github.com/aliyun/terraform-provider-alicloud/issues/4809))
- resource/alicloud_ddoscoo_instances: Updates its dependence SDK. Optimize documentation. ([#4823](https://github.com/aliyun/terraform-provider-alicloud/issues/4823))
- resource/alicloud_cms_alarm: supports timeouts setting. Updates its dependence SDK. ([#4826](https://github.com/aliyun/terraform-provider-alicloud/issues/4826))
- resource/alicloud_ga_listener: Optimize the update logic for certificates attributes ([#4813](https://github.com/aliyun/terraform-provider-alicloud/issues/4813))
- resource/alicloud_slb_rule: Updates its dependence SDK. supports delete timeouts setting ([#4820](https://github.com/aliyun/terraform-provider-alicloud/issues/4820))
- resource/click_house_db_cluster: Update optional values for db_cluster_version attributes. ([#4806](https://github.com/aliyun/terraform-provider-alicloud/issues/4806))
- resource/mongodb_instance: Wait for the running status before updating the resource_group_id attribute ([#4804](https://github.com/aliyun/terraform-provider-alicloud/issues/4804))
- resource/security_center_group: Add timeout retry condition; supports timeouts setting ([#4802](https://github.com/aliyun/terraform-provider-alicloud/issues/4802))
- resource/security_center_service_linked_role: Add timeout retry condition; supports delete timeouts setting ([#4802](https://github.com/aliyun/terraform-provider-alicloud/issues/4802))
- resource/alicloud_lindorm_instance: Optimize instance update logic ([#4801](https://github.com/aliyun/terraform-provider-alicloud/issues/4801))
- resource/alicloud_mongodb_audit_policy: Enlarges the creating and updating default timeout ([#4810](https://github.com/aliyun/terraform-provider-alicloud/issues/4810))
- resource/alicloud_alb_listener_additional_certificate_attachment: Added error retry codes ResourceInConfiguring.Listener, IncorrectStatus.Listener ([#4796](https://github.com/aliyun/terraform-provider-alicloud/issues/4796))
- resource/mongodb_sharding_instance: Wait for the running status before updating the resource_group_id attribute ([#4804](https://github.com/aliyun/terraform-provider-alicloud/issues/4804))
- resource/alicloud_slb_backend_server: add the retry code during the delete ([#4817](https://github.com/aliyun/terraform-provider-alicloud/issues/4817))	
- datasource/alicloud_ddoscoo_instances: Updates its dependence SDK. ([#4828](https://github.com/aliyun/terraform-provider-alicloud/issues/4828))
- datasource/alicloud_kvstore_instances: Updates its dependence SDK. ([#4837](https://github.com/aliyun/terraform-provider-alicloud/issues/4837))	
- datasource/emr_main_versions: Updates its dependence SDK. ([#4827](https://github.com/aliyun/terraform-provider-alicloud/issues/4827))
- datasource/alicloud_ecs_network_interfaces: support the field associated_public_ip ([#4817](https://github.com/aliyun/terraform-provider-alicloud/issues/4817))	
- testcase: Adds new unit test case for resource alicloud_cloud_firewall_control_policy_order alicloud_cloud_firewall_instance alicloud_cms_metric_rule_template ([#4792](https://github.com/aliyun/terraform-provider-alicloud/issues/4792))
- testcase: Adds new unit test case for resource alicloud_config_aggregate_config_rule alicloud_ddoscoo_domain_resource alicloud_ddoscoo_port ([#4799](https://github.com/aliyun/terraform-provider-alicloud/issues/4799))
- testcase: Adds new unit test case for resource alicloud_config_rule alicloud_config_delivery_channel alicloud_config_compliance_pack ([#4672](https://github.com/aliyun/terraform-provider-alicloud/issues/4672))
- testcase: Adds new unit test case for resource alicloud_direct_mail_mail_address alicloud_dfs_mount_point alicloud_direct_mail_domain ([#4812](https://github.com/aliyun/terraform-provider-alicloud/issues/4812))
- testcase: Adds new unit test case for resource alicloud_dfs_file_system alicloud_dfs_access_group alicloud_dfs_access_rule ([#4805](https://github.com/aliyun/terraform-provider-alicloud/issues/4805))
- testcase: Improves the gpdb and clickhoust testcases ([#4811](https://github.com/aliyun/terraform-provider-alicloud/issues/4811))
- testcases: Improves the alicloud_ddoscoo_domain_resource testcases ([#4819](https://github.com/aliyun/terraform-provider-alicloud/issues/4819))
- sdk/alibaba-cloud-go-sdk: Upgrades the sdk to v1.61.1538 ([#4840](https://github.com/aliyun/terraform-provider-alicloud/issues/4840))

BUG FIXES:

- resource/click_house_account: Fix test cases; supports timeouts setting ([#4806](https://github.com/aliyun/terraform-provider-alicloud/issues/4806))
- resource/alicloud_slb_acl: Fixes the Throlling.User error by adding retry ([#4832](https://github.com/aliyun/terraform-provider-alicloud/issues/4832))

## 1.162.0 (March 27, 2022)

- **New Resource:** `alicloud_vpn_pbr_route_entry` ([#4759](https://github.com/aliyun/terraform-provider-alicloud/issues/4759))
- **New Resource:** `alicloud_slb_acl_entry_attachment` ([#4771](https://github.com/aliyun/terraform-provider-alicloud/issues/4771))
- **New Resource:** `alicloud_mse_znode` ([#4757](https://github.com/aliyun/terraform-provider-alicloud/issues/4757))
- **New Resource:** `alicloud_log_resource` ([#4786](https://github.com/aliyun/terraform-provider-alicloud/issues/4786))
- **New Data Source:** `alicloud_log_resource_record` ([#4786](https://github.com/aliyun/terraform-provider-alicloud/issues/4786))	
- **New Data Source:** `alicloud_mse_znodes` ([#4757](https://github.com/aliyun/terraform-provider-alicloud/issues/4757))	
- **New Data Source:** `alicloud_vpn_pbr_route_entries` ([#4759](https://github.com/aliyun/terraform-provider-alicloud/issues/4759))

ENHANCEMENTS:

- resource/alicloud_sae_application: fix the convert error with the field enable_grey_tag_route ([#4794](https://github.com/aliyun/terraform-provider-alicloud/issues/4794))
- resource/alicloud_kvstore_connection: Enlarges the creating default timeout ([#4783](https://github.com/aliyun/terraform-provider-alicloud/issues/4783))
- resource/alicloud_mse_cluster: Add support for output parameters cluster_id. ([#4757](https://github.com/aliyun/terraform-provider-alicloud/issues/4757))
- resource/alicloud_log_etl: removed sls etl test update fromTime toTime and updated doc ([#4775](https://github.com/aliyun/terraform-provider-alicloud/issues/4775))
- resource/alicloud_kvstore_instance: Removes the default value and adds computed ([#4778](https://github.com/aliyun/terraform-provider-alicloud/issues/4778))
- resource/alicloud_kvstore_connection: Enlarges the deleting default timeout ([#4778](https://github.com/aliyun/terraform-provider-alicloud/issues/4778))	
- resource/alicloud_sae_application: update the issue that creating the resource with two deployment ([#4777](https://github.com/aliyun/terraform-provider-alicloud/issues/4777))
- resource/alicloud_dts_job_monitor_rule: Removes the attribute phone Computed setting ([#4766](https://github.com/aliyun/terraform-provider-alicloud/issues/4766))
- resource/alicloud_fnf_execution: update the target status after creating. resource/alicloud_cms_alarm: update the eneum value abourt the field escalations_warn escalations_info ([#4764](https://github.com/aliyun/terraform-provider-alicloud/issues/4764))
- resource/alicloud_actiontrail_history_delivery_job: Adds 1 minute sleep after deleting it to ensure ensure it has been destroy completely ([#4762](https://github.com/aliyun/terraform-provider-alicloud/issues/4762))
- resource/alicloud_dbfs_instance: Enlarges the delete default timeout ([#4761](https://github.com/aliyun/terraform-provider-alicloud/issues/4761))
- resource/alicloud_cen_instance: Enlarges the deleting default timeout to 10min ([#4774](https://github.com/aliyun/terraform-provider-alicloud/issues/4774))
- datasource/alicloud_cen_private_zones: Improves the ids element value and use resource id instead ([#4774](https://github.com/aliyun/terraform-provider-alicloud/issues/4774))
- datasource/alicloud_alb_rules: Adds output variable rule_actions.traffic_limit_config, rule_actions.traffic_mirror_config and rule_conditions.source_ip_config. resource/alicloud_alb_rule: Support for new parameters rule_actions.traffic_limit_config, rule_actions.traffic_mirror_config and rule_conditions.source_ip_config. ([#4773](https://github.com/aliyun/terraform-provider-alicloud/issues/4773))	
- testcase: Improves the yundun dbaudit sweeper testcase ([#4795](https://github.com/aliyun/terraform-provider-alicloud/issues/4795))
- testcase: Adds new unit test case for resource alicloud_alidns_access_strategy alicloud_alidns_instance alicloud_alidns_monitor_config ([#4760](https://github.com/aliyun/terraform-provider-alicloud/issues/4760))
- testcase: Adds new unit test case for resource testcase: alicloud_config_aggregator alicloud_resource_manager_policy_attachment alicloud_resource_manager_policy ([#4645](https://github.com/aliyun/terraform-provider-alicloud/issues/4645))
- testcase: Adds new unit test case for resource alicloud_brain_industrial_pid_loop alicloud_alidns_gtm_instance alicloud_alikafka_sasl_use ([#4765](https://github.com/aliyun/terraform-provider-alicloud/issues/4765))	
- testcase: Improves the cen and cloud_storage_gateway_express_sync_share_attachment testcases ([#4789](https://github.com/aliyun/terraform-provider-alicloud/issues/4789))	
- testcase: Improve the resource alicloud_cloud_storage_gateway_gateway_file_share unit testcase ([#4787](https://github.com/aliyun/terraform-provider-alicloud/issues/4787))	
- testcase: Adds new unit test case for resource alicloud_click_house_backup_policy alicloud_cddc_dedicated_host alicloud_cddc_dedicated_host_account ([#4775](https://github.com/aliyun/terraform-provider-alicloud/issues/4775))
- docs: Adds a note for resource/alicloud_cddc_dedicated_host_group to mark sqlServer does not support setting disk_allocation_ratio ([#4763](https://github.com/aliyun/terraform-provider-alicloud/issues/4763))
- docs: Add region support for alicloud_log_resource and alicloud_log_resource_record ([#4790](https://github.com/aliyun/terraform-provider-alicloud/issues/4790))	
- ci: Changes the all testcases running time ([#4754](https://github.com/aliyun/terraform-provider-alicloud/issues/4754))

BUG FIXES:

- resource/alicloud_cs_serverless_kubernetes: Support for creating professional serverless cluster ([#4768](https://github.com/aliyun/terraform-provider-alicloud/issues/4768))
- resource/alicloud_alb_load_balancer: Fixes the updating load_balancer_edition not effect bug ([#4780](https://github.com/aliyun/terraform-provider-alicloud/issues/4780))
- resource/alicloud_cms_monitor_group_instances: Fix the problem of page turning of query interface data ([#4770](https://github.com/aliyun/terraform-provider-alicloud/issues/4770))
- resource/alicloud_yundun_bastionhost: Fixes the InvalidApi error while invoking DescribeInstanceAttribute ([#4767](https://github.com/aliyun/terraform-provider-alicloud/issues/4767))
- resource/alicloud_cen_instance_attachment: Fixes the InstanceStatus.NotSupport error while invoking DetachCenChildInstance ([#4758](https://github.com/aliyun/terraform-provider-alicloud/issues/4758))
- resource/alicloud_gpdb_instance: Fixes the InternalError while deleting this resource ([#4753](https://github.com/aliyun/terraform-provider-alicloud/issues/4753))
- datasource/alicloud_vpcs: Fixes the vpc is not found because of it does not return system route table ([#4756](https://github.com/aliyun/terraform-provider-alicloud/issues/4756))
- datasource/alicloud_cdn_service: fix the service enable error ([#4772](https://github.com/aliyun/terraform-provider-alicloud/issues/4772))
- testcase:Fix alicloud_dts_synchronization_instance test case ([#4731](https://github.com/aliyun/terraform-provider-alicloud/issues/4731))

## 1.161.0 (March 20, 2022)

- **New Resource:** `alicloud_oss_bucket_replication` ([#4684](https://github.com/aliyun/terraform-provider-alicloud/issues/4684))
- **New Resource:** `alicloud_cr_chain` ([#4696](https://github.com/aliyun/terraform-provider-alicloud/issues/4696))	
- **New Resource:** `alicloud_log_ingestion` ([#4623](https://github.com/aliyun/terraform-provider-alicloud/issues/4623))
- **New Resource:** `alb_listener_additional_certificate_attachment` ([#4694](https://github.com/aliyun/terraform-provider-alicloud/issues/4694))
- **New Resource:** `alicloud_vpn_ipsec_server` ([#4705](https://github.com/aliyun/terraform-provider-alicloud/issues/4705))
- **New Data Source:** `alicloud_log_alert_resource` ([#4658](https://github.com/aliyun/terraform-provider-alicloud/issues/4658))
- **New Data Source:** `alicloud_vpn_ipsec_servers` ([#4705](https://github.com/aliyun/terraform-provider-alicloud/issues/4705))	
- **New Data Source:** `alicloud_dms_user_tenants` ([#4709](https://github.com/aliyun/terraform-provider-alicloud/issues/4709))
- **New Data Source:** `alicloud_cr_chains` ([#4696](https://github.com/aliyun/terraform-provider-alicloud/issues/4696))
- **New Data Source:** `alicloud_service_mesh_versions` ([#4745](https://github.com/aliyun/terraform-provider-alicloud/issues/4745))

ENHANCEMENTS:

- resource/alicloud_nas_mount_target: add the attribute mount_target_domain resource/alicloud_sae_application: fix the issue of updating the package_version ([#4750](https://github.com/aliyun/terraform-provider-alicloud/issues/4750))
- resource/alicloud_ga_additional_certificate: Waiting the accelerator and listener to be active after creating or deleting additional certificate ([#4748](https://github.com/aliyun/terraform-provider-alicloud/issues/4748))
- resource/alicloud_ssl_certificates_service_certificate: Adds StateRefreshFunc to ensure the resource has been deleted after running destroy ([#4744](https://github.com/aliyun/terraform-provider-alicloud/issues/4744))
- resource/alicloud_sae_application: Support field min_ready_instance_ratio ([#4707](https://github.com/aliyun/terraform-provider-alicloud/issues/4707))
- resource/alicloud_mongodb_instance: Support for new parameters network_type, vpc_id and resource_group_id; Updates its dependence SDK. ([#4737](https://github.com/aliyun/terraform-provider-alicloud/issues/4737))
- resource/alicloud_vpn_connection: change sdk to common api;Support for new parameters health_check_config, enable_dpd, enable_nat_traversal, bgp_config ([#4717](https://github.com/aliyun/terraform-provider-alicloud/issues/4717))
- resource/alicloud_hbr_vaule: add the field redundancy_type ([#4735](https://github.com/aliyun/terraform-provider-alicloud/issues/4735))
- resource/alicloud_log_alert: Update Resource ([#4658](https://github.com/aliyun/terraform-provider-alicloud/issues/4658))
- resource/alicloud_cen_route_map: Adds a output attribute route_map_id ([#4736](https://github.com/aliyun/terraform-provider-alicloud/issues/4736))
- resource/alicloud_vpc_bgp_network: Enlarges the create default timeout to 3min ([#4736](https://github.com/aliyun/terraform-provider-alicloud/issues/4736))
- resource/alicloud_polardb_endpoint: Add support for output parameters db_endpoint_id. ([#4726](https://github.com/aliyun/terraform-provider-alicloud/issues/4726))
- resource/alicloud_msc_sub_subscription: Update contact_ids type to a set to avoid potential diff error ([#4727](https://github.com/aliyun/terraform-provider-alicloud/issues/4727))
- resource/alicloud_cddc_dedicated_host_account: Adds wait after creating the resource to avoid notfounderror; Improves the testcases ([#4724](https://github.com/aliyun/terraform-provider-alicloud/issues/4724))
- resource/alb_listener: Optimize XForward field ([#4694](https://github.com/aliyun/terraform-provider-alicloud/issues/4694))	
- resource/alicloud_vpn_route_entry: change sdk to common api;Support for new parameters route_entry_type, status ([#4703](https://github.com/aliyun/terraform-provider-alicloud/issues/4703))
- resource/alicloud_ddoscoo_domain_resource: Update the attribute instance_ids type to a set to avoid protential diff error ([#4704](https://github.com/aliyun/terraform-provider-alicloud/issues/4704))
- resource/alicloud_alikafka_instance: Supports to update attribute deploy_type ([#4691](https://github.com/aliyun/terraform-provider-alicloud/issues/4691))
- resource/alicloud_mongodb_sharding_instance: Support for new parameters network_type, vpc_id, protocol_type and resource_group_id; Updates its dependence SDK. ([#4650](https://github.com/aliyun/terraform-provider-alicloud/issues/4650))
- resource/resource_alicloud_log_store, resource_alicloud_log_audit ([#4667](https://github.com/aliyun/terraform-provider-alicloud/issues/4667))
- resource/alicloud_open_search_app_group: Adds a output attribute instance_id ([#4701](https://github.com/aliyun/terraform-provider-alicloud/issues/4701))
- resource/alicloud_msc_sub_subscription: Optimize the handling of creating return values ([#4695](https://github.com/aliyun/terraform-provider-alicloud/issues/4695))
- datasource/alicloud_simple_application_server_images: Supports new parameter platform ([#4715](https://github.com/aliyun/terraform-provider-alicloud/issues/4715))
- datasource/alicloud_simple_application_server_plans: Supports new parameter platform ([#4715](https://github.com/aliyun/terraform-provider-alicloud/issues/4715))
- datasource/alicloud_cr_ee_namespace: Adds two outputs namespace_name and namespace_id; Improves the ids values ([#4730](https://github.com/aliyun/terraform-provider-alicloud/issues/4730))
- data_source/alicloud_vpn_gateways: Adds new parameter enable_ipsec. ([#4705](https://github.com/aliyun/terraform-provider-alicloud/issues/4705))	
- datasource/alicloud_cen_route_maps: Improves the ids values ([#4736](https://github.com/aliyun/terraform-provider-alicloud/issues/4736))
- testcase: Resolve ram role and ram policy resources conflict against ([#4742](https://github.com/aliyun/terraform-provider-alicloud/issues/4742))	
- testcase: Adds new unit test case for resource alicloud_alikafka_consumer_group alicloud_cloud_storage_gateway_gateway_smb_user alicloud_cloud_storage_gateway_storage_bundle ([#4740](https://github.com/aliyun/terraform-provider-alicloud/issues/4740))
- testcase: Adds new unit test case for resource alicloud_cloud_storage_gateway_gateway_cache_disk alicloud_cloud_storage_gateway_gateway_file_share alicloud_cloud_storage_gateway_gateway_logging ([#4728](https://github.com/aliyun/terraform-provider-alicloud/issues/4728))	
- testcase: Adds new unit test case for resource alicloud_cloud_sso_access_assignment alicloud_bastionhost_user alicloud_bastionhost_host_group ([#4699](https://github.com/aliyun/terraform-provider-alicloud/issues/4699))
- testcase: Adds new unit test case for resource alicloud_bastionhost_user_attachment alicloud_cms_group_metric_rule alicloud_bastionhost_user_group ([#4708](https://github.com/aliyun/terraform-provider-alicloud/issues/4708))
- testcase: Adds new unit test case for resource alicloud_cloud_storage_gateway_gateway_block_volume alicloud_cloud_storage_gateway_express_sync_share_attachment alicloud_cloud_storage_gateway_express_sync ([#4719](https://github.com/aliyun/terraform-provider-alicloud/issues/4719))	
- testcase: Improves the eci resource testcases ([#4692](https://github.com/aliyun/terraform-provider-alicloud/issues/4692))
- testcase: Improves the mse gateway testcases ([#4693](https://github.com/aliyun/terraform-provider-alicloud/issues/4693))
- testcase: Improves the cen resource testcases ([#4698](https://github.com/aliyun/terraform-provider-alicloud/issues/4698))
- testcase: Improves the acr ee testcases ([#4702](https://github.com/aliyun/terraform-provider-alicloud/issues/4702))
- testcase: Improve cen_vbr_health_checks testcase; Adds sweeper test for vbr ([#4706](https://github.com/aliyun/terraform-provider-alicloud/issues/4706))
- testcase: Improves the dms testcases; Improves the eais testcase ([#4709](https://github.com/aliyun/terraform-provider-alicloud/issues/4709))
- testcase: Improve the yundun dbaudit testcases ([#4713](https://github.com/aliyun/terraform-provider-alicloud/issues/4713))
- testcase: Improves the several testcases ([#4714](https://github.com/aliyun/terraform-provider-alicloud/issues/4714))
- testcases: Improves the cen resource testcases ([#4738](https://github.com/aliyun/terraform-provider-alicloud/issues/4738))	
- docs/alicloud_hbr_vaults: document optimization ([#4697](https://github.com/aliyun/terraform-provider-alicloud/issues/4697))
- docs/alikafka_instance.html.markdown: format demo	([#4667](https://github.com/aliyun/terraform-provider-alicloud/issues/4667))
- credential: oss resources supports more ways to enter credentials for authentication for oss. ([#4723](https://github.com/aliyun/terraform-provider-alicloud/issues/4723))

BUG FIXES:

- resource/alicloud_cen_instance: Fixes the InvalidOperation.CenInstanceStatus error while deleting the resource ([#4752](https://github.com/aliyun/terraform-provider-alicloud/issues/4752))
- resource/alicloud_ecd_simple_office_site: Fixes the DesktopAccessTypeNotChanged when invoking the ModifyOfficeSiteAttribute ([#4751](https://github.com/aliyun/terraform-provider-alicloud/issues/4751))
- resource/alicloud_ddoscoo_instance: Fixes the Throttling.User error while invoking the DescribeInstanceSpecs ([#4749](https://github.com/aliyun/terraform-provider-alicloud/issues/4749))
- resource/alicloud_eipanycast_address_attachment: Fixes the InvalidRegionId error when descring eipanycast endpoint ([#4718](https://github.com/aliyun/terraform-provider-alicloud/issues/4718))
- resource/alicloud_ga_ip_set: Fixes the MissingIpSetIds error while deleting this resource ([#4741](https://github.com/aliyun/terraform-provider-alicloud/issues/4741))
- resource/alicloud_oos_parameter: Fixes the description value is empty after updating other attributes ([#4743](https://github.com/aliyun/terraform-provider-alicloud/issues/4743))
- resource/alicloud_cen_route_map: Fixes the InternalError when creating this resource ([#4739](https://github.com/aliyun/terraform-provider-alicloud/issues/4739))
- resource/alicloud_cen_route_map: Fixes the MissingParameter error because of missing DestinationCidrBlocks when invoking ModifyCenRouteMap ([#4729](https://github.com/aliyun/terraform-provider-alicloud/issues/4729))
- resource/alicloud_mongodb_audit_policy:Fix test cases; supports timeouts setting. ([#4716](https://github.com/aliyun/terraform-provider-alicloud/issues/4716))
- resource/alicloud_msc_sub_webhook,alicloud_alb_listener_additional_certificate_attachment: Fix test case bugs ([#4722](https://github.com/aliyun/terraform-provider-alicloud/issues/4722))
- reource/alicloud_rds_account: Fixes the retry implementation bug to fix Throttling error ([#4714](https://github.com/aliyun/terraform-provider-alicloud/issues/4714))
- resource/alicloud_ddoscoo_port: Fixes the anycast_controller3006 error when the resource has been deleted ([#4704](https://github.com/aliyun/terraform-provider-alicloud/issues/4704))
- resource/vpc_traffic_mirror_session: Fix test cases ([#4683](https://github.com/aliyun/terraform-provider-alicloud/issues/4683))
- resource/alicloud_ga_bandwidth_package_attachment: Fixes the StateError.Accelerator error while creating it; Improves the ga testcases and adds sweeper testcase ([#4700](https://github.com/aliyun/terraform-provider-alicloud/issues/4700))
- reource/alicloud_nas_file_system: Fixes the retry implementation bug to fix Throttling.Api error ([#4711](https://github.com/aliyun/terraform-provider-alicloud/issues/4711))
- resource/alicloud_drds_instance: Fixes the InternalError by adding retry implementation ([#4712](https://github.com/aliyun/terraform-provider-alicloud/issues/4712))
- datasource/alicloud_gpdb_accounts: Fixes the filter error by param status; Improves the testcases ([#4710](https://github.com/aliyun/terraform-provider-alicloud/issues/4710))
- datasource/alicloud_sae_applications: fix the type mount_desc issue ([#4707](https://github.com/aliyun/terraform-provider-alicloud/issues/4707))
- datasource/data_source_alicloud_log_projects:bug fix ([#4667](https://github.com/aliyun/terraform-provider-alicloud/issues/4667))
- datasource/alicloud_bastionhost_instances: Fiexes the Throttling.User error by adding retry implementation ([#4720](https://github.com/aliyun/terraform-provider-alicloud/issues/4720))
- datasource/vpc_traffic_mirror_sessions: Fix test cases ([#4683](https://github.com/aliyun/terraform-provider-alicloud/issues/4683))

## 1.160.0 (March 13, 2022)

- **New Resource:** `alicloud_sae_grey_tag_route` ([#4644](https://github.com/aliyun/terraform-provider-alicloud/issues/4644))
- **New Resource:** `alicloud_ecs_snapshot_group` ([#4666](https://github.com/aliyun/terraform-provider-alicloud/issues/4666))
- **New Data Source:** `alicloud_ecs_snapshot_groups` ([#4666](https://github.com/aliyun/terraform-provider-alicloud/issues/4666))	
- **New Data Source:** `alicloud_sae_grey_tag_routes` ([#4644](https://github.com/aliyun/terraform-provider-alicloud/issues/4644))

ENHANCEMENTS:

- resource/alicloud_lindorm_instance: Enlarges the its default creating timeout ([#4688](https://github.com/aliyun/terraform-provider-alicloud/issues/4688))
- resource/alicloud_mongodb_sharding_instance: Supports to update attribute tde_status ([#4686](https://github.com/aliyun/terraform-provider-alicloud/issues/4686))
- resource/alicloud_mongodb_instance: Adds retry for invoking DescribeDBInstanceAttribute and ResetPassword ([#4682](https://github.com/aliyun/terraform-provider-alicloud/issues/4682))
- resource/alicloud_adb_cluster: Adds retry for invoking DescribeTaskInfo ([#4678](https://github.com/aliyun/terraform-provider-alicloud/issues/4678))
- resource/alicloud_instance: Adds checking empty before setting period to avoid an invalid value 0 ([#4671](https://github.com/aliyun/terraform-provider-alicloud/issues/4671))
- resource/alicloud_vpn_customer_gateway: change sdk to common api;Support for new parameter asn ([#4669](https://github.com/aliyun/terraform-provider-alicloud/issues/4669))
- resource/alicloud_vpn_gateway: change sdk to common api;Support for new parameters auto_pay, tags ([#4656](https://github.com/aliyun/terraform-provider-alicloud/issues/4656))
- resource/alicloud_ess_scaling_group: Add support for new parameter tags ([#4648](https://github.com/aliyun/terraform-provider-alicloud/issues/4648))
- resource/cloud_firewall_instance: Add Support for the international site ([#4655](https://github.com/aliyun/terraform-provider-alicloud/issues/4655))
- resource/alicloud_gpdb_instance: Enlarges the default creating timeout ([#4665](https://github.com/aliyun/terraform-provider-alicloud/issues/4665))
- datasource/alicloud_ess_scalinggroups: Add support for new parameter tags ([#4648](https://github.com/aliyun/terraform-provider-alicloud/issues/4648))	
- testcase: Adds new unit test case for resource alicloud_cloud_sso_user alicloud_cloud_sso_group alicloud_cloud_sso_scim_server_credential ([#4680](https://github.com/aliyun/terraform-provider-alicloud/issues/4680))
- testcase: Improves the slb resources testcase ([#4681](https://github.com/aliyun/terraform-provider-alicloud/issues/4681))	
- testcase: Adds SDK error status code for resource testcase ([#4649](https://github.com/aliyun/terraform-provider-alicloud/issues/4649))
- testcase: Improves the cen instance unit test ([#4657](https://github.com/aliyun/terraform-provider-alicloud/issues/4657))
- docs/alicloud_hbr_nas_backup_plan: document optimization ([#4663](https://github.com/aliyun/terraform-provider-alicloud/issues/4663))
- docs/alicloud_hbr_ecs_backup_plan: document optimization ([#4664](https://github.com/aliyun/terraform-provider-alicloud/issues/4664))
- docs/alicloud_hbr_nas_backup_plans,alicloud_hbr_oss_backup_plans: doc ([#4661](https://github.com/aliyun/terraform-provider-alicloud/issues/4661))
- docs/alicloud_hbr_restore_jobs: document optimization ([#4660](https://github.com/aliyun/terraform-provider-alicloud/issues/4660))
- docs/alicloud_hbr_snapshots: document optimization ([#4659](https://github.com/aliyun/terraform-provider-alicloud/issues/4659))
- docs/alicloud_hbr_backup_jobs: document optimization ([#4662](https://github.com/aliyun/terraform-provider-alicloud/issues/4662))

BUG FIXES:

- resource/alicloud_dcdn_domain: Fixes the wait timeout error when offline the domain ([#4690](https://github.com/aliyun/terraform-provider-alicloud/issues/4690))
- resource/alicoud_mongodb_audit_policy: Fixes the OperationDenied.DBInstanceStatus error when creating or updating this resource ([#4685](https://github.com/aliyun/terraform-provider-alicloud/issues/4685))
- resource/alicloud_ecs_disk: Fixes the DiskNotPortable error while modifying disk payment type ([#4673](https://github.com/aliyun/terraform-provider-alicloud/issues/4673))
- resource/alicloud_event_bridge_rule: Fixes the diff error which caused by system default value ([#4679](https://github.com/aliyun/terraform-provider-alicloud/issues/4679))
- resource/alicloud_hbase_instance: Fixes the Instance.InvalidStatus error while deleting it ([#4675](https://github.com/aliyun/terraform-provider-alicloud/issues/4675))
- resource/resource_alicloud_express_connect_virtual_border_router: Fixes the DependencyViolation.BgpGroup error when deleting the resource ([#4670](https://github.com/aliyun/terraform-provider-alicloud/issues/4670))
- resource/alicloud_gpdb_elastic_instance: Fixes the IncorrectDBState error while deleting the resource ([#4665](https://github.com/aliyun/terraform-provider-alicloud/issues/4665))
- testcases: Fixes the resource testcase bug ([#4665](https://github.com/aliyun/terraform-provider-alicloud/issues/4665))
- testcase: Fix the unit for resource testcase ([#4652](https://github.com/aliyun/terraform-provider-alicloud/issues/4652))
- testcase: Fix the unit for resource testcase:alicloud_ga_ip_set ([#4654](https://github.com/aliyun/terraform-provider-alicloud/issues/4654))

## 1.159.0 (March 06, 2022)

- **New Resource:** `alicloud_sddp_data_limit` ([#4622](https://github.com/aliyun/terraform-provider-alicloud/issues/4622))
- **New Resource:** `alicloud_ecs_image_component` ([#4630](https://github.com/aliyun/terraform-provider-alicloud/issues/4630))
- **New Resource:** `alicloud_sea_application_scaling_rule` ([#4624](https://github.com/aliyun/terraform-provider-alicloud/issues/4624))
- **New Data Source:** `alicloud_sea_application_scaling_rules` ([#4624](https://github.com/aliyun/terraform-provider-alicloud/issues/4624))
- **New Data Source:** `alicloud_ecs_image_components` ([#4630](https://github.com/aliyun/terraform-provider-alicloud/issues/4630))	
- **New Data Source:** `alicloud_sddp_data_limits` ([#4622](https://github.com/aliyun/terraform-provider-alicloud/issues/4622))

ENHANCEMENTS:

- resource/alicloud_alikafka_sasl_user: change sdk to common api;Support for new parameter type ([#4635](https://github.com/aliyun/terraform-provider-alicloud/issues/4635))
- resource/alicloud_ess_scaling_group: new parameter launch_template_version ([#4598](https://github.com/aliyun/terraform-provider-alicloud/issues/4598))
- resource/alicloud_dts_synchronization_instance: Add support for output parameters auto_start, auto_pay ([#4614](https://github.com/aliyun/terraform-provider-alicloud/issues/4614))
- resource/alicloud_ram_role: supports setting timeouts when creating and deleting ([#4631](https://github.com/aliyun/terraform-provider-alicloud/issues/4631))
- testcase: Adds new unit test case for resource testcase: alicloud_resource_manager_folder alicloud_resource_manager_handshake alicloud_ga_ip_set ([#4636](https://github.com/aliyun/terraform-provider-alicloud/issues/4636))
- testcase: Adds two method used to write unit test ([#4568](https://github.com/aliyun/terraform-provider-alicloud/issues/4568))
- testcase: Improve the effectiveness of test cases ([#4617](https://github.com/aliyun/terraform-provider-alicloud/issues/4617))
- testcase: Adds unit test for resource alicloud_arms_dispatch_rule ([#4642](https://github.com/aliyun/terraform-provider-alicloud/issues/4642))	
- Improves the retry strategy when the error is Throttling ([#4618](https://github.com/aliyun/terraform-provider-alicloud/issues/4618))
- Addes two method to improve unit testcase ([#4625](https://github.com/aliyun/terraform-provider-alicloud/issues/4625))
- errors: Checking NotFoundError by http status code ([#4641](https://github.com/aliyun/terraform-provider-alicloud/issues/4641))

BUG FIXES:

- resource/alicloud_datahub_project: Fix the updating project comment diff error ([#4640](https://github.com/aliyun/terraform-provider-alicloud/issues/4640))
- resource/alicloud_datahub_project: Fix the updating project comment diff error ([#4639](https://github.com/aliyun/terraform-provider-alicloud/issues/4639))
- resource/alicloud_ram_role: Fixes the Throttling.User error on ListPoliciesForRole ([#4637](https://github.com/aliyun/terraform-provider-alicloud/issues/4637))
- resource/alicloud_nat_gateway: fixes the TaskConflict error when there are multi nat gateways to create ([#4619](https://github.com/aliyun/terraform-provider-alicloud/issues/4619))

## 1.158.0 (February 27, 2022)

- **New Resource:** `alicloud_ess_alb_server_group_attachment` ([#4594](https://github.com/aliyun/terraform-provider-alicloud/issues/4594))
- **New Resource:** `alicloud_ecp_instance` ([#4588](https://github.com/aliyun/terraform-provider-alicloud/issues/4588))
- **New Resource:** `alicloud_dcdn_ipa_domain` ([#4600](https://github.com/aliyun/terraform-provider-alicloud/issues/4600))
- **New Data Source:** `alicloud_dcdn_ipa_domains` ([#4600](https://github.com/aliyun/terraform-provider-alicloud/issues/4600))	
- **New Data Source:** `alicloud_ecp_instances` ([#4588](https://github.com/aliyun/terraform-provider-alicloud/issues/4588))
- **New Data Source:** `alicloud_ecp_zones` ([#4588](https://github.com/aliyun/terraform-provider-alicloud/issues/4588))
- **New Data Source:** `alicloud_ecp_instance_types` ([#4588](https://github.com/aliyun/terraform-provider-alicloud/issues/4588))

ENHANCEMENTS:

- resource/alicloud_gpdb_elastic_instance: Add support for output parameters db_instance_category, encryption_type, encryption_key, tags ([#4608](https://github.com/aliyun/terraform-provider-alicloud/issues/4608))
- resource/pvtz_rule: add the query field bind_vpcs ([#4607](https://github.com/aliyun/terraform-provider-alicloud/issues/4607))
- resource/alb_load_balancer: add the query field dns_nam ([#4607](https://github.com/aliyun/terraform-provider-alicloud/issues/4607))	
- resource/alicloud_cs_kubernetes_node_pool: support to specify desired node size for node pool ([#4596](https://github.com/aliyun/terraform-provider-alicloud/issues/4596))
- datasource/ess_scalinggroups: Add support for output parameters vpc_id,vswitch_id,health_check_type,suspended_processes,group_deletion_protection,modification_time,total_instance_count ([#4603](https://github.com/aliyun/terraform-provider-alicloud/issues/4603))
- datasource/ecs_network_interfaces: Add support for output parameters network_interface_traffic_mode,owner_id ([#4603](https://github.com/aliyun/terraform-provider-alicloud/issues/4603))
- testcase: Improve the effectiveness of test cases ([#4554](https://github.com/aliyun/terraform-provider-alicloud/issues/4554))
- testcase: Adds new unit test case for resource alicloud_oos_patch_baseline alicloud_oos_parameter alicloud_oos_execution ([#4597](https://github.com/aliyun/terraform-provider-alicloud/issues/4597))
- testcase: Adds new unit test case for resource alicloud_oos_state_configuration alicloud_oos_service_setting alicloud_oos_secret_parameter ([#4601](https://github.com/aliyun/terraform-provider-alicloud/issues/4601))
- testcase: Adds new unit test case for resource alicloud_nas_access_rule alicloud_nas_access_group alicloud_oos_template ([#4604](https://github.com/aliyun/terraform-provider-alicloud/issues/4604))
- testcase: Adds new unit test case for resource alicloud_nas_fileset alicloud_nas_auto_snapshot_policy alicloud_nas_file_system ([#4609](https://github.com/aliyun/terraform-provider-alicloud/issues/4609))
- testcase: Adds new unit test case for resource alicloud_kms_key alicloud_nas_mount_target alicloud_nas_snapshot ([#4613](https://github.com/aliyun/terraform-provider-alicloud/issues/4613))	
- testcase: Improves the provider testcase when changing the supported regions ([#4610](https://github.com/aliyun/terraform-provider-alicloud/issues/4610))

BUG FIXES:

- resource/click_house_db_clusters: Fixed the difference error in the attribute db_cluster_access_white_list; Remove the db_cluster_ip_array_attribute attribute ([#4546](https://github.com/aliyun/terraform-provider-alicloud/issues/4546))
- testcase: fix CIDR block conflicts for resource alicloud_cs_kubernete ([#4606](https://github.com/aliyun/terraform-provider-alicloud/issues/4606))

## 1.157.0 (February 20, 2022)

- **New Resource:** `alicloud_dts_migration_job` ([#4572](https://github.com/aliyun/terraform-provider-alicloud/issues/4572))
- **New Resource:** `alicloud_mse_gateway` ([#4577](https://github.com/aliyun/terraform-provider-alicloud/issues/4577))
- **New Resource:** `alicloud_dts_migration_instance` ([#4572](https://github.com/aliyun/terraform-provider-alicloud/issues/4572))
- **New Resource:** `alicloud_ram_service_linked_role` ([#4590](https://github.com/aliyun/terraform-provider-alicloud/issues/4590))
- **New Resource:** `alicloud_mongodb_sharding_network_private_address` ([#4584](https://github.com/aliyun/terraform-provider-alicloud/issues/4584))
- **New Data Source:** `alicloud_mongodb_sharding_network_private_addresses` ([#4584](https://github.com/aliyun/terraform-provider-alicloud/issues/4584))
- **New Data Source:** `alicloud_mse_gateways` ([#4577](https://github.com/aliyun/terraform-provider-alicloud/issues/4577))	
- **New Data Source:** `alicloud_dts_migration_jobs` ([#4572](https://github.com/aliyun/terraform-provider-alicloud/issues/4572))

ENHANCEMENTS:

- resource/alicloud_cen_transit_router_peer_attachment: support updating bandwidth_type with DataTransfer ([#4590](https://github.com/aliyun/terraform-provider-alicloud/issues/4590))
- resource/alicloud_alikafka_consumer_group: change sdk to common api;Support for new parameter description ([#4583](https://github.com/aliyun/terraform-provider-alicloud/issues/4583))
- datasource/alicloud_slb_zones: Adds new parameter master_zone_id and slave_zone_id; Deprecates tehe output slb_slave_zone_ids ([#4593](https://github.com/aliyun/terraform-provider-alicloud/issues/4593))	
- testcase: Adds new unit test case for resource alicloud_actiontrail_history_delivery_job alicloud_actiontrail_trail alicloud_cr_endpoint_acl_policy ([#4576](https://github.com/aliyun/terraform-provider-alicloud/issues/4576))
- testcase: Adds new unit test case for resource alicloud_cloud_firewall_control_policy alicloud_security_center_group alicloud_security_center_service_linked_role ([#4580](https://github.com/aliyun/terraform-provider-alicloud/issues/4580))
- testcase: Adds new unit test case for resource alicloud_arms_alert_contact alicloud_arms_alert_contact_group alicloud_arms_prometheus_alert_rule ([#4585](https://github.com/aliyun/terraform-provider-alicloud/issues/4585))
- testcase: Adds new unit test case for resource alicloud_pvtz_rule_attachment alicloud_pvtz_rule alicloud_pvtz_endpoint ([#4589](https://github.com/aliyun/terraform-provider-alicloud/issues/4589))
- testcase: Adds new unit test case for resource alicloud_oos_application_group alicloud_oos_application alicloud_pvtz_user_vpc_authorization ([#4592](https://github.com/aliyun/terraform-provider-alicloud/issues/4592))

BUG FIXES:

- datasource/alicloud_bastionhost_host_account: Fixed the not found error returned by the query after the resource was deleted ([#4576](https://github.com/aliyun/terraform-provider-alicloud/issues/4576))
- datasource/alicloud_bastionhost_host: Fixed the not found error returned by the query after the resource was deleted ([#4576](https://github.com/aliyun/terraform-provider-alicloud/issues/4576))

## 1.156.0 (February 15, 2022)

- **New Resource:** `alicloud_dbfs_snapshot` ([#4553](https://github.com/aliyun/terraform-provider-alicloud/issues/4553))
- **New Resource:** `alicloud_dbfs_instance_attachment` ([#4553](https://github.com/aliyun/terraform-provider-alicloud/issues/4553))
- **New Data Source:** `alicloud_msc_sub_contact_verification_message` ([#4569](https://github.com/aliyun/terraform-provider-alicloud/issues/4569))	
- **New Data Source:** `alicloud_dbfs_snapshots` ([#4553](https://github.com/aliyun/terraform-provider-alicloud/issues/4553))

BUG FIXES:

- resource/alicloud_db_instance: fix the error of the type convertion ([#4573](https://github.com/aliyun/terraform-provider-alicloud/issues/4573))
- resource/alicloud_db_instance, alicloud_rds_clone_db_instance, alicloud_rds_upgrade_db_instance pg_hba_conf bug fix ([#4575](https://github.com/aliyun/terraform-provider-alicloud/issues/4575))

## 1.155.0 (February 13, 2022)

- **New Resource:** `alicloud_ecs_storage_capacity_unit` ([#4562](https://github.com/aliyun/terraform-provider-alicloud/issues/4562))
- **New Resource:** `alicloud_nas_recycle_bin` ([#4556](https://github.com/aliyun/terraform-provider-alicloud/issues/4556))	
- **New Data Source:** `alicloud_ecs_storage_capacity_units` ([#4562](https://github.com/aliyun/terraform-provider-alicloud/issues/4562))

ENHANCEMENTS:

- resource/alicloud_db_instance add new Attribute pg_hba_conf to support pgsql AD domain ([#4547](https://github.com/aliyun/terraform-provider-alicloud/issues/4547))
- resource/alicloud_rds_clone_db_instance, alicloud_rds_upgrade_db_instance add new Attribute pg_hba_conf to support pgsql AD domain ([#4558](https://github.com/aliyun/terraform-provider-alicloud/issues/4558))	
- testcase: Adds new unit test case for resource alicloud_alidns_custom_line alicloud_sddp_config alicloud_alidns_address_pool ([#4551](https://github.com/aliyun/terraform-provider-alicloud/issues/4551))
- testcase: Adds new unit test case for resource alicloud_waf_instance alicloud_waf_certificate alicloud_waf_protection_module ([#4552](https://github.com/aliyun/terraform-provider-alicloud/issues/4552))
- testcase: Adds new unit test case for resource alicloud_amqp_instance alicloud_amqp_queue alicloud_amqp_binding ([#4561](https://github.com/aliyun/terraform-provider-alicloud/issues/4561))
- testcase: Adds new unit test case for resource alicloud_ecs_auto_snapshot_policy alicloud_amqp_exchange alicloud_amqp_virtual_host ([#4563](https://github.com/aliyun/terraform-provider-alicloud/issues/4563))
- testcase: Adds new unit test case for resource alicloud_bastionhost_host_account alicloud_bastionhost_host alicloud_kvstore_audit_log_config ([#4570](https://github.com/aliyun/terraform-provider-alicloud/issues/4570))

## 1.154.0 (January 28, 2022)

- **New Resource:** `alicloud_nas_data_flow` ([#4538](https://github.com/aliyun/terraform-provider-alicloud/issues/4538))
- **New Data Source:** `alicloud_nas_data_flows` ([#4538](https://github.com/aliyun/terraform-provider-alicloud/issues/4538))

ENHANCEMENTS:

- resource/alicloud_nas_data_flow: update support regions NASCPFSSupportRegions. ([#4540](https://github.com/aliyun/terraform-provider-alicloud/issues/4540))
- datasource/alicloud_nat_gateways: Adds three internal parameters current_pagepage_size total_count to support paging ([#4541](https://github.com/aliyun/terraform-provider-alicloud/issues/4541))
- datasource/alicloud_slb_load_balancers: Adds three internal parameters current_page page_size total_count to support paging ([#4534](https://github.com/aliyun/terraform-provider-alicloud/issues/4534))
- datasource/alicloud_security_groups: Adds three internal parameters current_pagepage_size total_count to support paging ([#4536](https://github.com/aliyun/terraform-provider-alicloud/issues/4536))
- datasource/alicloud_vpcs: Adds three internal parameters current_pagepage_size total_count to support paging ([#4533](https://github.com/aliyun/terraform-provider-alicloud/issues/4533))
- datasource/alicloud_adb_db_clusters: Adds three internal parameters current_pagepage_size total_count to support paging ([#4542](https://github.com/aliyun/terraform-provider-alicloud/issues/4542))
- datasource/alicloud_db_instances: Adds three internal parameters current_pagepage_size total_count to support paging ([#4542](https://github.com/aliyun/terraform-provider-alicloud/issues/4542))
- datasource/alicloud_route_tables: Adds three internal parameters current_pagepage_size total_count to support paging ([#4542](https://github.com/aliyun/terraform-provider-alicloud/issues/4542))	
- datasource/alicloud_slb_zones: Supports new output parameters address_type and address_ip_version ([#4543](https://github.com/aliyun/terraform-provider-alicloud/issues/4543))	
- testcase: Adds a new test case for resource alicloud_alb_security_policy ([#4444](https://github.com/aliyun/terraform-provider-alicloud/issues/4444))
- testcase: Adds a new test case for resource alicloud_alb_security_policy ([#4407](https://github.com/aliyun/terraform-provider-alicloud/issues/4407))
- testcase: Adds a new test case for resource alicloud_slb_load_balancee ([#4411](https://github.com/aliyun/terraform-provider-alicloud/issues/4411))
- testcase: Adds a new test case for resource alicloud_alb_load_balancer ([#4443](https://github.com/aliyun/terraform-provider-alicloud/issues/4443))
- testcase: Adds a new test case for resource alicloud_express_connect_physical_connection ([#4280](https://github.com/aliyun/terraform-provider-alicloud/issues/4280))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_vpc_attachment ([#4436](https://github.com/aliyun/terraform-provider-alicloud/issues/4436))
- testcase: Adds a new test case for resource alicloud_alb_rule ([#4446](https://github.com/aliyun/terraform-provider-alicloud/issues/4446))
- testcase: Adds a new test case for resource alicloud_db_instance ([#4453](https://github.com/aliyun/terraform-provider-alicloud/issues/4453))
- testcase: Adds a new test case for resource alicloud_cen_bandwidth_package ([#4422](https://github.com/aliyun/terraform-provider-alicloud/issues/4422))
- testcase: Adds a new test case for resource alicloud_alb_server_group ([#4445](https://github.com/aliyun/terraform-provider-alicloud/issues/4445))
- testcase: Adds new unit test case for resource alicloud_alb_health_check_template alicloud_slb_tls_cipher_policy alicloud_slb_ca_certificate ([#4529](https://github.com/aliyun/terraform-provider-alicloud/issues/4529))
- testcase: Adds new unit test case for resource alicloud_cen_transit_router_route_table_association alicloud_cen_transit_router_route_table_propagation alicloud_cen_transit_router_route_table ([#4520](https://github.com/aliyun/terraform-provider-alicloud/issues/4520))
- testcase: Adds new unit test case for resource alicloud_cdn_real_time_log_delivery alicloud_cen_transit_router_vbr_attachment alicloud_cen_transit_router_vpc_attachment ([#4523](https://github.com/aliyun/terraform-provider-alicloud/issues/4523))
- testcase: Adds new unit test case for resource alicloud_alb_security_policy alicloud_rds_backup alicloud_ecd_image ([#4531](https://github.com/aliyun/terraform-provider-alicloud/issues/4531))
- testcase: Adds new unit test case for resource alicloud_ecd_simple_office_site alicloud_ecd_network_package alicloud_ecd_nas_file_system ([#4537](https://github.com/aliyun/terraform-provider-alicloud/issues/4537))
- testcase: Adds new unit test case for resource alicloud_ecd_user alicloud_ecd_command alicloud_ram_saml_provider ([#4539](https://github.com/aliyun/terraform-provider-alicloud/issues/4539))
- testcase: Improve the effectiveness of test cases ([#4530](https://github.com/aliyun/terraform-provider-alicloud/issues/4530))
- testcase/alicloud_nat_gateway: Improves the nat gateway testcases ([#4474](https://github.com/aliyun/terraform-provider-alicloud/issues/4474))
- testcase/alicloud_snat_entry: Improves the snat entry testcases ([#4474](https://github.com/aliyun/terraform-provider-alicloud/issues/4474))
- testcase: Adds new unit test case for resource alicloud_nas_lifecycle_policy ([#4535](https://github.com/aliyun/terraform-provider-alicloud/issues/4535))
- testcase: Improve the unit of the test cases ([#4544](https://github.com/aliyun/terraform-provider-alicloud/issues/4544))

BUG FIXES:

- bug/alicloud_snat_entry: Corrected field source_vswitch_id, source_cidr to Computed ([#4528](https://github.com/aliyun/terraform-provider-alicloud/issues/4528))

## 1.153.0 (January 23, 2022)

- **New Resource:** `alicloud_alidns_monitor_config`([#4477](https://github.com/aliyun/terraform-provider-alicloud/issues/4477))
- **New Resource:** `alicloud_vpc_bgp_peer`([#4500](https://github.com/aliyun/terraform-provider-alicloud/issues/4500))
- **New Resource:** `alicloud_vpc_dhcp_options_set_attachment`([#4505](https://github.com/aliyun/terraform-provider-alicloud/issues/4505))
- **New Resource:** `alicloud_nas_fileset`([#4508](https://github.com/aliyun/terraform-provider-alicloud/issues/4508))
- **New Resource:** `alicloud_nas_auto_snapshot_policy`([#4509](https://github.com/aliyun/terraform-provider-alicloud/issues/4509))
- **New Resource:** `alicloud_nas_lifecycle_policy`([#4513](https://github.com/aliyun/terraform-provider-alicloud/issues/4513))
- **New Resource:** `alicloud_rds_upgrade_db_instance`([#4475](https://github.com/aliyun/terraform-provider-alicloud/issues/4475))	
- **New Resource:** `alicloud_vpc_bgp_network`([#4516](https://github.com/aliyun/terraform-provider-alicloud/issues/4516))
- **New Data Source:** `alicloud_vpc_bgp_networks`([#4516](https://github.com/aliyun/terraform-provider-alicloud/issues/4516))	
- **New Data Source:** `alicloud_nas_lifecycle_policies`([#4513](https://github.com/aliyun/terraform-provider-alicloud/issues/4513))	
- **New Data Source:** `alicloud_nas_auto_snapshot_policies`([#4509](https://github.com/aliyun/terraform-provider-alicloud/issues/4509))
- **New Data Source:** `alicloud_nas_filesets`([#4508](https://github.com/aliyun/terraform-provider-alicloud/issues/4508))	
- **New Data Source:** `alicloud_vpc_bgp_peers`([#4500](https://github.com/aliyun/terraform-provider-alicloud/issues/4500))
- **New Data Source:** `alicloud_cdn_ip_info`([#4511](https://github.com/aliyun/terraform-provider-alicloud/issues/4511))

ENHANCEMENTS:

- resource/alicloud_security_group_rule: support updating prefix_list_id([#4496](https://github.com/aliyun/terraform-provider-alicloud/issues/4496))
- resource/sae_application: add the Async await process([#4525](https://github.com/aliyun/terraform-provider-alicloud/issues/4525))
- resource/alicloud_hbr_nas_backup_plan: remove attribute create_time([#4518](https://github.com/aliyun/terraform-provider-alicloud/issues/4518))
- resource/alicloud_nas_file_system: Support for creating cpfs file system and configuration tags([#4508](https://github.com/aliyun/terraform-provider-alicloud/issues/4508))
- datasource/alicloud_alikafka_topics: Adds two internal parameters current_page and page_size to support paging([#4514](https://github.com/aliyun/terraform-provider-alicloud/issues/4514))
- datasource/alicloud_emr_clusters: Adds three internal parameters current_page page_size total_count to support paging([#4519](https://github.com/aliyun/terraform-provider-alicloud/issues/4519))
- datasource/alicloud_instances: Adds three internal parameters current_page page_size total_count to support paging([#4521](https://github.com/aliyun/terraform-provider-alicloud/issues/4521))
- datasource/alicloud_ecs_disks: Adds three internal parameters current_page page_size total_count to support paging([#4524](https://github.com/aliyun/terraform-provider-alicloud/issues/4524))	
- testcase: Adds a new test case for resource alicloud_db_database([#4452](https://github.com/aliyun/terraform-provider-alicloud/issues/4452))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_route_table_association([#4433](https://github.com/aliyun/terraform-provider-alicloud/issues/4433))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_route_entry([#4431](https://github.com/aliyun/terraform-provider-alicloud/issues/4431))
- testcase: Adds a new test case for resource alicloud_cen_route_service([#4427](https://github.com/aliyun/terraform-provider-alicloud/issues/4427))
- testcase: Adds a new test case for resource alicloud_dcdn_domain([#4420](https://github.com/aliyun/terraform-provider-alicloud/issues/4420))
- testcase: Adds new unit test case for resource alicloud_ecs_session_manager_status alicloud_ecs_key_pair alicloud_ecs_network_interface_attachment([#4506](https://github.com/aliyun/terraform-provider-alicloud/issues/4506))
- testcase: Adds new unit test case for resource alicloud_ecs_snapshot alicloud_ecs_hpc_cluster alicloud_ecs_deployment_set([#4487](https://github.com/aliyun/terraform-provider-alicloud/issues/4487))
- testcase: Adds a new test case for resource alicloud_rds_parameter_group([#4449](https://github.com/aliyun/terraform-provider-alicloud/issues/4449))
- testcase: Adds a new test case for resource alicloud_rds_account([#4448](https://github.com/aliyun/terraform-provider-alicloud/issues/4448))
- testcase: Adds new unit test case for resource alicloud_cen_transit_router_route_entry alicloud_cen_transit_router_peer_attachment alicloud_cen_transit_router([#4428](https://github.com/aliyun/terraform-provider-alicloud/issues/4428))
- testcase: Adds new unit test case for resource alicloud_vpc_vbr_ha alicloud_cen_instance alicloud_vpc_bgp_group([#4512](https://github.com/aliyun/terraform-provider-alicloud/issues/4512))
- testcase: Improve the effectiveness of test cases([#4515](https://github.com/aliyun/terraform-provider-alicloud/issues/4515))
- testcase: Improve the effectiveness of test cases([#4526](https://github.com/aliyun/terraform-provider-alicloud/issues/4526))
- testcase: Adds a new test case for resource alicloud_cen_instance([#4424](https://github.com/aliyun/terraform-provider-alicloud/issues/4424))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_peer_attachment([#4429](https://github.com/aliyun/terraform-provider-alicloud/issues/4429))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_route_table([#4432](https://github.com/aliyun/terraform-provider-alicloud/issues/4432))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_route_table_propagation([#4434](https://github.com/aliyun/terraform-provider-alicloud/issues/4434))
- testcase: Adds a new test case for resource alicloud_cen_transit_router_vbr_attachment([#4435](https://github.com/aliyun/terraform-provider-alicloud/issues/4435))
- testcase: Adds a new test case for resource alicloud_cen_vbr_health_check ([#4437](https://github.com/aliyun/terraform-provider-alicloud/issues/4437))
- testcase: Adds a new test case for resource alicloud_alb_acl([#4439](https://github.com/aliyun/terraform-provider-alicloud/issues/4439))
- testcase: Adds a new test case for resource alicloud_alb_health_check_template([#4440](https://github.com/aliyun/terraform-provider-alicloud/issues/4440))
- testcase: Adds a new test case for resource alicloud_alb_listener([#4441](https://github.com/aliyun/terraform-provider-alicloud/issues/4441))

## 1.152.0 (January 16, 2022)

- **New Resource:** `alicloud_vpc_bgp_group`([#4465](https://github.com/aliyun/terraform-provider-alicloud/issues/4465))
- **New Resource:** `alicloud_ram_security_preference`([#4478](https://github.com/aliyun/terraform-provider-alicloud/issues/4478))
- **New Resource:** `alicloud_nas_snapshot`([#4483](https://github.com/aliyun/terraform-provider-alicloud/issues/4483))
- **New Resource:** `alicloud_hbr_replication_vault`([#4488](https://github.com/aliyun/terraform-provider-alicloud/issues/4488))
- **New Resource:** `alicloud_alidns_address_pool`([#4476](https://github.com/aliyun/terraform-provider-alicloud/issues/4476))
- **New Resource:** `alicloud_ecs_prefix_list`([#4492](https://github.com/aliyun/terraform-provider-alicloud/issues/4492))
- **New Resource:** `alicloud_alidns_access_strategy`([#4491](https://github.com/aliyun/terraform-provider-alicloud/issues/4491))
- **New Data Source:** `alicloud_ecs_prefix_lists`([#4492](https://github.com/aliyun/terraform-provider-alicloud/issues/4492))
- **New Data Source:** `alicloud_alidns_address_pools`([#4476](https://github.com/aliyun/terraform-provider-alicloud/issues/4476))
- **New Data Source:** `alicloud_hbr_replication_vault_regions`([#4488](https://github.com/aliyun/terraform-provider-alicloud/issues/4488))
- **New Data Source:** `alicloud_nas_snapshots`([#4483](https://github.com/aliyun/terraform-provider-alicloud/issues/4483))
- **New Data Source:** `alicloud_vpc_bgp_groups`([#4465](https://github.com/aliyun/terraform-provider-alicloud/issues/4465))
- **New Data Source:** `alicloud_alidns_access_strategies`([#4491](https://github.com/aliyun/terraform-provider-alicloud/issues/4491))

ENHANCEMENTS:

- resource/alicloud_security_group_rule: support updating prefix_list_id([#4496](https://github.com/aliyun/terraform-provider-alicloud/issues/4496))
- datasource/alicloud_alikafka_topics: Adds new attribute id status_name instance_id tags([#4494](https://github.com/aliyun/terraform-provider-alicloud/issues/4494))
- datasource/alicloud_alikafka_instances: Adds new attribute upgrade_service_detail_info tags domain_endpoint ssl_domain_endpoint sasl_domain_endpoint allowed_list([#4494](https://github.com/aliyun/terraform-provider-alicloud/issues/4494))
- datasource/alicloud_alikafka_consumer_groups: Adds new attribute id consumer_id instance_id remark tags([#4494](https://github.com/aliyun/terraform-provider-alicloud/issues/4494))
- datasource/alicloud_cloud_storage_gateway_storage_bundles: Adds two internal parameters page_number and page_size to support paging([#4490](https://github.com/aliyun/terraform-provider-alicloud/issues/4490))
- datasource/alicloud_cloud_storage_gateway_gateways: Adds two internal parameters page_number and page_size to support paging([#4493](https://github.com/aliyun/terraform-provider-alicloud/issues/4493))
- datasource/alicloud_nas_zones: Add support for field file_system_type([#4483](https://github.com/aliyun/terraform-provider-alicloud/issues/4483))
- testcase: Adds new unit test case for resource alicloud_ecs_dedicated_host_cluster alicloud_ecs_auto_snapshot_policy_attachment alicloud_ecs_command([#4482](https://github.com/aliyun/terraform-provider-alicloud/issues/4482))
- testcase: Adds new unit test case for resource alicloud_route_table alicloud_forward_entry alicloud_vpc_flow_log([#4481](https://github.com/aliyun/terraform-provider-alicloud/issues/4481))
- docs/d/kvstore_connections: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/actiontrail_history_delivery_job: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/actiontrail_trail: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/db_backup_policy: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/kvstore_account: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/kvstore_instance: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/slb_domain_extension: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/slb_listener: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/slb_load_balancer: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/ssl_vpn_serverdocs/r/vpc_ipv6_egress_rule: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- docs/r/vpn_connection: document optimization([#4486](https://github.com/aliyun/terraform-provider-alicloud/issues/4486))
- client: adds a compatibile endpoint for adb service([#4502](https://github.com/aliyun/terraform-provider-alicloud/issues/4502))
- common: adds missing importing package and format the code([#4503](https://github.com/aliyun/terraform-provider-alicloud/issues/4503))
- ci:checkout the ci account doc/resource_actiontrail_history_delivery_job: improve the document([#4473](https://github.com/aliyun/terraform-provider-alicloud/issues/4473))

BUG FIXES:

- resource/alicloud_mhub_app: fixe the accessed issues in different regions([#4480](https://github.com/aliyun/terraform-provider-alicloud/issues/4480))
- resource/alicloud_mhub_product: fixe the accessed issues in different regions([#4480](https://github.com/aliyun/terraform-provider-alicloud/issues/4480))
- resource/alicloud_cs_kubernetes_node_pool: Fixed an issue where modifying node pool parameters would cause elastic scaling to be turned off([#4497](https://github.com/aliyun/terraform-provider-alicloud/issues/4497))

## 1.151.0 (January 09, 2022)

- **New Resource:** `alicloud_alidns_custom_line`([#4456](https://github.com/aliyun/terraform-provider-alicloud/issues/4456))
- **New Resource:** `alicloud_vpc_vbr_ha`([#4461](https://github.com/aliyun/terraform-provider-alicloud/issues/4461))	
- **New Resource:** `alicloud_ros_template_scratch`([#4421](https://github.com/aliyun/terraform-provider-alicloud/issues/4421))
- **New Resource:** `alidns_gtm_instance`([#4464](https://github.com/aliyun/terraform-provider-alicloud/issues/4464))
- **New Data Source:** `alidns_gtm_instances`([#4464](https://github.com/aliyun/terraform-provider-alicloud/issues/4464))
- **New Data Source:** `alicloud_ros_template_scratches`([#4421](https://github.com/aliyun/terraform-provider-alicloud/issues/4421))	
- **New Data Source:** `alicloud_alidns_custom_lines`([#4456](https://github.com/aliyun/terraform-provider-alicloud/issues/4456))

ENHANCEMENTS:

- alicloud_ess_scalingconfiguration: Adds new attributes spot_strategy and spot_price_limit([#4413](https://github.com/aliyun/terraform-provider-alicloud/issues/4413))
- datasource/alicloud_cen_transit_routers: Modify the parameter transit_router_id to Optional doc/cen_transit_routers: Optimize documentation([#4459](https://github.com/aliyun/terraform-provider-alicloud/issues/4459))
- datasource/alicloud_cloud_storage_gateway_gateways: Optimize payment_type output parameter conversion([#4469](https://github.com/aliyun/terraform-provider-alicloud/issues/4469))
- testcase: Update the invalid test([#4419](https://github.com/aliyun/terraform-provider-alicloud/issues/4419))
- testcase: Adds a new test case for resource alicloud_ecs_launch_template([#4313](https://github.com/aliyun/terraform-provider-alicloud/issues/4313))
- testcase: Adds a new test case for resource alicloud_ecs_snapshot([#4324](https://github.com/aliyun/terraform-provider-alicloud/issues/4324))
- testcase: Adds a new test case for resource alicloud_ecs_dedicated_host_cluster([#4334](https://github.com/aliyun/terraform-provider-alicloud/issues/4334))
- testcase: Change vpc and vswitch creation to read([#4399](https://github.com/aliyun/terraform-provider-alicloud/issues/4399))
- testcase: Change vpc and vswitch creation to read([#4387](https://github.com/aliyun/terraform-provider-alicloud/issues/4387))
- testcase: Adds a new test case for resource alicloud_snat_entry([#4276](https://github.com/aliyun/terraform-provider-alicloud/issues/4276))
- testcase: Adds a new test case for resource alicloud_ecs_dedicated_host([#4291](https://github.com/aliyun/terraform-provider-alicloud/issues/4291))
- testcase: Adds a new test case for resource alicloud_ecs_disk([#4302](https://github.com/aliyun/terraform-provider-alicloud/issues/4302))
- testcase: Adds a new test case for resource alicloud_image([#4331](https://github.com/aliyun/terraform-provider-alicloud/issues/4331))
- testcase: Adds a new test case for resource alicloud_ecs_disk_attachment([#4333](https://github.com/aliyun/terraform-provider-alicloud/issues/4333))
- testcase: Adds a new test case for resource alicloud_ecs_network_interface([#4336](https://github.com/aliyun/terraform-provider-alicloud/issues/4336))
- testcase: Adds new unit test case for resource alicloud_vpc_traffic_mirror_filter_egress_rule alicloud_vpc_traffic_mirror_filter alicloud_vpc_traffic_mirror_filter_ingress_rule([#4458](https://github.com/aliyun/terraform-provider-alicloud/issues/4458))
- testcase: Adds new unit test case for resource alicloud_vpc_nat_ip alicloud_vpc_nat_ip_cidr alicloud_havip([#4466](https://github.com/aliyun/terraform-provider-alicloud/issues/4466))
- testcase: Adds a new test case for resource alicloud_nat_gateway([#4272](https://github.com/aliyun/terraform-provider-alicloud/issues/4272))

BUG FIXES:

- resource/alicloud_rds_account: Fixes the OperationDenied.DBInstanceStatus when deleting rds account([#4471](https://github.com/aliyun/terraform-provider-alicloud/issues/4471))
- resource/ga_bandwidth_package_attachment: fix the attachment while the bandwidth package type is cross domain([#4470](https://github.com/aliyun/terraform-provider-alicloud/issues/4470))

## 1.150.0 (January 02, 2022)

- **New Resource:** `alicloud_ga_acl`([#4416](https://github.com/aliyun/terraform-provider-alicloud/issues/4416))
- **New Resource:** `alicloud_ga_acl_attachment`([#4416](https://github.com/aliyun/terraform-provider-alicloud/issues/4416))	
- **New Resource:** `alicloud_ga_additional_certificate`([#4425](https://github.com/aliyun/terraform-provider-alicloud/issues/4425))
- **New Resource:** `alicloud_cs_kubernetes_addon`([#4402](https://github.com/aliyun/terraform-provider-alicloud/issues/4402))
- **New Data Source:** `alicloud_cs_kubernetes_addons`([#4402](https://github.com/aliyun/terraform-provider-alicloud/issues/4402))
- **New Data Source:** `alicloud_ga_additional_certificates`([#4425](https://github.com/aliyun/terraform-provider-alicloud/issues/4425))	
- **New Data Source:** `alicloud_ga_acls`([#4416](https://github.com/aliyun/terraform-provider-alicloud/issues/4416))

ENHANCEMENTS:

- resource/alicloud_ga_accelerator: Added the time limit of the field duration.([#4426](https://github.com/aliyun/terraform-provider-alicloud/issues/4426))
- datasource/alicloud_instance_types: Removes the parameter system_disk_category default value cloud_efficiency([#4430](https://github.com/aliyun/terraform-provider-alicloud/issues/4430))
- docs/alicloud_kms_key: Improves the resource attribute description([#4415](https://github.com/aliyun/terraform-provider-alicloud/issues/4415))
- doc/alicloud_cen_transit_router: Optimize document([#4417](https://github.com/aliyun/terraform-provider-alicloud/issues/4417))
- docs/cloud_sso_access_configuration: Optimize document([#4423](https://github.com/aliyun/terraform-provider-alicloud/issues/4423))
- testcase: Adds a new test case for resource alicloud_common_bandwidth_package([#4262](https://github.com/aliyun/terraform-provider-alicloud/issues/4262))
- testcase: Fixes the alicloud_cs_kubernetes_addon test case bug([#4451](https://github.com/aliyun/terraform-provider-alicloud/issues/4451))

BUG FIXES:

- resource/alicloud_slb_acl: Fixed the limit on the number of IP entries; Updates its dependence SDK.([#4447](https://github.com/aliyun/terraform-provider-alicloud/issues/4447))
- testcase: Fixes the alicloud_cs_kubernetes_addon test case bug([#4450](https://github.com/aliyun/terraform-provider-alicloud/issues/4450))

## 1.149.0 (December 26, 2021)

- **New Resource:** `alicloud_rds_backup`([#4343](https://github.com/aliyun/terraform-provider-alicloud/issues/4343))
- **New Resource:** `alicloud_rds_clone_db_instance`([#4361](https://github.com/aliyun/terraform-provider-alicloud/issues/4361))	
- **New Resource:** `alicloud_cr_chart_namespace`([#4391](https://github.com/aliyun/terraform-provider-alicloud/issues/4391))
- **New Resource:** `alicloud_fnf_execution`([#4395](https://github.com/aliyun/terraform-provider-alicloud/issues/4395))
- **New Resource:** `alicloud_mongodb_sharding_network_public_address`([#4397](https://github.com/aliyun/terraform-provider-alicloud/issues/4397))
- **New Resource:** `alicloud_cr_chart_repository`([#4393](https://github.com/aliyun/terraform-provider-alicloud/issues/4393))
- **New Data Source:** `alicloud_mongodb_sharding_network_addresses`([#4397](https://github.com/aliyun/terraform-provider-alicloud/issues/4397))
- **New Data Source:** `alicloud_cr_chart_repositories`([#4393](https://github.com/aliyun/terraform-provider-alicloud/issues/4393))	
- **New Data Source:** `alicloud_fnf_executions`([#4395](https://github.com/aliyun/terraform-provider-alicloud/issues/4395))
- **New Data Source:** `alicloud_cr_chart_namespaces`([#4391](https://github.com/aliyun/terraform-provider-alicloud/issues/4391))	
- **New Data Source:** `alicloud_rds_backups`([#4343](https://github.com/aliyun/terraform-provider-alicloud/issues/4343))

ENHANCEMENTS:

- resource/alicloud_instance: Support updating the filed deployment_set_id and deployment_set_group_no([#4408](https://github.com/aliyun/terraform-provider-alicloud/issues/4408))
- resource/alicloud_cs_kubernetes_node_pool: CS kubernetes nodepool support deploymentSet([#4371](https://github.com/aliyun/terraform-provider-alicloud/issues/4371))
- resource/alicloud_cr_endpoint_acl_policy : Added error retry code SLB_SERVICE_ERROR([#4351](https://github.com/aliyun/terraform-provider-alicloud/issues/4351))
- resource/alicloud_dts_synchronization_job: Change delete api; Improved test cases([#4401](https://github.com/aliyun/terraform-provider-alicloud/issues/4401))
- docs/cloud_sso_access_configuration: Optimize document([#4412](https://github.com/aliyun/terraform-provider-alicloud/issues/4412))
- docs/cloud_sso_group: Optimize document([#4412](https://github.com/aliyun/terraform-provider-alicloud/issues/4412))	
- docs/cloud_sso_user: Optimize document([#4412](https://github.com/aliyun/terraform-provider-alicloud/issues/4412))
- testcase: Change vpc and vswitch creation to read([#4376](https://github.com/aliyun/terraform-provider-alicloud/issues/4376))
- testcase: Change vpc and vswitch creation to read([#4382](https://github.com/aliyun/terraform-provider-alicloud/issues/4382))
- testcase: Improves the resource sweeper testcases([#4386](https://github.com/aliyun/terraform-provider-alicloud/issues/4386))
- testcase: Improves the ddos instance testcases([#4390](https://github.com/aliyun/terraform-provider-alicloud/issues/4390))	
- testcase: Change vpc and vswitch creation to read([#4394](https://github.com/aliyun/terraform-provider-alicloud/issues/4394))	
- GithubWorkFlow: 1. Add the consistency check between the schema and document 2. Add the incompatible check between the current pr and previous provder version([#4378](https://github.com/aliyun/terraform-provider-alicloud/issues/4378))

BUG FIXES:

- resource/alicloud_amqp_instance: fix the product_type checkout between domestic account and international account([#4409](https://github.com/aliyun/terraform-provider-alicloud/issues/4409))
- resource/alicloud_cs_kubernetes_node_pool unschedulable parameter bugfix([#4403](https://github.com/aliyun/terraform-provider-alicloud/issues/4403))
- resource/cloud_sso_access_configuration: Fixed character length limit error for access_configuration_name attribute([#4412](https://github.com/aliyun/terraform-provider-alicloud/issues/4412))
- GithubWorkFlow: fix the issue of the markdown parser([#4392](https://github.com/aliyun/terraform-provider-alicloud/issues/4392))

## 1.148.0 (December 19, 2021)

- **New Resource:** `alicloud_mongodb_audit_policy`([#4368](https://github.com/aliyun/terraform-provider-alicloud/issues/4368))
- **New Resource:** `cloud_sso_access_configuration_provisioning`([#4369](https://github.com/aliyun/terraform-provider-alicloud/issues/4369))
- **New Resource:** `alicloud_mongodb_account`([#4375](https://github.com/aliyun/terraform-provider-alicloud/issues/4375))
- **New Resource:** `alicloud_mongodb_serverless_instance`([#4365](https://github.com/aliyun/terraform-provider-alicloud/issues/4365))
- **New Resource:** `ecs_session_manager_status`([#4337](https://github.com/aliyun/terraform-provider-alicloud/issues/4337))
- **New Resource:** `cddc_dedicated_host_account`([#4358](https://github.com/aliyun/terraform-provider-alicloud/issues/4358))
- **New Data Source:** `cddc_dedicated_host_accounts`([#4365](https://github.com/aliyun/terraform-provider-alicloud/issues/4365))
- **New Data Source:** `alicloud_mongodb_serverless_instances`([#4365](https://github.com/aliyun/terraform-provider-alicloud/issues/4365))	
- **New Data Source:** `alicloud_mongodb_accounts`([#4375](https://github.com/aliyun/terraform-provider-alicloud/issues/4375))	
- **New Data Source:** `alicloud_mongodb_audit_policies`([#4368](https://github.com/aliyun/terraform-provider-alicloud/issues/4368))
- **New Data Source:** `cloud_sso_service`([#4367](https://github.com/aliyun/terraform-provider-alicloud/issues/4367))
	
ENHANCEMENTS:

- resource/alicloud_pvtz_zone: Support update sync_status without user_info([#4372](https://github.com/aliyun/terraform-provider-alicloud/issues/4372))
- resource/alicloud_db_instance Add new attribute fresh_white_list_readins to support read-only instances to which you want to synchronize the IP address whitelist.([#4379](https://github.com/aliyun/terraform-provider-alicloud/issues/4379))
- resource/alicloud_cddc_dedicated_host_group: Added support for the field open_permission([#4358](https://github.com/aliyun/terraform-provider-alicloud/issues/4358))
- datasource/alicloud_alikafka_instances: Adds new attribute expired_time,msg_retain,ssl_end_point([#4352](https://github.com/aliyun/terraform-provider-alicloud/issues/4352))
- datasource/alicloud_cen_instances: Adds new attribute creation_time([#4349](https://github.com/aliyun/terraform-provider-alicloud/issues/4349))
- datasource/alicloud_ddoscoo_instances: Adds new attribute remark,ip_mode,debt_status,edition,ip_version,status,enabled,expire_time,create_time([#4352](https://github.com/aliyun/terraform-provider-alicloud/issues/4352))
- datasource/alicloud_adb_db_clusters: Adds new attribute mode([#4354](https://github.com/aliyun/terraform-provider-alicloud/issues/4354))
- datasource/alicloud_click_house_db_clusters: Adds new attribute control_version([#4355](https://github.com/aliyun/terraform-provider-alicloud/issues/4355))
- datasource/alicloud_cloud_storage_gateway_storage_bundles: Adds new attribute create_time([#4359](https://github.com/aliyun/terraform-provider-alicloud/issues/4359))
- datasource/alicloud_click_house_db_clusters: Adds new attribute status([#4362](https://github.com/aliyun/terraform-provider-alicloud/issues/4362))
- datasource/alicloud_sae_service: Add error code. datasource/alicloud_cen_instances: Adds new attribute create_time.([#4364](https://github.com/aliyun/terraform-provider-alicloud/issues/4364))	
- doc/alicloud_cloud_firewall_control_policy: document optimization([#4366](https://github.com/aliyun/terraform-provider-alicloud/issues/4366))
- doc/alicloud_cloud_dts_subscription_job: document optimization([#4373](https://github.com/aliyun/terraform-provider-alicloud/issues/4373))
- doc/alicloud_ga_accelerator,alicloud_ga_bandwidth_package: Optimize the documentation([#4377](https://github.com/aliyun/terraform-provider-alicloud/issues/4377))
- doc/config: Optimize the config documentation resource/alicloud_config_aggregator: changed the field aggregator_accounts from Required into optional([#4374](https://github.com/aliyun/terraform-provider-alicloud/issues/4374))
- docs/alb_acl: Optimize document.([#4380](https://github.com/aliyun/terraform-provider-alicloud/issues/4380))

BUG FIXES:

- resource/alicloud_alb_acl: Fixed the limit on the number of IP entries.([#4380](https://github.com/aliyun/terraform-provider-alicloud/issues/4380))
- datasource/alicloud_alb_acls: Fix query bug for acl_entries.([#4380](https://github.com/aliyun/terraform-provider-alicloud/issues/4380))
- datasource/alicloud_adb_db_clusters: Fix the problem of test case failure.([#4364](https://github.com/aliyun/terraform-provider-alicloud/issues/4364))

## 1.147.0 (December 12, 2021)

- **New Resource:** `alicloud_cddc_dedicated_host`([#4297](https://github.com/aliyun/terraform-provider-alicloud/issues/4297))
- **New Resource:** `alicloud_oos_service_setting`([#4321](https://github.com/aliyun/terraform-provider-alicloud/issues/4321))
- **New Resource:** `alicloud_oos_parameter`([#4327](https://github.com/aliyun/terraform-provider-alicloud/issues/4327))
- **New Resource:** `alicloud_oos_state_configuration`([#4323](https://github.com/aliyun/terraform-provider-alicloud/issues/4323))
- **New Resource:** `alicloud_oos_secret_parameter`([#4328](https://github.com/aliyun/terraform-provider-alicloud/issues/4328))
- **New Resource:** `alicloud_click_house_backup_policy`([#4341](https://github.com/aliyun/terraform-provider-alicloud/issues/4341))
- **New Data Source:** `alicloud_click_house_backup_policies`([#4341](https://github.com/aliyun/terraform-provider-alicloud/issues/4341))
- **New Data Source:** `alicloud_oos_secret_parameters`([#4328](https://github.com/aliyun/terraform-provider-alicloud/issues/4328))	
- **New Data Source:** `alicloud_oos_state_configurations`([#4323](https://github.com/aliyun/terraform-provider-alicloud/issues/4323))
- **New Data Source:** `alicloud_oos_parameters`([#4327](https://github.com/aliyun/terraform-provider-alicloud/issues/4327))	
- **New Data Source:** `alicloud_cddc_dedicated_hosts`([#4297](https://github.com/aliyun/terraform-provider-alicloud/issues/4297))
- **New Data Source:** `alicloud_cddc_zones`([#4297](https://github.com/aliyun/terraform-provider-alicloud/issues/4297))
- **New Data Source:** `alicloud_cddc_host_ecs_level_infos`([#4297](https://github.com/aliyun/terraform-provider-alicloud/issues/4297))

ENHANCEMENTS:

- resource/alicloud_instance: add the condition of the filed auto_release_time during updating([#4346](https://github.com/aliyun/terraform-provider-alicloud/issues/4346))
- resource/alicloud_amqp_instance: Supports create instance using international account([#4345](https://github.com/aliyun/terraform-provider-alicloud/issues/4345))
- resource/alicloud_db_backup_policy,add new attribute released_keep_policy to support modify released_keep_policy.([#4294](https://github.com/aliyun/terraform-provider-alicloud/issues/4294))
- resource/alicloud_cs_kubernetes_node_pool: enhanced the consistency of node count([#4330](https://github.com/aliyun/terraform-provider-alicloud/issues/4330))
- testcase: Adds new unit test case for resource alicloud_vswitch([#4347](https://github.com/aliyun/terraform-provider-alicloud/issues/4347))
- docs/brain_industrial_service,datahub_service,edas_service,mns_service,sae_service,vs_service,alidns_instance,amqp_instance,cloud_firewall_instance,sddp_instance : Update the support situation at the international site([#4332](https://github.com/aliyun/terraform-provider-alicloud/issues/4332))	
- doc/alicloud_log_audit: Add new parameter vpc_flow_enabled,vpc_flow_ttl,vpc_flow_collection_policy,vpc_sync_enabled,vpc_sync_ttl,ddos_bgp_access_enabled,ddos_bgp_access_ttl,ddos_dip_access_enabled,ddos_dip_access_ttl,ddos_dip_access_ti_enabled, Update the default value of oss_access_ttl,drds_audit_ttl,slb_access_ttl, Correct the parameter drds_audit_enabled([#4322](https://github.com/aliyun/terraform-provider-alicloud/issues/4322))
- Github WorkFlow: Add Some Basic Checks in PR([#4319](https://github.com/aliyun/terraform-provider-alicloud/issues/4319))
- Revert New Resource alicloud_rds_clone_db_instance([#4326](https://github.com/aliyun/terraform-provider-alicloud/issues/4326))

BUG FIXES:

- datasource/alicloud_emr_clusters: Fix the issue that the enable_details query is invalid([#4340](https://github.com/aliyun/terraform-provider-alicloud/issues/4340))

## 1.146.0 (December 05, 2021)

- **New Resource:** `alicloud_ecs_dedicated_host_cluster`([#4275](https://github.com/aliyun/terraform-provider-alicloud/issues/4275))
- **New Resource:** `alicloud_oos_application_group`([#4299](https://github.com/aliyun/terraform-provider-alicloud/issues/4299))
- **New Resource:** `alicloud_dts_consumer_channel`([#4290](https://github.com/aliyun/terraform-provider-alicloud/issues/4290))
- **New Resource:** `alicloud_ecd_image`([#4204](https://github.com/aliyun/terraform-provider-alicloud/issues/4204))
- **New Resource:** `alicloud_oos_patch_baseline`([#4305](https://github.com/aliyun/terraform-provider-alicloud/issues/4305))
- **New Resource:** `alicloud_ecd_command`([#4244](https://github.com/aliyun/terraform-provider-alicloud/issues/4244))  
- **New Data Source:** `alicloud_oos_patch_baselines`([#4305](https://github.com/aliyun/terraform-provider-alicloud/issues/4305))
- **New Data Source:** `alicloud_ecd_images`([#4204](https://github.com/aliyun/terraform-provider-alicloud/issues/4204))	
- **New Data Source:** `alicloud_emr_clusters`([#4301](https://github.com/aliyun/terraform-provider-alicloud/issues/4301))
- **New Data Source:** `alicloud_dts_consumer_channels`([#4290](https://github.com/aliyun/terraform-provider-alicloud/issues/4290))	
- **New Data Source:** `alicloud_oos_application_groups`([#4299](https://github.com/aliyun/terraform-provider-alicloud/issues/4299))	
- **New Data Source:** `alicloud_ecs_dedicated_host_clusters`([#4275](https://github.com/aliyun/terraform-provider-alicloud/issues/4275))
- **New Data Source:** `alicloud_ecd_commands`([#4244](https://github.com/aliyun/terraform-provider-alicloud/issues/4244))  

ENHANCEMENTS:

- resource/alicloud_pvtz_zone: Support updating the filed user_info and sync_status([#4300](https://github.com/aliyun/terraform-provider-alicloud/issues/4300))
- resource/alicloud_config_compliance_pack: Support updating the filed compliance_pack_name([#4295](https://github.com/aliyun/terraform-provider-alicloud/issues/4295))
- resource/alicloud_ga_accelerator: Adds new attributes renewal_status and auto_renew_duration to supports auto renew([#4306](https://github.com/aliyun/terraform-provider-alicloud/issues/4306))
- resource/alicloud_dts_synchronization_instance: replace api DescribeSynchronizationJobs to new api DescribeDtsJobDetail([#4298](https://github.com/aliyun/terraform-provider-alicloud/issues/4298))
- resource/alicloud_ram_user: Update the error message([#4075](https://github.com/aliyun/terraform-provider-alicloud/issues/4075))	
- datasource/alicloud_oos_application_groups: Adds output variable update_time.([#4312](https://github.com/aliyun/terraform-provider-alicloud/issues/4312))
- datasource/alicloud_config_aggregate_config_rules: add the Attributes aggregator_id, compliance([#4304](https://github.com/aliyun/terraform-provider-alicloud/issues/4304))
- datasource/alicloud_config_config_rules: removed the fields member_id, multi_account([#4304](https://github.com/aliyun/terraform-provider-alicloud/issues/4304))	
- testcase: Adds new testcase for resource alicloud_vpc_dhcp_options_set([#4251](https://github.com/aliyun/terraform-provider-alicloud/issues/4251))
- testcase: Adds new testcase for resource alicloud_vpc_flow_log([#4252](https://github.com/aliyun/terraform-provider-alicloud/issues/4252))
- testcase: Add new testcase for resource alicloud_vpc_traffic_mirror_filter([#4254](https://github.com/aliyun/terraform-provider-alicloud/issues/4254))
- testcase: Add new testcase for resource alicloud_vpc_traffic_mirror_filter_egress_rule([#4255](https://github.com/aliyun/terraform-provider-alicloud/issues/4255))
- testcase: Adds new testcase for resource alicloud_vpc_traffic_mirror_filter_ingress_rule([#4256](https://github.com/aliyun/terraform-provider-alicloud/issues/4256))
- testcase: Add new testcases for resource alicloud_vpc([#4257](https://github.com/aliyun/terraform-provider-alicloud/issues/4257))
- testcase: Add new testcase for resource alicloud_vpc_nat_ip([#4259](https://github.com/aliyun/terraform-provider-alicloud/issues/4259))
- testcase: Adds new test case for resource alicloud_vpc_nat_ip_cidr([#4261](https://github.com/aliyun/terraform-provider-alicloud/issues/4261))	
- testcase: Adds new test case for resource alicloud_havip([#4269](https://github.com/aliyun/terraform-provider-alicloud/issues/4269))
- testcase: Adds new test case for resource alicloud_network_acl([#4273](https://github.com/aliyun/terraform-provider-alicloud/issues/4273))	
- testcase: Adds new test case for resource alicloud_route_table([#4274](https://github.com/aliyun/terraform-provider-alicloud/issues/4274))	
- testcase: Adds new test case for resource alicloud_vswitch([#4277](https://github.com/aliyun/terraform-provider-alicloud/issues/4277))	
- testcase: Adds new testcase for resource alicloud_vpc_traffic_mirror_session([#4281](https://github.com/aliyun/terraform-provider-alicloud/issues/4281))	
- testcase: Adds new unit test case for resource alicloud_vpc([#4314](https://github.com/aliyun/terraform-provider-alicloud/issues/4314))
- testcase: Adds new test case for resource alicloud_ecs_key_pair([#4303](https://github.com/aliyun/terraform-provider-alicloud/issues/4303))
- testcase: Adds a new test case for resource alicloud_ecs_deployment_set([#4292](https://github.com/aliyun/terraform-provider-alicloud/issues/4292))	
- testcase: Adds a new test case for resource alicloud_ecs_command([#4289](https://github.com/aliyun/terraform-provider-alicloud/issues/4289))
- testcase: Adds a new test case for resource alicloud_ecs_auto_snapshot_policy([#4288](https://github.com/aliyun/terraform-provider-alicloud/issues/4288))	
- testcase: Adds a new test case for resource alicloud_eip_address([#4265](https://github.com/aliyun/terraform-provider-alicloud/issues/4265))
- testcase: Adds a new test case for resource alicloud_forward_entry([#4268](https://github.com/aliyun/terraform-provider-alicloud/issues/4268))	
- testcase: Improves the log project sweeper test case([#4317](https://github.com/aliyun/terraform-provider-alicloud/issues/4317))
- testcase: Upgrades the gomonkey version to v2([#4318](https://github.com/aliyun/terraform-provider-alicloud/issues/4318))  
- docs/alicloud_dts_synchronization_job: Improves its docs on attribute dts_job_name([#4311](https://github.com/aliyun/terraform-provider-alicloud/issues/4311))	
- doc/alicloud_cloud_sso_user: Document optimization doc/alicloud_cloud_sso_directory: Document optimization([#4309](https://github.com/aliyun/terraform-provider-alicloud/issues/4309))
- docs/alicloud_cs_managed_kubernetes: Corrects the misspelled words([#4248](https://github.com/aliyun/terraform-provider-alicloud/issues/4248))
- docs/alicloud_sae_application:Support updating the filed replicas([#4316](https://github.com/aliyun/terraform-provider-alicloud/issues/4316))

BUG FIXES:

- resource/alicloud_ga_accelerator: Fixes the InvalidRegionId error when getting the its endpoint([#4310](https://github.com/aliyun/terraform-provider-alicloud/issues/4310))
- resource/alicloud_polardb_db_instance: Fixes the setting security_ips bug without filtering hidden values([#4233](https://github.com/aliyun/terraform-provider-alicloud/issues/4233))
- resource/alicloud_ga_bandwidth_package,alicloud_ga_ip_set: Fix the GreaterThanGa.IpSetBandwidth error([#4307](https://github.com/aliyun/terraform-provider-alicloud/issues/4307))

## 1.145.0 (November 28, 2021)

- **New Resource:** `alicloud_ros_stack_instance`([#4258](https://github.com/aliyun/terraform-provider-alicloud/issues/4258))
- **New Resource:** `alicloud_eci_virtual_node`([#4266](https://github.com/aliyun/terraform-provider-alicloud/issues/4266))
- **New Resource:** `alicloud_oos_application`([#4271](https://github.com/aliyun/terraform-provider-alicloud/issues/4271))
- **New Data Source:** `alicloud_oos_applications`([#4271](https://github.com/aliyun/terraform-provider-alicloud/issues/4271))  
- **New Data Source:** `alicloud_eci_virtual_nodes`([#4266](https://github.com/aliyun/terraform-provider-alicloud/issues/4266))  
- **New Data Source:** `alicloud_ros_stack_instances`([#4258](https://github.com/aliyun/terraform-provider-alicloud/issues/4258))
- **New Data Source:** `alicloud_eci_zones`([#4266](https://github.com/aliyun/terraform-provider-alicloud/issues/4266))

ENHANCEMENTS:

- provider: Adds TF_APPEND_USER_AGENT environment variables to support setting custom user-agent([#4287](https://github.com/aliyun/terraform-provider-alicloud/issues/4287))
- resource/config_rule: Support configuring the specified field status([#4242](https://github.com/aliyun/terraform-provider-alicloud/issues/4242))
- resource/alicloud_click_house_db_cluster: Add db_cluster_access_white_list attribute.([#4247](https://github.com/aliyun/terraform-provider-alicloud/issues/4247))
- resource/config_aggregate_config_rule: Support updating the filed status([#4250](https://github.com/aliyun/terraform-provider-alicloud/issues/4250))
- resource/alicloud_cloud_sso_access_configuration: Modify the parametrs permission_policy_name and permission_policy_type as required parameters.([#4263](https://github.com/aliyun/terraform-provider-alicloud/issues/4263))
- resource/alicloud_cloud_sso_access_assignment: Optimize the logic of resource acquisition.([#4263](https://github.com/aliyun/terraform-provider-alicloud/issues/4263))
- resource/cloud_storage_gateway_gateway_file_share_test: Refine test cases.([#4264](https://github.com/aliyun/terraform-provider-alicloud/issues/4264))
- resource/alicloud_cs_kubernetes_node_pool: Support multi security groups.([#4267](https://github.com/aliyun/terraform-provider-alicloud/issues/4267))
- resource/alicloud_instance: Support configuring the filed secondary_private_ip_address_count([#4270](https://github.com/aliyun/terraform-provider-alicloud/issues/4270))
- resource/config_aggregate_compliance_pack: Support updating the filed aggregate_compliance_pack_name([#4282](https://github.com/aliyun/terraform-provider-alicloud/issues/4282))
- datasource/alicloud_images: Adds two attribute image_id and image_name([#4285](https://github.com/aliyun/terraform-provider-alicloud/issues/4285))  

BUG FIXES:

- resource/alicloud_ecs_disk: Fixes the InvalidParameter error when modifying the disk charge type([#4284](https://github.com/aliyun/terraform-provider-alicloud/issues/4284))
- resource/alicloud_cs_serverless_kubernetes: fix vswitch_ids returns null([#4267](https://github.com/aliyun/terraform-provider-alicloud/issues/4267))
- resource/alicloud_cs_managed_kubernetes: Fix the inconsistency of the number of cluster nodes([#4279](https://github.com/aliyun/terraform-provider-alicloud/issues/4279))
- data_source/alb_security_policies: Fixing query errors; Refine test cases.([#4283](https://github.com/aliyun/terraform-provider-alicloud/issues/4283))
- doc/cloud_storage_gateway_gateway_cache_disk: Fix formatting errors.([#4264](https://github.com/aliyun/terraform-provider-alicloud/issues/4264))
- datasource/alicloud_log_service: fix logtail Unmarshal bug and update log service([#4236](https://github.com/aliyun/terraform-provider-alicloud/issues/4236))

## 1.144.0 (November 21, 2021)

- **New Resource:** `alicloud_direct_mail_tag`([#4178](https://github.com/aliyun/terraform-provider-alicloud/issues/4178))
- **New Resource:** `alicloud_ecd_desktop`([#4199](https://github.com/aliyun/terraform-provider-alicloud/issues/4199))
- **New Resource:** `alicloud_cloud_storage_gateway_gateway_cache_disk`([#4217](https://github.com/aliyun/terraform-provider-alicloud/issues/4217))
- **New Resource:** `alicloud_cloud_storage_gateway_gateway_logging`([#4227](https://github.com/aliyun/terraform-provider-alicloud/issues/4227))
- **New Resource:** `alicloud_cloud_storage_gateway_gateway_file_share`([#4231](https://github.com/aliyun/terraform-provider-alicloud/issues/4231))
- **New Resource:** `alicloud_cloud_storage_gateway_gateway_block_volume`([#4234](https://github.com/aliyun/terraform-provider-alicloud/issues/4234))
- **New Resource:** `alicloud_cloud_storage_gateway_express_sync`([#4239](https://github.com/aliyun/terraform-provider-alicloud/issues/4239))
- **New Resource:** `alicloud_cloud_storage_gateway_express_sync_share_attachment`([#4239](https://github.com/aliyun/terraform-provider-alicloud/issues/4239))
- **New Data Source:** `alicloud_direct_mail_tags`([#4178](https://github.com/aliyun/terraform-provider-alicloud/issues/4178))
- **New Data Source:** `alicloud_ecd_desktops`([#4199](https://github.com/aliyun/terraform-provider-alicloud/issues/4199))
- **New Data Source:** `alicloud_cloud_storage_gateway_gateway_cache_disks`([#4217](https://github.com/aliyun/terraform-provider-alicloud/issues/4217))
- **New Data Source:** `data_source_alicloud_cloud_storage_gateway_stocks`([#4224](https://github.com/aliyun/terraform-provider-alicloud/issues/4224)) 
- **New Data Source:** `alicloud_cloud_storage_gateway_gateway_file_shares`([#4231](https://github.com/aliyun/terraform-provider-alicloud/issues/4231))
- **New Data Source:** `alicloud_cloud_storage_gateway_gateway_block_volumes`([#4234](https://github.com/aliyun/terraform-provider-alicloud/issues/4234))
- **New Data Source:** `alicloud_cloud_storage_gateway_express_syncs`([#4239](https://github.com/aliyun/terraform-provider-alicloud/issues/4239))

ENHANCEMENTS:

- resource/alicloud_ram_role: Support updating the filed description([#4212](https://github.com/aliyun/terraform-provider-alicloud/issues/4212))
- resource/alicloud_instance: Support configuring the filed hpc_cluster_id([#4214](https://github.com/aliyun/terraform-provider-alicloud/issues/4214))
- resource/alicloud_msc_sub_contact: Support setting Chinese contact name,Change position to take Others to Other([#4221](https://github.com/aliyun/terraform-provider-alicloud/issues/4221))
- resource/alicloud_instance: Supports configuring the secondary_private_ips for primary network interface([#4223](https://github.com/aliyun/terraform-provider-alicloud/issues/4223))
- resource/alicloud_instance: Support the secondary_private_ips 's retry process([#4228](https://github.com/aliyun/terraform-provider-alicloud/issues/4228))
- docs: Improves the Config's available region in the documentation([#4238](https://github.com/aliyun/terraform-provider-alicloud/issues/4238))

BUG FIXES:

- resource/alicloud_slb_listener: Fixes the importing diff error caused by delete_protection_validation and health_check_http_code default value([#4240](https://github.com/aliyun/terraform-provider-alicloud/issues/4240))

## 1.143.0 (November 14, 2021)

- **New Resource:** `alicloud_vpc_ipv6_internet_bandwidth`([#4176](https://github.com/aliyun/terraform-provider-alicloud/issues/4176))
- **New Resource:** `alicloud_pvtz_endpoint`([#4177](https://github.com/aliyun/terraform-provider-alicloud/issues/4177))
- **New Resource:** `alicloud_simple_application_server_firewall_rule`([#4183](https://github.com/aliyun/terraform-provider-alicloud/issues/4183))
- **New Resource:** `alicloud_pvtz_rule_attachment`([#4185](https://github.com/aliyun/terraform-provider-alicloud/issues/4185))
- **New Resource:** `alicloud_pvtz_rules`([#4185](https://github.com/aliyun/terraform-provider-alicloud/issues/4185))
- **New Resource:** `alicloud_simple_application_server_snapshot`([#4196](https://github.com/aliyun/terraform-provider-alicloud/issues/4196))
- **New Resource:** `alicloud_simple_application_server_custom_image`([#4205](https://github.com/aliyun/terraform-provider-alicloud/issues/4205))
- **New Data Source:** `alicloud_vpc_ipv6_internet_bandwidths`([#4176](https://github.com/aliyun/terraform-provider-alicloud/issues/4176))
- **New Data Source:** `alicloud_pvtz_endpoints`([#4177](https://github.com/aliyun/terraform-provider-alicloud/issues/4177))
- **New Data Source:** `alicloud_pvtz_resolver_zones`([#4177](https://github.com/aliyun/terraform-provider-alicloud/issues/4177)) 
- **New Data Source:** `alicloud_simple_application_server_firewall_rules`([#4183](https://github.com/aliyun/terraform-provider-alicloud/issues/4183))
- **New Data Source:** `alicloud_pvtz_rules`([#4185](https://github.com/aliyun/terraform-provider-alicloud/issues/4185))
- **New Data Source:** `alicloud_simple_application_server_snapshots`([#4196](https://github.com/aliyun/terraform-provider-alicloud/issues/4196))
- **New Data Source:** `alicloud_simple_application_server_disks`([#4196](https://github.com/aliyun/terraform-provider-alicloud/issues/4196))
- **New Data Source:** `alicloud_ecd_bundles`([#4202](https://github.com/aliyun/terraform-provider-alicloud/issues/4202))
- **New Data Source:** `alicloud_simple_application_server_custom_images`([#4205](https://github.com/aliyun/terraform-provider-alicloud/issues/4205))

ENHANCEMENTS:

- resource/alicloud_ess_scalingconfiguration: Adds new attributes host_name([#4180](https://github.com/aliyun/terraform-provider-alicloud/issues/4180))
- resource/alicloud_cloud_sso_access_configuration: add regular check resource/alicloud_cloud_sso_directory : add regular check, Support separate update of saml_identity_provider_configuration property([#4193](https://github.com/aliyun/terraform-provider-alicloud/issues/4193))
- resource/alicloud_cloud_sso_group: add regular check resource/alicloud_cloud_sso_user: add regular chec([#4193](https://github.com/aliyun/terraform-provider-alicloud/issues/4193))
- resource/bastionhost_instance: Add new field enable_public_access([#4206](https://github.com/aliyun/terraform-provider-alicloud/issues/4206))
- resource/alicloud_simple_application_server_custom_image_test:Optimize test cases.([#4208](https://github.com/aliyun/terraform-provider-alicloud/issues/4208))
- resource/alicloud_simple_application_server_snapshot_test:Optimize test cases.([#4208](https://github.com/aliyun/terraform-provider-alicloud/issues/4208))
- Github WorkFlow: Add markdown-terraform-format && markdown-terraform-validate([#4184](https://github.com/aliyun/terraform-provider-alicloud/issues/4184))
- Github WorkFlow: Add markdown-terraform-format([#4190](https://github.com/aliyun/terraform-provider-alicloud/issues/4190))
- docs/alicloud_log_store: Improves its documentation([#4186](https://github.com/aliyun/terraform-provider-alicloud/issues/4186))

BUG FIXES:

- resource/alicloud_db_clone_instances:fix bug about not filter securityIps by DBInstanceIPArrayName([#4182](https://github.com/aliyun/terraform-provider-alicloud/issues/4182))
- datasource/alicloud_alb_server_groups: Fix the issue of enable_details export error([#4181](https://github.com/aliyun/terraform-provider-alicloud/issues/4181))
- doc/alicloud_cloud_storage_gateway_gateway_smb_user: Fixes the title error([#4187](https://github.com/aliyun/terraform-provider-alicloud/issues/4187))
- bug/alicloud_cms_monitor_group_instances: Fix the problem that cannot be imported when the number of instances exceeds 30([#4203](https://github.com/aliyun/terraform-provider-alicloud/issues/4203))

## 1.142.0 (November 7, 2021)

- **New Resource:** `alicloud_ecd_user`([#4126](https://github.com/aliyun/terraform-provider-alicloud/issues/4126))
- **New Resource:** `alicloud_vpc_traffic_mirror_session`([#4156](https://github.com/aliyun/terraform-provider-alicloud/issues/4156))
- **New Resource:** `alicloud_gpdb_account`([#4158](https://github.com/aliyun/terraform-provider-alicloud/issues/4158)) 
- **New Resource:** `alicloud_security_center_slr`([#4159](https://github.com/aliyun/terraform-provider-alicloud/issues/4159))
- **New Resource:** `alicloud_vpc_ipv6_gateway`([#4161](https://github.com/aliyun/terraform-provider-alicloud/issues/4161))
- **New Resource:** `alicloud_vpc_ipv6_egress_rule`([#4167](https://github.com/aliyun/terraform-provider-alicloud/issues/4167))
- **New Resource:** `alicloud_event_bridge_service_linked_role`([#4159](https://github.com/aliyun/terraform-provider-alicloud/issues/4159))  
- **New Resource:** `alicloud_ecd_network_package`([#4153](https://github.com/aliyun/terraform-provider-alicloud/issues/4153))
- **New Resource:** `alicloud_cms_dynamic_tag_group`([#4160](https://github.com/aliyun/terraform-provider-alicloud/issues/4160)) 
- **New Resource:** `alicloud_cloud_storage_gateway_gateway_smb_user`([#4163](https://github.com/aliyun/terraform-provider-alicloud/issues/4163))
- **New Data Source:** `alicloud_ecd_users`([#4126](https://github.com/aliyun/terraform-provider-alicloud/issues/4126))  
- **New Data Source:** `alicloud_vpc_traffic_mirror_sessions`([#4156](https://github.com/aliyun/terraform-provider-alicloud/issues/4156))
- **New Data Source:** `alicloud_gpdb_accounts`([#4158](https://github.com/aliyun/terraform-provider-alicloud/issues/4158))
- **New Data Source:** `alicloud_vpc_ipv6_gateways`([#4161](https://github.com/aliyun/terraform-provider-alicloud/issues/4161))
- **New Data Source:** `alicloud_vpc_ipv6_egress_rules`([#4167](https://github.com/aliyun/terraform-provider-alicloud/issues/4167))
- **New Data Source:** `alicloud_vpc_ipv6_addresses`([#4167](https://github.com/aliyun/terraform-provider-alicloud/issues/4167))
- **New Data Source:** `alicloud_ecd_network_packages`([#4153](https://github.com/aliyun/terraform-provider-alicloud/issues/4153))
- **New Data Source:** `alicloud_cms_dynamic_tag_groups`([#4160](https://github.com/aliyun/terraform-provider-alicloud/issues/4160))
- **New Data Source:** `alicloud_cloud_storage_gateway_gateway_smb_users`([#4163](https://github.com/aliyun/terraform-provider-alicloud/issues/4163))

ENHANCEMENTS:

- resource/alicloud_cloud_storage_gateway_gateway_smb_user: Adds waiting codes to wait the task is completed([#4175](https://github.com/aliyun/terraform-provider-alicloud/issues/4175))
- resource/alicloud_ecd_user: redefine connectivity EcdUserSupportRegions; data_source/alicloud_ecd_users: redefine connectivity EcdUserSupportRegions([#4162](https://github.com/aliyun/terraform-provider-alicloud/issues/4162))
- resource/alicloud_event_bridge_service_sle: After the version 1.142.0, the resource is renamed as alicloud_event_bridge_service_linked_role.([#4159](https://github.com/aliyun/terraform-provider-alicloud/issues/4159))
- resource/alicloud_ecs_network_interface: Add delete error retry code InvalidOperation.Conflict([#4173](https://github.com/aliyun/terraform-provider-alicloud/issues/4173))  
- datasource/alicloud_dataworks_service: Renames to alicloud_data_works_service; docs: Improves the docs subcategory([#4157](https://github.com/aliyun/terraform-provider-alicloud/issues/4157))
- Github WorkFlow: Add markdown-link-check && markdown-spell-check([#4166](https://github.com/aliyun/terraform-provider-alicloud/issues/4166))

BUG FIXES:

- datasource/alicloud_alb_load_balancers: fix load_balancer_business_status spelling error([#4170](https://github.com/aliyun/terraform-provider-alicloud/issues/4170))
- docs: Fixes the spelling error([#4169](https://github.com/aliyun/terraform-provider-alicloud/issues/4169))

## 1.141.0 (October 31, 2021)

- **New Resource:** `alicloud_waf_protection_module`([#4143](https://github.com/aliyun/terraform-provider-alicloud/issues/4143))
- **New Resource:** `alicloud_vpc_traffic_mirror_service`([#4134](https://github.com/aliyun/terraform-provider-alicloud/issues/4134))
- **New Resource:** `alicloud_msc_sub_webhook`([#4138](https://github.com/aliyun/terraform-provider-alicloud/issues/4138))
- **New Resource:** `alicloud_ecd_nas_file_system`([#4139](https://github.com/aliyun/terraform-provider-alicloud/issues/4139))  
- **New Resource:** `alicloud_cloud_sso_user_attachment`([#4140](https://github.com/aliyun/terraform-provider-alicloud/issues/4140))   
- **New Resource:** `alicloud_cloud_sso_access_assignment`([#4140](https://github.com/aliyun/terraform-provider-alicloud/issues/4140))
- **New Data Source:** `alicloud_msc_sub_webhooks`([#4138](https://github.com/aliyun/terraform-provider-alicloud/issues/4138))
- **New Data Source:** `alicloud_ecd_nas_file_systems`([#4139](https://github.com/aliyun/terraform-provider-alicloud/issues/4139)) 

ENHANCEMENTS:

- datasource/alicloud_dataworks_service: Renames to alicloud_data_works_service; docs: Improves the docs subcategory([#4157](https://github.com/aliyun/terraform-provider-alicloud/issues/4157))
- resource/alicloud_ess_scaling_group: supports configurating launch_template_id([#4133](https://github.com/aliyun/terraform-provider-alicloud/issues/4133))
- resource/alicloud_eci_container_group: supports configurating image_registry_credential([#4137](https://github.com/aliyun/terraform-provider-alicloud/issues/4137))
- resource/alicloud_mhub_app: redefine connectivity MHUBsupportregions([#4139](https://github.com/aliyun/terraform-provider-alicloud/issues/4139))
- resource/alicloud_config_aggregate_compliance_pack : Modify the parameter compliance_pack_template_id to optional, Field config_rules has been deprecated from provider version 1.141.0. New field config_rule_ids' instead.([#4141](https://github.com/aliyun/terraform-provider-alicloud/issues/4141))
- resource/alicloud_config_aggregate_config_rule: Add the output parameter config_rule_id([#4141](https://github.com/aliyun/terraform-provider-alicloud/issues/4141))  
- resource/alicloud_config_compliance_pack : Modify the parameter compliance_pack_template_id to optional, Field config_rules has been deprecated from provider version 1.141.0. New field config_rule_ids' instead([#4141](https://github.com/aliyun/terraform-provider-alicloud/issues/4141))
- resource/alicloud_mongodb_instance: support auto_renew field resource/alicloud_mongodb_sharding_instance: support auto_renew field and transforming charge_type from Postpaid to Prepaid([#4146](https://github.com/aliyun/terraform-provider-alicloud/issues/4146)) 
- resource/alicloud_monitor_group: support creating MonitorGroup By resource_group_id([#4147](https://github.com/aliyun/terraform-provider-alicloud/issues/4147))
- resource/alicloud_cs_managed_kubernetes: supports control plane log collection and retain resources when destroy cluster([#4154](https://github.com/aliyun/terraform-provider-alicloud/issues/4154))  
- data_source/alicloud_mhub_apps: redefine connectivity MHUBsupportregions([#4139](https://github.com/aliyun/terraform-provider-alicloud/issues/4139))
- provider: Adds new parameter credentials_uri to support sidecar credentials([#4142](https://github.com/aliyun/terraform-provider-alicloud/issues/4142))
- doc/alicloud_cloud_sso_directory : Optimize document format doc/alicloud_cloud_sso_access_configuration : Optimize document format resource/alicloud_cloud_sso_user : Modify the parameter user_name as required([#4152](https://github.com/aliyun/terraform-provider-alicloud/issues/4152))


BUG FIXES:

- provider: Fixes the undefined: io.ReadAll error([#4145](https://github.com/aliyun/terraform-provider-alicloud/issues/4145))

## 1.140.0 (October 24, 2021)

- **New Resource:** `alicloud_ecd_simple_office_site`([#4129](https://github.com/aliyun/terraform-provider-alicloud/issues/4129))
- **New Resource:** `alicloud_cloud_sso_access_configuration`([#4109](https://github.com/aliyun/terraform-provider-alicloud/issues/4109))
- **New Resource:** `alicloud_dfs_file_system`([#4112](https://github.com/aliyun/terraform-provider-alicloud/issues/4112)) 
- **New Resource:** `alicloud_vpc_traffic_mirror_filter`([#4113](https://github.com/aliyun/terraform-provider-alicloud/issues/4113)) 
- **New Resource:** `alicloud_dfs_access_rule`([#4116](https://github.com/aliyun/terraform-provider-alicloud/issues/4116)) 
- **New Resource:** `alicloud_dfs_mount_point`([#4118](https://github.com/aliyun/terraform-provider-alicloud/issues/4118)) 
- **New Resource:** `alicloud_vpc_traffic_mirror_filter_egress_rule`([#4119](https://github.com/aliyun/terraform-provider-alicloud/issues/4119))
- **New Data Source:** `alicloud_ecd_simple_office_sites`([#4129](https://github.com/aliyun/terraform-provider-alicloud/issues/4129))
- **New Data Source:** `alicloud_cloud_sso_access_configurations`([#4109](https://github.com/aliyun/terraform-provider-alicloud/issues/4109))
- **New Data Source:** `alicloud_dfs_zones`([#4112](https://github.com/aliyun/terraform-provider-alicloud/issues/4112))
- **New Data Source:** `alicloud_dfs_file_systems`([#4112](https://github.com/aliyun/terraform-provider-alicloud/issues/4112)) 
- **New Data Source:** `alicloud_vpc_traffic_mirror_filters`([#4113](https://github.com/aliyun/terraform-provider-alicloud/issues/4113)) 
- **New Data Source:** `alicloud_dfs_access_rules`([#4116](https://github.com/aliyun/terraform-provider-alicloud/issues/4116))
- **New Data Source:** `alicloud_dfs_mount_points`([#4118](https://github.com/aliyun/terraform-provider-alicloud/issues/4118))
- **New Data Source:** `alicloud_nas_zones`([#4120](https://github.com/aliyun/terraform-provider-alicloud/issues/4120))
- **New Data Source:** `alicloud_vpc_traffic_mirror_filter_egress_rules`([#4127](https://github.com/aliyun/terraform-provider-alicloud/issues/4127))

ENHANCEMENTS:

- resource/alicloud_ecd_simple_office_site: Optimize testcase parameter && doc/alicloud_vs_service: Optimize the page layout([#4131](https://github.com/aliyun/terraform-provider-alicloud/issues/4131))
- resource/alicloud_eip_address: Support prepaid instances to set the auto_pay field([#4130](https://github.com/aliyun/terraform-provider-alicloud/issues/4130))
- resource/alicloud_waf_instance: Adds new attribute region; resource/alicloud_waf_domain: Adds retry strategy to avoid ThrottlingUser error([#4110](https://github.com/aliyun/terraform-provider-alicloud/issues/4110))
- resource/alicloud_mongodb_instance support querying replica_sets([#4114](https://github.com/aliyun/terraform-provider-alicloud/issues/4114))
- resource/alicloud_mongodb_sharding_instance support querying config_server_list([#4114](https://github.com/aliyun/terraform-provider-alicloud/issues/4114))
- resource/alicloud_api_gateway_api: Support API replay attacks.([#4115](https://github.com/aliyun/terraform-provider-alicloud/issues/4115))
- resource/alicloud_nas_file_system: Adds new attribute zone_id([#4120](https://github.com/aliyun/terraform-provider-alicloud/issues/4120))
- resource/alicloud_eip_address: Support prepaid instances to set the auto_pay field([#4122](https://github.com/aliyun/terraform-provider-alicloud/issues/4122)) 
- datasource/vpc_traffic_mirror_filters: Remove egress_rules and ingress_rules in its outputs([#4124](https://github.com/aliyun/terraform-provider-alicloud/issues/4124))
- doc/actiontrail_history_delivery_job: Optimize document format doc/actiontrail_history_delivery_jobs: Optimize document format([#4111](https://github.com/aliyun/terraform-provider-alicloud/issues/4111))

BUG FIXES:

- resource/alicloud_cloud_sso_directory: Fix the problem of dependency property saml_identity_provider_configuration when deleting([#4109](https://github.com/aliyun/terraform-provider-alicloud/issues/4109))

## 1.139.0 (October 17, 2021)

- **New Resource:** `alicloud_cloud_firewall_instance`([#4102](https://github.com/aliyun/terraform-provider-alicloud/issues/4102))
- **New Resource:** `alicloud_actiontrail_history_delivery_job`([#4101](https://github.com/aliyun/terraform-provider-alicloud/issues/4101))
- **New Resource:** `alicloud_cr_instance_endpoint_acl_policy`([#4087](https://github.com/aliyun/terraform-provider-alicloud/issues/4087))
- **New Data Source:** `alicloud_sae_instance_specifications`([#4103](https://github.com/aliyun/terraform-provider-alicloud/issues/4103)) 
- **New Data Source:** `alicloud_cloud_firewall_instances`([#4102](https://github.com/aliyun/terraform-provider-alicloud/issues/4102))
- **New Data Source:** `alicloud_actiontrail_history_delivery_jobs`([#4101](https://github.com/aliyun/terraform-provider-alicloud/issues/4101))
- **New Data Source:** `alicloud_cen_transit_router_service`([#4092](https://github.com/aliyun/terraform-provider-alicloud/issues/4092))
- **New Data Source:** `alicloud_cr_instance_endpoint_acl_policies`([#4087](https://github.com/aliyun/terraform-provider-alicloud/issues/4087))
- **New Data Source:** `alicloud_cr_endpoint_acl_service`([#4087](https://github.com/aliyun/terraform-provider-alicloud/issues/4087))

ENHANCEMENTS:

- resource/alicloud_waf_instance: Adds new attribute region; resource/alicloud_waf_domain: Adds retry strategy to avoid ThrottlingUser error([#4110](https://github.com/aliyun/terraform-provider-alicloud/issues/4110))
- Github WorkFlow: Add precheck format && golang-ci-lint([#4106](https://github.com/aliyun/terraform-provider-alicloud/issues/4106))
- resource/alicloud_dts_synchronization_instance: modify additional input parameters for the createInstance API, make AutoPay to false([#4081](https://github.com/aliyun/terraform-provider-alicloud/issues/4081))
- resource/alicloud_hbr_backup_client, resource/alicloud_hbr_ecs_backup_plan, resource/alicloud_hbr_oss_backup_plan, resource/alicloud_hbr_nas_backup_plan, resource/alicloud_hbr_restore_job, resource/alicloud_hbr_vault and theirs datasource: Improves the attribute value, test case and documents([#4080](https://github.com/aliyun/terraform-provider-alicloud/issues/4080))
- doc/alicloud_common_bandwidth_package: Optimize document format resource/alicloud_eip_address: Support internet charge type PayByDominantTraffic([#4082](https://github.com/aliyun/terraform-provider-alicloud/issues/4082))
- testcase: Improves the testcase when changing region([#4099](https://github.com/aliyun/terraform-provider-alicloud/issues/4099))
- resource/alicloud_hbr_nas_backup_plan:Improvement DetachNasFileSystem([#4096](https://github.com/aliyun/terraform-provider-alicloud/issues/4096))
- docs/alicloud_route_entry: Supports two new nexthop type IPv6Gateway and Attachment([#4091](https://github.com/aliyun/terraform-provider-alicloud/issues/4091))
- doc/alicloud_cr_ee_instance: Optimize document format([#4087](https://github.com/aliyun/terraform-provider-alicloud/issues/4087))
- datasource/alicloud_alb_listeners: Fix the bug of parameter certifiates output doc/alicloud_alb_listener: Optimize document format doc/alicloud_alb_listeners: Optimize document format([#4083](https://github.com/aliyun/terraform-provider-alicloud/issues/4083))
- resource/alicloud_dts_synchronization_instance: modify additional input parameters for the createInstance API, make AutoPay to false; docs/alicloud_dts_synchronization_instance, alicloud_dts_synchronization_job: fix examples.([#4081](https://github.com/aliyun/terraform-provider-alicloud/issues/4081))
- resource/alicloud_hbr_backup_client, resource/alicloud_hbr_ecs_backup_plan, resource/alicloud_hbr_oss_backup_plan, resource/alicloud_hbr_nas_backup_plan, resource/alicloud_hbr_restore_job, resource/alicloud_hbr_vault and theirs datasource: Improves the attribute value, test case and documents.([#4080](https://github.com/aliyun/terraform-provider-alicloud/issues/4080))
- resource/alicloud_sae_application: supports updating Slb([#4035](https://github.com/aliyun/terraform-provider-alicloud/issues/4035))

BUG FIXES:

- datasource/alicloud_bastionhost_users: Fixes the status without output error([#4084](https://github.com/aliyun/terraform-provider-alicloud/issues/4084))
- datasource/alicloud_alb_listeners: Fix the bug of parameter certifiates output doc/alicloud_alb_listener: Optimize document format doc/alicloud_alb_listeners: Optimize document format([#4083](https://github.com/aliyun/terraform-provider-alicloud/issues/4083))
- docs/alicloud_dts_synchronization_instance, alicloud_dts_synchronization_job: fix examples.([#4081](https://github.com/aliyun/terraform-provider-alicloud/issues/4081))

## 1.138.0 (September 30, 2021)

- **New Resource:**  `alicloud_dts_subscription_job`([#4068](https://github.com/aliyun/terraform-provider-alicloud/issues/4068))
- **New Resource:**  `alicloud_dts_synchronization_instance`([#4068](https://github.com/aliyun/terraform-provider-alicloud/issues/4068))
- **New Resource:**  `alicloud_pvtz_user_vpc_authorization`([#4052](https://github.com/aliyun/terraform-provider-alicloud/issues/4052))
- **New Resource:**  `alicloud_mhub_product`([#4047](https://github.com/aliyun/terraform-provider-alicloud/issues/4047)) 
- **New Resource:**  `alicloud_dts_subscription_job`([#4017](https://github.com/aliyun/terraform-provider-alicloud/issues/4017))
- **New Resource:**  `alicloud_cloud_sso_scim_server_credential`([#4064](https://github.com/aliyun/terraform-provider-alicloud/issues/4064))
- **New Resource:**  `alicloud_service_mesh_service_mesh`([#4059](https://github.com/aliyun/terraform-provider-alicloud/issues/4059))
- **New Resource:**  `alicloud_mhub_app`([#4062](https://github.com/aliyun/terraform-provider-alicloud/issues/4062))
- **New Resource:**  `alicloud_cloud_sso_group`([#4063](https://github.com/aliyun/terraform-provider-alicloud/issues/4063))
- **New Data Source:**  `alicloud_dts_subscription_jobs`([#4068](https://github.com/aliyun/terraform-provider-alicloud/issues/4068))
- **New Data Source:** `alicloud_click_house_regions`([#4065](https://github.com/aliyun/terraform-provider-alicloud/issues/4065))
- **New Data Source:** `alicloud_mhub_products`([#4047](https://github.com/aliyun/terraform-provider-alicloud/issues/4047))
- **New Data Source:** `alicloud_dts_subscription_jobs`([#4017](https://github.com/aliyun/terraform-provider-alicloud/issues/4017))
- **New Data Source:** `alicloud_cloud_sso_scim_server_credentials`([#4064](https://github.com/aliyun/terraform-provider-alicloud/issues/4064))
- **New Data Source:** `alicloud_service_mesh_service_meshes`([#4059](https://github.com/aliyun/terraform-provider-alicloud/issues/4059))
- **New Data Source:** `alicloud_mhub_apps`([#4062](https://github.com/aliyun/terraform-provider-alicloud/issues/4062))
- **New Data Source:** `alicloud_cloud_sso_groups`([#4063](https://github.com/aliyun/terraform-provider-alicloud/issues/4063))
- **New Data Source:** `alicloud_hbr_backup_jobs`([#3950](https://github.com/aliyun/terraform-provider-alicloud/issues/3950))

ENHANCEMENTS:

- resource/alicloud_mhub_app: Setting the PreCheck after getting the resource([#4072](https://github.com/aliyun/terraform-provider-alicloud/issues/4072))
- resource/alicloud_hbr_ecs_backup_plan,resource/alicloud_hbr_nas_backup_plan,resource/alicloud_hbr_oss_backup_plan: adjust the property backup_type and it's document.([#3950](https://github.com/aliyun/terraform-provider-alicloud/issues/3950))
- resource/alicloud_db_instance,alicloud_kvstore_instance: Improves the waiting time after modifying the security_ips([#4070](https://github.com/aliyun/terraform-provider-alicloud/issues/4070))
- resource/alicloud_cs_serverless_kubernetes: Setting the attribute vswitch_ids after getting the resource([#4058](https://github.com/aliyun/terraform-provider-alicloud/issues/4058))
- resource/alicloud_config_aggregator: Adjust the state judgment when the resource is created([#4057](https://github.com/aliyun/terraform-provider-alicloud/issues/4057))
- resource/alicloud_config_aggregate_compliance_pack : Adjust the state judgment when the resource is create or update([#4057](https://github.com/aliyun/terraform-provider-alicloud/issues/4057))
- resource/alicloud_config_compliance_pack : Adjust the state judgment when the resource is create or update([#4057](https://github.com/aliyun/terraform-provider-alicloud/issues/4057))
- resource/alicloud_image_copy: Removes the cancelCopyImage action([#4061](https://github.com/aliyun/terraform-provider-alicloud/issues/4061)) 
- resource/alicloud_hbr_ecs_backup_client: optimize creation timeout and it's test case;([#3950](https://github.com/aliyun/terraform-provider-alicloud/issues/3950))
- data_source/data_source_alicloud_hbr_snapshots: optimized property "status"and its docs; ([#3950](https://github.com/aliyun/terraform-provider-alicloud/issues/3950))
- provider: Supports new region ap-southeast-6([#4071](https://github.com/aliyun/terraform-provider-alicloud/issues/4071))
- sweeper test: Improves the cen sweeper testcases([#4060](https://github.com/aliyun/terraform-provider-alicloud/issues/4060))
- Adds a new resource alicloud_imp_app_template and datasource alicloud_imp_app_templates([#4049](https://github.com/aliyun/terraform-provider-alicloud/issues/4049))

BUG FIXES:

- resource/alicloud_vpn_customer_gateway: Fixes the OperationConflict error while creating it([#4056](https://github.com/aliyun/terraform-provider-alicloud/issues/4056))
- resource/alicloud_bastionhost_user_attachment: Fixes the Commodity.BizError.InvalidStatus error while deleting the resource([#4067](https://github.com/aliyun/terraform-provider-alicloud/issues/4067))
- resource/alicloud_cs_edge_kubernetes: Fixes the diff error caused by attribute resource_group_id; Improves the some testcases([#4055](https://github.com/aliyun/terraform-provider-alicloud/issues/4055))
- Doc/cloud_firewall: fix typo in cloud firewall demo code([#4030](https://github.com/aliyun/terraform-provider-alicloud/issues/4030))

## 1.137.0 (September 26, 2021)

- **New Resource:**  `alicloud_imp_app_template`([#4049](https://github.com/aliyun/terraform-provider-alicloud/issues/4049))
- **New Resource:**  `alicloud_rdc_organization`([#4013](https://github.com/aliyun/terraform-provider-alicloud/issues/4013))
- **New Resource:**  `alicloud_eais_instance`([#4032](https://github.com/aliyun/terraform-provider-alicloud/issues/4032))
- **New Resource:**  `alicloud_sae_ingress`([#3911](https://github.com/aliyun/terraform-provider-alicloud/issues/3911))
- **New Data Source:** `alicloud_imp_app_templates`([#4049](https://github.com/aliyun/terraform-provider-alicloud/issues/4049))
- **New Data Source:** `alicloud_rdc_organizations`([#4013](https://github.com/aliyun/terraform-provider-alicloud/issues/4013))
- **New Data Source:** `alicloud_eais_instances`([#4032](https://github.com/aliyun/terraform-provider-alicloud/issues/4032))
- **New Data Source:** `alicloud_sae_ingresses`([#3911](https://github.com/aliyun/terraform-provider-alicloud/issues/3911))

ENHANCEMENTS:

- resource/alicloud_vpc_dhcp_options_set: Optimize resource creation([#4033](https://github.com/aliyun/terraform-provider-alicloud/issues/4033))
- doc/common_bandwidth_package: Adjust document position doc/eipanycast_anycast_eip_address: Adjust document position([#4029](https://github.com/aliyun/terraform-provider-alicloud/issues/4029))
- testcase: Improves the rds testcases([#4045](https://github.com/aliyun/terraform-provider-alicloud/issues/4045))
- sdk: Upgrades the sdk tea-rpc to 1.2.0 and tea-roa to 1.3.0 to support parameters SourceIp and SecureTransport([#4044](https://github.com/aliyun/terraform-provider-alicloud/issues/4044))
- provider: Enlarges the read_timeout and connect_timeout to 60s([#4043](https://github.com/aliyun/terraform-provider-alicloud/issues/4043))
- resource/alicloud_db_instance: Sets the attribute zone_id_slave_a to computed to fix the diff error([#4042](https://github.com/aliyun/terraform-provider-alicloud/issues/4042))
- resource/alicloud_rds_account: Adds UnlockAccount action to fix the Lock error when deleting PostgreSQL database account([#4040](https://github.com/aliyun/terraform-provider-alicloud/issues/4040))
- testcase:Fix vpc,vswithc,fc sweepers([#4038](https://github.com/aliyun/terraform-provider-alicloud/issues/4038))

BUG FIXES:

- resource/alicloud_log_oss_shipper: Fixes the ShipperNotExist error while deleting the resource([#4048](https://github.com/aliyun/terraform-provider-alicloud/issues/4048))
- resource/alicloud_cen_instance: Fixes the setting name bug; datasource/alicloud_ots_instance_attachments: Fixes the code bug while checking whether error is nil([#4046](https://github.com/aliyun/terraform-provider-alicloud/issues/4046))
- resource/alicloud_route_table: Fixes the OperationConflict error when creating a new table([#4041](https://github.com/aliyun/terraform-provider-alicloud/issues/4041))
- datasource/alicloud_db_instance_classes: Fixes the db_instance_storage_type bug; datasource/alicloud_db_zones: Fixes the multi bug([#4039](https://github.com/aliyun/terraform-provider-alicloud/issues/4039))

## 1.136.0 (September 13, 2021)

- **New Resource:**  `alicloud_dbfs_instance`([#4024](https://github.com/aliyun/terraform-provider-alicloud/issues/4024))
- **New Resource:**  `alicloud_sddp_instance`([#3997](https://github.com/aliyun/terraform-provider-alicloud/issues/3997))
- **New Resource:**  `alicloud_vpc_nat_ip_cidr`([#4005](https://github.com/aliyun/terraform-provider-alicloud/issues/4005))
- **New Resource:**  `alicloud_vpc_nat_ip`([#4015](https://github.com/aliyun/terraform-provider-alicloud/issues/4015))
- **New Resource:**  `alicloud_quick_bi_user`([#4007](https://github.com/aliyun/terraform-provider-alicloud/issues/4007))
- **New Resource:**  `alicloud_vod_domain`([#4006](https://github.com/aliyun/terraform-provider-alicloud/issues/4006))
- **New Resource:**  `alicloud_arms_dispatch_rule`([#4006](https://github.com/aliyun/terraform-provider-alicloud/issues/4006))
- **New Resource:**  `alicloud_open_search_app_group`([#4021](https://github.com/aliyun/terraform-provider-alicloud/issues/4021))
- **New Resource:**  `alicloud_graph_database_db_instance`([#4020](https://github.com/aliyun/terraform-provider-alicloud/issues/4020))
- **New Resource:**  `alicloud_arms_prometheus_alert_rule`([#4022](https://github.com/aliyun/terraform-provider-alicloud/issues/4022))
- **New Data Source:** `alicloud_dbfs_instances`([#4024](https://github.com/aliyun/terraform-provider-alicloud/issues/4024))
- **New Data Source:** `alicloud_sddp_instances`([#3997](https://github.com/aliyun/terraform-provider-alicloud/issues/3997))
- **New Data Source:** `alicloud_vpc_nat_ip_cidrs`([#4005](https://github.com/aliyun/terraform-provider-alicloud/issues/4005))
- **New Data Source:** `alicloud_vpc_nat_ips`([#4015](https://github.com/aliyun/terraform-provider-alicloud/issues/4015))
- **New Data Source:** `alicloud_quick_bi_users`([#4007](https://github.com/aliyun/terraform-provider-alicloud/issues/4007))
- **New Data Source:** `alicloud_vod_domains`([#4006](https://github.com/aliyun/terraform-provider-alicloud/issues/4006))
- **New Data Source:** `alicloud_arms_dispatch_rules`([#4023](https://github.com/aliyun/terraform-provider-alicloud/issues/4023))
- **New Data Source:** `alicloud_open_search_app_groups`([#4021](https://github.com/aliyun/terraform-provider-alicloud/issues/4021))
- **New Data Source:** `alicloud_graph_database_db_instances`([#4020](https://github.com/aliyun/terraform-provider-alicloud/issues/4020))  
- **New Data Source:** `alicloud_arms_prometheus_alert_rules`([#4022](https://github.com/aliyun/terraform-provider-alicloud/issues/4022))

ENHANCEMENTS:

- resource/alicloud_db_instances: Adds attribute db_time_zone to set time zone of the instance.([#4003](https://github.com/aliyun/terraform-provider-alicloud/issues/4003))
- resource/alicloud_db_instances: Adds attribute released_keep_policy to set the policy of the backup files after the instance is released.([#4008](https://github.com/aliyun/terraform-provider-alicloud/issues/4008))
- resource/alicloud_alb_listeners: Adds new attribute acl_config to set associate acls([#3979](https://github.com/aliyun/terraform-provider-alicloud/issues/3979))
- resource/alicloud_waf_certificate: Adds new attribute certificate_id to support uploading a certificate from ssl([#4011](https://github.com/aliyun/terraform-provider-alicloud/issues/4011))
- resource/alicloud_nat_gateway: Adds new attribute network_type to support create Vpc NatGateway([#4012](https://github.com/aliyun/terraform-provider-alicloud/issues/4012))
- resource/alicloud_image: Adds new attribute delete_auto_snapshot to automatically delete dependence snapshots while deleting image([#4025](https://github.com/aliyun/terraform-provider-alicloud/issues/4025))
- doc/alicloud_instance: Optimize system_disk_performance_level parameter([#4009](https://github.com/aliyun/terraform-provider-alicloud/issues/4009))
- sdk/alibaba-cloud-go-sdk: Upgrades the sdk to v1.61.1264([#4026](https://github.com/aliyun/terraform-provider-alicloud/issues/4026))
- testcase/alicloud_db_instance: Improves the rds testcases([#4028](https://github.com/aliyun/terraform-provider-alicloud/issues/4028))

BUG FIXES:

- resource/alicloud_cr_ee_instance: Fix the problem of import failure in the international station([#4014](https://github.com/aliyun/terraform-provider-alicloud/issues/4014))

## 1.135.0 (September 13, 2021)

- **New Resource:** `alicloud_bastionhost_host_group_account_user_group_attachment`([#4000](https://github.com/aliyun/terraform-provider-alicloud/issues/4000))
- **New Resource:** `alicloud_bastionhost_host_group_account_user_attachment`([#3999](https://github.com/aliyun/terraform-provider-alicloud/issues/3999))
- **New Resource:** `alicloud_bastionhost_account_user_attachment`([#3998](https://github.com/aliyun/terraform-provider-alicloud/issues/3998))
- **New Resource:** `alicloud_bastionhost_account_user_group_attachment`([#3996](https://github.com/aliyun/terraform-provider-alicloud/issues/3996))
- **New Resource:** `alicloud_msc_sub_subscription`([#3994](https://github.com/aliyun/terraform-provider-alicloud/issues/3994))
- **New Resource:** `alicloud_video_surveillance_system_group`([#3993](https://github.com/aliyun/terraform-provider-alicloud/issues/3993))
- **New Resource:** `alicloud_bastionhost_host_attachment`([#3991](https://github.com/aliyun/terraform-provider-alicloud/issues/3991))
- **New Resource:** `alicloud_bastionhost_host_account`([#3989](https://github.com/aliyun/terraform-provider-alicloud/issues/3989))
- **New Resource:** `alicloud_bastionhost_host`([#3984](https://github.com/aliyun/terraform-provider-alicloud/issues/3984))
- **New Resource:** `alicloud_waf_certificate`([#3982](https://github.com/aliyun/terraform-provider-alicloud/issues/3982))
- **New Resource:** `alicloud_slb_tls_cipher_policy`([#3981](https://github.com/aliyun/terraform-provider-alicloud/issues/3981))
- **New Resource:** `simple_application_server_instance`([#3978](https://github.com/aliyun/terraform-provider-alicloud/issues/3978))
- **New Resource:** `alicloud_slb_tls_cipher_policy`([#3981](https://github.com/aliyun/terraform-provider-alicloud/issues/3981))
- **New Resource:** `alicloud_cloud_sso_directory`([#3972](https://github.com/aliyun/terraform-provider-alicloud/issues/3972))
- **New Resource:** `alicloud_database_gateway_gateway`([#3970](https://github.com/aliyun/terraform-provider-alicloud/issues/3970))
- **New Resource:** `alicloud_dts_jobmonitor_rule`([#3965](https://github.com/aliyun/terraform-provider-alicloud/issues/3965))
- **New Resource:**  `alicloud_direct_mail_mail_address`([#3961](https://github.com/aliyun/terraform-provider-alicloud/issues/3961))
- **New Resource:**  `alicloud_amqp_binding`([#3799](https://github.com/aliyun/terraform-provider-alicloud/issues/3799))
- **New Data Source:** `alicloud_msc_sub_subscriptions`([#3994](https://github.com/aliyun/terraform-provider-alicloud/issues/3994))
- **New Data Source:** `alicloud_video_surveillance_system_groups`([#3993](https://github.com/aliyun/terraform-provider-alicloud/issues/3993))
- **New Data Source:** `alicloud_bastionhost_host_accounts`([#3989](https://github.com/aliyun/terraform-provider-alicloud/issues/3989))
- **New Data Source:** `alicloud_bastionhost_hosts`([#3984](https://github.com/aliyun/terraform-provider-alicloud/issues/3984))
- **New Data Source:** `alicloud_waf_certificates`([#3982](https://github.com/aliyun/terraform-provider-alicloud/issues/3982))
- **New Data Source:** `alicloud_slb_tls_cipher_policies`([#3984](https://github.com/aliyun/terraform-provider-alicloud/issues/3984))
- **New Data Source:** `simple_application_server_instances`([#3978](https://github.com/aliyun/terraform-provider-alicloud/issues/3978))
- **New Data Source:** `alicloud_simple_application_server_images`([#3978](https://github.com/aliyun/terraform-provider-alicloud/issues/3978))
- **New Data Source:** `alicloud_simple_application_server_plans`([#3978](https://github.com/aliyun/terraform-provider-alicloud/issues/3978))
- **New Data Source:** `alicloud_cloud_sso_directories`([#3972](https://github.com/aliyun/terraform-provider-alicloud/issues/3972))
- **New Data Source:** `alicloud_database_gateway_gateways`([#3970](https://github.com/aliyun/terraform-provider-alicloud/issues/3970))
- **New Data Source:** `alicloud_direct_mail_mail_addresses`([#3961](https://github.com/aliyun/terraform-provider-alicloud/issues/3961))
- **New Data Source:** `alicloud_amqp_bindings`([#3799](https://github.com/aliyun/terraform-provider-alicloud/issues/3799))

ENHANCEMENTS:

- resource/alicloud_ess_scalingconfiguration: Support resource_group_id.
- resource/alicloud_image_copy: Supports to cancel image when copying image is timeout; Adds new attribute delete_auto_snapshot to delete snapshot automatically when deleting copied image([#4001](https://github.com/aliyun/terraform-provider-alicloud/issues/4001))
- doc/alicloud_cdn_doamin_config: Optimize document format([#3995](https://github.com/aliyun/terraform-provider-alicloud/issues/3995))
- reource/alicloud_msc_sub_contact: Modify the enumeration value of position and limit Locale to en([#3994](https://github.com/aliyun/terraform-provider-alicloud/issues/3994))
- datasource/alicloud_db_instances: Adds attribute enable_details to show extra parameter template([#3988](https://github.com/aliyun/terraform-provider-alicloud/issues/3988))
- resource/alicloud_bastionhost_instance: Improves the attribute value setting when invoking SetRenewal to update renewal attribute([#3986](https://github.com/aliyun/terraform-provider-alicloud/issues/3986))
- resource/alicloud_ess_scalingconfiguration: Adds new attribute resource_group_id to support set resource group([#3985](https://github.com/aliyun/terraform-provider-alicloud/issues/3985))
- resource/alicloud_log_audit: logservice audit support resource directory([#3983](https://github.com/aliyun/terraform-provider-alicloud/issues/3983))
- datasource/alicloud_db_instance_classes: Upgrades its dependence OpenAPI to DescribeAvailableClasses([#3973](https://github.com/aliyun/terraform-provider-alicloud/issues/3973))
- Upgrades the dependence sdk tea-rpc and tea-roa to fix the useless retry([#3971](https://github.com/aliyun/terraform-provider-alicloud/issues/3971))
- datasource/alicloud_db_instance_engines: Upgrades its dependence OpenAPI to DescribeAvailableZones([#3970](https://github.com/aliyun/terraform-provider-alicloud/issues/3970))
- datasource/alicloud_db_zones: Upgrades its dependence OpenAPI to DescribeAvailableZones([#3968](https://github.com/aliyun/terraform-provider-alicloud/issues/3968))
- testcase: Improves the bastionhost user attachment testcase([#3967](https://github.com/aliyun/terraform-provider-alicloud/issues/3967))

BUG FIXES:

- resource/alicloud_fc_trigger: Fixes fc trigger white space change error([#3980](https://github.com/aliyun/terraform-provider-alicloud/issues/3980))

## 1.134.0 (September 5, 2021)

- **New Resource:** `alicloud_dts_jobmonitor_rule`([#3965](https://github.com/aliyun/terraform-provider-alicloud/issues/3965))
- **New Resource:** `alicloud_bastionhost_user_attachment`([#3964](https://github.com/aliyun/terraform-provider-alicloud/issues/3964))
- **New Resource:** `alicloud_cdn_real_time_log_delivery`([#3963](https://github.com/aliyun/terraform-provider-alicloud/issues/3963))
- **New Resource:** `alicloud_direct_mail_mail_address`([#3961](https://github.com/aliyun/terraform-provider-alicloud/issues/3961))
- **New Resource:** `alicloud_bastionhost_host_group`([#3955](https://github.com/aliyun/terraform-provider-alicloud/issues/3955))
- **New Resource:** `alicloud_click_house_db_cluster`([#3948](https://github.com/aliyun/terraform-provider-alicloud/issues/3948))
- **New Resource:** `alicloud_vpc_dhcp_options_set`([#3944](https://github.com/aliyun/terraform-provider-alicloud/issues/3944))
- **New Resource:** `alicloud_express_connect_virtual_border_router`([#3943](https://github.com/aliyun/terraform-provider-alicloud/issues/3943))
- **New Resource:** `alicloud_clisck_house_account`([#3940](https://github.com/aliyun/terraform-provider-alicloud/issues/3940))
- **New Resource:** `alicloud_alb_health_check_template`([#3938](https://github.com/aliyun/terraform-provider-alicloud/issues/3938))
- **New Resource:** `alicloud_imm_project`([#3936](https://github.com/aliyun/terraform-provider-alicloud/issues/3936))
- **New Resource:** `alicloud_cms_metric_rule_template`([#3931](https://github.com/aliyun/terraform-provider-alicloud/issues/3931))
- **New Resource:** `alicloud_iot_device_group`([#3929](https://github.com/aliyun/terraform-provider-alicloud/issues/3929))
- **New Resource:** `alicloud_direct_mail_domain`([#3837](https://github.com/aliyun/terraform-provider-alicloud/issues/3837))
- **New Data Source:** `alicloud_cdn_real_time_log_deliveries`([#3963](https://github.com/aliyun/terraform-provider-alicloud/issues/3963))
- **New Data Source:** `alicloud_direct_mail_mail_addresses`([#3961](https://github.com/aliyun/terraform-provider-alicloud/issues/3961))
- **New Data Source:** `alicloud_bastionhost_host_groups`([#3955](https://github.com/aliyun/terraform-provider-alicloud/issues/3955))
- **New Data Source:** `alicloud_click_house_db_clusters`([#3948](https://github.com/aliyun/terraform-provider-alicloud/issues/3948))
- **New Data Source:** `alicloud_vpc_dhcp_options_sets`([#3944](https://github.com/aliyun/terraform-provider-alicloud/issues/3944))
- **New Data Source:** `alicloud_express_connect_virtual_border_routers`([#3943](https://github.com/aliyun/terraform-provider-alicloud/issues/3943))
- **New Data Source:** `alicloud_clisck_house_accounts`([#3940](https://github.com/aliyun/terraform-provider-alicloud/issues/3940))
- **New Data Source:** `alicloud_alb_health_check_templates`([#3938](https://github.com/aliyun/terraform-provider-alicloud/issues/3938))
- **New Data Source:** `alicloud_imm_project`([#3936](https://github.com/aliyun/terraform-provider-alicloud/issues/3936))
- **New Data Source:** `alicloud_cms_metric_rule_templates`([#3931](https://github.com/aliyun/terraform-provider-alicloud/issues/3931))
- **New Data Source:** `alicloud_iot_device_groups`([#3929](https://github.com/aliyun/terraform-provider-alicloud/issues/3929))
- **New Data Source:** `alicloud_direct_mail_domains`([#3837](https://github.com/aliyun/terraform-provider-alicloud/issues/3837))

ENHANCEMENTS:

- datasource/alicloud_db_instance_engines: Upgrades its dependence OpenAPI to DescribeAvailableZones([#3969](https://github.com/aliyun/terraform-provider-alicloud/issues/3969))
- resource/resource_alicloud_cs_kubernetes_permissions: update doc([#3962](https://github.com/aliyun/terraform-provider-alicloud/issues/3962))
- datasource/alicloud_db_zones: Upgrades its dependence OpenAPI to DescribeAvailableZones ([#3968](https://github.com/aliyun/terraform-provider-alicloud/issues/3968))
- testcase: Improves the bastionhost user attachment testcase([#3967](https://github.com/aliyun/terraform-provider-alicloud/issues/3967))
- testcase/alb: add sweeper test([#3966](https://github.com/aliyun/terraform-provider-alicloud/issues/3966))
- website: Fixed the sidebar([#3960](https://github.com/aliyun/terraform-provider-alicloud/issues/3960))
- testcase: Improves the provider test setting region id ([#3959](https://github.com/aliyun/terraform-provider-alicloud/issues/3959))
- resource/alicloud_mongodb_instance,alicloud_mongodb_sharding_instance: Adds new attribute order_type to support updating instance spec([#3958](https://github.com/aliyun/terraform-provider-alicloud/issues/3958))
- improves the client config source_ip and security_transport([#3956](https://github.com/aliyun/terraform-provider-alicloud/issues/3956))
- resource/alicloud_iot_device_group: Increase the length limit of the groupname attribute([#3954](https://github.com/aliyun/terraform-provider-alicloud/issues/3954))
- docs: Improves the resource vbr and its datasource docs([#3953](https://github.com/aliyun/terraform-provider-alicloud/issues/3953))
- resource/alicloud_cen_transit_router: Fixes the ParameterInstanceId error when deleting the resource; Improves other testcases([#3952](https://github.com/aliyun/terraform-provider-alicloud/issues/3952))
- testcase: Improves the alicloud_cen_atachment testcases; Improves the sweep testcases([#3951](https://github.com/aliyun/terraform-provider-alicloud/issues/3951))
- testcase: Improves the alicloud_cen_tranit_router_xxx testcases by adding vbr resource([#3946](https://github.com/aliyun/terraform-provider-alicloud/issues/3946))
- resource/alicloud_ram_user_policy_attachment,alicloud_ram_role_policy_attachment,alicloud_ram_group_policy_attachment: Fixes the resource not found error when creating an attachment using system policy([#3945](https://github.com/aliyun/terraform-provider-alicloud/issues/3945))
- doc/alicloud_alb_server_group: Optimize document links doc/alicloud_msc_sub_contact: Optimize document links doc/alicloud_msc_sub_contac testcase/alicloud_direct_mail_receivers: Optimize Test case testcase/alicloud_direct_mail_receiverses: Optimize Test case testcase/alicloud_alb_listener: Remove invalid logts: Optimize document links([#3941](https://github.com/aliyun/terraform-provider-alicloud/issues/3941))
- datasource/alicloud_db_instances: Upgrades its dependence sdk; datasource/alicloud_db_zones: Supports more attributes, like engine, engine_version([#3932](https://github.com/aliyun/terraform-provider-alicloud/issues/3932))

BUG FIXES:

- resource/alicloud_ram_user: Fixes the EntityNotExist.User error when getting user ([#3957](https://github.com/aliyun/terraform-provider-alicloud/issues/3957))
- resource/alicloud_alikafka_instance: Fixes the diff error caused by eip_max and security_group([#3937](https://github.com/aliyun/terraform-provider-alicloud/issues/3937))
- testcase:Fixed testcase's value for sae application([#3934](https://github.com/aliyun/terraform-provider-alicloud/issues/3934))
- datasource/alicloud_db_zones, alicloud_db_instance_classes, alicloud_db_instance_engines: Uses new api DescribeZones and DescribeInstanceClasses to improve them([#3930](https://github.com/aliyun/terraform-provider-alicloud/issues/3930))
- docs/alicloud_hbr_vault,alicloud_hbr_ecs_backup_client,alicloud_hbr_ecs_backup_plan,alicloud_nas_backup_plan,alicloud_oss_backup_plan,alicloud_snapshots,alicloud_restore_job: Corrects its docs and adds some note([#3928](https://github.com/aliyun/terraform-provider-alicloud/issues/3928))
- resource/alicloud_config_aggregate_compliance_pack: Change config_rule_parameters, parameter_name, parameter_value toOptional resource/alicloud_config_compliance_pack: Change config_rule_parameters, parameter_name, parameter_value to Optional([#3927](https://github.com/aliyun/terraform-provider-alicloud/issues/3927))
- doc/alicloud_alb_listeners: Optimize document links doc/alicloud_alb_load_balancers: Optimize document links testcase/alicloud_alb_rules: remove listener_id Field([#3926](https://github.com/aliyun/terraform-provider-alicloud/issues/3926))

## 1.133.0 (August 30, 2021)

- **New Resource:** `alicloud_ens_key_pair`([#3917](https://github.com/aliyun/terraform-provider-alicloud/issues/3917))
- **New Resource:** `alicloud_sae_application`([#3916](https://github.com/aliyun/terraform-provider-alicloud/issues/3916))
- **New Resource:** `alicloud_alb_rule`([#3915](https://github.com/aliyun/terraform-provider-alicloud/issues/3915))
- **New Resource:** `alicloud_security_center_group`([#3867](https://github.com/aliyun/terraform-provider-alicloud/issues/3867))
- **New Resource:** `alicloud_alb_acls`([#3853](https://github.com/aliyun/terraform-provider-alicloud/issues/3853))
- **New Resource:** `alicloud_bastionhost_user`([#3893](https://github.com/aliyun/terraform-provider-alicloud/issues/3893))
- **New Resource:** `alicloud_dfs_access_group`([#3885](https://github.com/aliyun/terraform-provider-alicloud/issues/3885))
- **New Resource:** `alicloud_ehpc_job_template`([#3871](https://github.com/aliyun/terraform-provider-alicloud/issues/3871))
- **New Resource:** `alicloud_sddp_config`([#3889](https://github.com/aliyun/terraform-provider-alicloud/issues/3889))
- **New Resource:** `alicloud_hbr_restore_job`([#3890](https://github.com/aliyun/terraform-provider-alicloud/issues/3890))
- **New Resource:** `alicloud_alb_listener`([#3908](https://github.com/aliyun/terraform-provider-alicloud/issues/3908))
- **New Data Source:** `alicloud_ens_key_pairs`([#3917](https://github.com/aliyun/terraform-provider-alicloud/issues/3917))
- **New Data Source:** `alicloud_sae_applications`([#3916](https://github.com/aliyun/terraform-provider-alicloud/issues/3916))
- **New Data Source:** `alicloud_alb_rules`([#3915](https://github.com/aliyun/terraform-provider-alicloud/issues/3915))
- **New Data Source:** `alicloud_security_center_groups`([#3867](https://github.com/aliyun/terraform-provider-alicloud/issues/3867))
- **New Data Source:** `alicloud_alb_acls`([#3853](https://github.com/aliyun/terraform-provider-alicloud/issues/3853))
- **New Data Source:** `alicloud_hbr_snapshots`([#3883](https://github.com/aliyun/terraform-provider-alicloud/issues/3883))
- **New Data Source:** `alicloud_bastionhost_users`([#3893](https://github.com/aliyun/terraform-provider-alicloud/issues/3893))
- **New Data Source:** `alicloud_dfs_access_groups`([#3885](https://github.com/aliyun/terraform-provider-alicloud/issues/3885))
- **New Data Source:** `alicloud_ehpc_job_templates`([#3871](https://github.com/aliyun/terraform-provider-alicloud/issues/3871))
- **New Data Source:** `alicloud_sddp_configs`([#3889](https://github.com/aliyun/terraform-provider-alicloud/issues/3889))
- **New Data Source:** `alicloud_hbr_restore_jobs`([#3890](https://github.com/aliyun/terraform-provider-alicloud/issues/3890))
- **New Data Source:** `alicloud_alb_listeners`([#3908](https://github.com/aliyun/terraform-provider-alicloud/issues/3908))

ENHANCEMENTS:

- resource/alicloud_slb_listener: Attribute scheduler support more values tch and qch([#3924](https://github.com/aliyun/terraform-provider-alicloud/issues/3924))
- resource/alicloud_slb_listener: Supports to setting scheduler in the creating to fix it cannot modify([#3923](https://github.com/aliyun/terraform-provider-alicloud/issues/3923))
- resource/alicloud_bastionhost_instance: Enlarges the create timeout and improves its docs([#3899](https://github.com/aliyun/terraform-provider-alicloud/issues/3899))
- resource/alicloud_alb_security_policy: add formatInt(response["TotalCount"]) == 0 selection([#3902](https://github.com/aliyun/terraform-provider-alicloud/issues/3902))
- resource/alicloud_log_store: Adds retry in sls delete logstore and fix resource logtail config nil bug([#3887](https://github.com/aliyun/terraform-provider-alicloud/issues/3887))
- resource/alicloud_event_bridge_service: Optimize the way to activate the service([#3902](https://github.com/aliyun/terraform-provider-alicloud/issues/3902))
- resource/alicloud_hbr_restore_job: update property options and fix hbr snapshot datasource testcase([#3914](https://github.com/aliyun/terraform-provider-alicloud/issues/3914))
- datasource/alicloud_hbr_snapshots: update timechecker([#3906](https://github.com/aliyun/terraform-provider-alicloud/issues/3906))
- testcase/alicloud_alb_server_group: Optimize the creation of test-dependent([#3902](https://github.com/aliyun/terraform-provider-alicloud/issues/3902))
- ECS instances testcase: Limit ALB supported regions testcase: Limit Event Bridge([#3902](https://github.com/aliyun/terraform-provider-alicloud/issues/3902))
- supported regions testcase: Limit DFS supported regions docs/alb_server_group: Optimization Basic Usage Example([#3902](https://github.com/aliyun/terraform-provider-alicloud/issues/3902))
- provider: Adds two new attribute source_ip and security_transport([#3900](https://github.com/aliyun/terraform-provider-alicloud/issues/3900))
- testcase: Improves the sweeper testcases([#3884](https://github.com/aliyun/terraform-provider-alicloud/issues/3884))
- testcase: Improves the testcase for fetching default vpc and vswitch([#3895](https://github.com/aliyun/terraform-provider-alicloud/issues/3895))
- testcase: Renames the testcase name by classifing them with product code([#3897](https://github.com/aliyun/terraform-provider-alicloud/issues/3897))
- testcase: Improves the testcase resource name([#3904](https://github.com/aliyun/terraform-provider-alicloud/issues/3904))

BUG FIXES:

- resource/alicloud_polardb_cluster: Fixes the resource not found error([#3896](https://github.com/aliyun/terraform-provider-alicloud/issues/3896))
- resource/alicloud_arms_contact: Fixes the ParameterMissing error when invoking UpdateAlertContact([#3898](https://github.com/aliyun/terraform-provider-alicloud/issues/3898))
- resource/alicloud_elasticsearch_instance: Fixes the GetCustomerLabelFail error by adding retry([#3901](https://github.com/aliyun/terraform-provider-alicloud/issues/3901))
- resource/alicloud_bastihost_instance: Fixes the InvalidApi error([#3903](https://github.com/aliyun/terraform-provider-alicloud/issues/3903))
- resource/alicloud_sddp_rule: Fixes the Sddp's Endpoint([#3907](https://github.com/aliyun/terraform-provider-alicloud/issues/3907))
- Fixes the concurrent write bug when describing the endpoints([#3894](https://github.com/aliyun/terraform-provider-alicloud/issues/3894))
- testcase: Fixes hbr snapshot doc and test case([#3905](https://github.com/aliyun/terraform-provider-alicloud/issues/3905))
- testcase: Fixed lang's import bug for sddp config([#3909](https://github.com/aliyun/terraform-provider-alicloud/issues/3909))

## 1.132.0 (August 21, 2021)

- **New Resource:** `alicloud_hbr_nas_backup_plan`([#3810](https://github.com/aliyun/terraform-provider-alicloud/issues/3810))
- **New Resource:** `alicloud_hbr_ecs_backup_plan`([#3810](https://github.com/aliyun/terraform-provider-alicloud/issues/3810))
- **New Resource:** `alicloud_cloud_storage_gateway_gateway`([#3843](https://github.com/aliyun/terraform-provider-alicloud/issues/3843))  
- **New Resource:** `alicloud_lindorm_instance`([#3861](https://github.com/aliyun/terraform-provider-alicloud/issues/3861))
- **New Resource:** `alicloud_cddc_dedicated_host_group`([#3869](https://github.com/aliyun/terraform-provider-alicloud/issues/3869))  
- **New Resource:** `alicloud_hbr_ecs_backup_client`([#3863](https://github.com/aliyun/terraform-provider-alicloud/issues/3863))
- **New Resource:** `alicloud_alb_load_balancer`([#3864](https://github.com/aliyun/terraform-provider-alicloud/issues/3864)) 
- **New Resource:** `alicloud_msc_sub_contact`([#3872](https://github.com/aliyun/terraform-provider-alicloud/issues/3872))
- **New Resource:** `alicloud_sddp_rule`([#3875](https://github.com/aliyun/terraform-provider-alicloud/issues/3875))
- **New Resource:** `alicloud_express_connect_physical_connection`([#3876](https://github.com/aliyun/terraform-provider-alicloud/issues/3876))
- **New Resource:** `alicloud_bastionhost_user_group`([#3879](https://github.com/aliyun/terraform-provider-alicloud/issues/3879))
- **New Data Source:** `alicloud_cloud_storage_gateway_gateways`([#3843](https://github.com/aliyun/terraform-provider-alicloud/issues/3843))  
- **New Data Source:** `alicloud_express_connect_access_points`([#3852](https://github.com/aliyun/terraform-provider-alicloud/issues/3852))
- **New Data Source:** `alicloud_hbr_ecs_backup_plans`([#3810](https://github.com/aliyun/terraform-provider-alicloud/issues/3810))
- **New Data Source:** `alicloud_lindorm_instances`([#3861](https://github.com/aliyun/terraform-provider-alicloud/issues/3861))
- **New Data Source:** `alicloud_alb_load_balancers`([#3864](https://github.com/aliyun/terraform-provider-alicloud/issues/3864))
- **New Data Source:** `alicloud_alb_zones`([#3864](https://github.com/aliyun/terraform-provider-alicloud/issues/3864))  
- **New Data Source:** `alicloud_express_connect_physical_connection_service`([#3865](https://github.com/aliyun/terraform-provider-alicloud/issues/3865))
- **New Data Source:** `alicloud_cddc_dedicated_host_groups`([#3869](https://github.com/aliyun/terraform-provider-alicloud/issues/3869))
- **New Data Source:** `alicloud_hbr_ecs_backup_clients`([#3863](https://github.com/aliyun/terraform-provider-alicloud/issues/3863))  
- **New Data Source:** `alicloud_msc_sub_contacts`([#3872](https://github.com/aliyun/terraform-provider-alicloud/issues/3872))
- **New Data Source:** `alicloud_express_connect_physical_connections`([#3876](https://github.com/aliyun/terraform-provider-alicloud/issues/3876))
- **New Data Source:**`alicloud_sddp_rules`([#3875](https://github.com/aliyun/terraform-provider-alicloud/issues/3875))
- **New Data Source:**`alicloud_bastionhost_user_groups`([#3879](https://github.com/aliyun/terraform-provider-alicloud/issues/3879))

ENHANCEMENTS:

- resource/alicloud_cr_ee_instance: Adds new attribute password to support reset instance login password([#3854](https://github.com/aliyun/terraform-provider-alicloud/issues/3854))
- resource/alicloud_cs_kubernetes_autoscaler: upgrade client-go version([#3839](https://github.com/aliyun/terraform-provider-alicloud/issues/3839))
- resource/alicloud_cr_ee_instance: Supports to set create timeout; testcase: Improves the alicloud_cr_ee_sync_rule testcases([#3856](https://github.com/aliyun/terraform-provider-alicloud/issues/3856))  
- resource/alicloud_cdn_domain_config: Removes the function_args forceNew and to support updating it in place([#3835](https://github.com/aliyun/terraform-provider-alicloud/issues/3835)) 
- resource/alicloud_event_bridge_slr: Adds role AliyunServiceRoleForEventBridgeSendToMNS for attribute product_name([#3859](https://github.com/aliyun/terraform-provider-alicloud/issues/3859))
- resource/alicloud_polardb_endpoint: Adds new attribute ssl_auto_rotate and ssl_certificate_url to set SSL certificate rotation([#3868](https://github.com/aliyun/terraform-provider-alicloud/issues/3868))  
- datasource/alicloud_event_bridge_service: Adds new attribute code to support international site([#3859](https://github.com/aliyun/terraform-provider-alicloud/issues/3859)) 
- resource/alicloud_yundun_bastionhost_instance: Fixes the setting security_group_ids failed error;Rename this resource to alicloud_bastionhost_instance([#3880](https://github.com/aliyun/terraform-provider-alicloud/issues/3880))
- data/alicloud_cr_ee_instances: Outputs more attributes authorization_token and temp_username([#3855](https://github.com/aliyun/terraform-provider-alicloud/issues/3855))
- datasource: Fixes the NotApplicable when using the alicloud_pvtz_serivce, alicloud_fnf_service, and alicloud_edas_service([#3877](https://github.com/aliyun/terraform-provider-alicloud/issues/3877))
- ci: Update go version to 0.13.4([#3857](https://github.com/aliyun/terraform-provider-alicloud/issues/3857))
- ci: Update go version to 0.13.4([#3858](https://github.com/aliyun/terraform-provider-alicloud/issues/3858))  
- testcase: Improves the running testcase strategy([#3848](https://github.com/aliyun/terraform-provider-alicloud/issues/3848))
- testcase: Improves the sweeper testcase([#3860](https://github.com/aliyun/terraform-provider-alicloud/issues/3860))  
- testcase: Improves the sweeper testcase([#3849](https://github.com/aliyun/terraform-provider-alicloud/issues/3849))
- docs/alicloud_cs_kubernetes_node_pool: Updates documentation and adds notes for node pool([#3870](https://github.com/aliyun/terraform-provider-alicloud/issues/3870))

BUG FIXES:

- resource/alicloud_actiontrail_trail: Fixes the error when updating trail config oss_write_role_arn([#3851](https://github.com/aliyun/terraform-provider-alicloud/issues/3851))
- resource/alicloud_cs_kubernetes_node_pool: fix update nodepool error([#3839](https://github.com/aliyun/terraform-provider-alicloud/issues/3839))
- Fixes the empty pointer error when setting a list attribute value([#3878](https://github.com/aliyun/terraform-provider-alicloud/issues/3878))

## 1.131.0 (August 16, 2021)

- **New Resource:** `alicloud_scdn_domain_config`([#3847](https://github.com/aliyun/terraform-provider-alicloud/issues/3847))
- **New Resource:** `alicloud_dcdn_domain_config`([#3846](https://github.com/aliyun/terraform-provider-alicloud/issues/3846))
- **New Resource:** `alicloud_arms_alert_contact_group`([#3845](https://github.com/aliyun/terraform-provider-alicloud/issues/3845))
- **New Resource:** `alb_server_group`([#3834](https://github.com/aliyun/terraform-provider-alicloud/issues/3834))
- **New Resource:** `alicloud_data_work_folder`([#3831](https://github.com/aliyun/terraform-provider-alicloud/issues/3831))
- **New Resource:** `alicloud_hbr_oss_backup_plan`([#3827](https://github.com/aliyun/terraform-provider-alicloud/issues/3827))
- **New Resource:** `alicloud_scdn_domain`([#3840](https://github.com/aliyun/terraform-provider-alicloud/issues/3840))
- **New Data Source:** `alicloud_arms_alert_contact_groups`([#3845](https://github.com/aliyun/terraform-provider-alicloud/issues/3845))
- **New Data Source:** `alb_server_groups`([#3834](https://github.com/aliyun/terraform-provider-alicloud/issues/3834))
- **New Data Source:** `alicloud_data_work_folders`([#3831](https://github.com/aliyun/terraform-provider-alicloud/issues/3831))
- **New Data Source:** `alicloud_hbr_oss_backup_plans`([#3827](https://github.com/aliyun/terraform-provider-alicloud/issues/3827))
- **New Data Source:** `alicloud_scdn_domains`([#3840](https://github.com/aliyun/terraform-provider-alicloud/issues/3840))

ENHANCEMENTS:

- Add Github WorkFlow(pull_request,tf_acctest)([#3836](https://github.com/aliyun/terraform-provider-alicloud/issues/3836))
- resource/alicloud_hbr_vault: Improves its update action([#3816](https://github.com/aliyun/terraform-provider-alicloud/issues/3816))
- resource/alicloud_instance: Adds new attribute instance_name([#3830](https://github.com/aliyun/terraform-provider-alicloud/issues/3830))
- testcase: Improves the sweep testcase for log_project([#3817](https://github.com/aliyun/terraform-provider-alicloud/issues/3817))
- docs/alicloud_eip_address: Corrects its docs and adds some note([#3823](https://github.com/aliyun/terraform-provider-alicloud/issues/3823))
- docs/alicloud_amqp_exchange: Adds the enum HEADERS for the exchange_type([#3832](https://github.com/aliyun/terraform-provider-alicloud/issues/3832))

BUG FIXES:

- resource/alicloud_event_bridge_rule: Fixes the targets parameters bug and update its testcase([#3842](https://github.com/aliyun/terraform-provider-alicloud/issues/3842))
- resource/alicloud_ess_attachment: Fixes the bug: call of reflect.Value.Set on zero Value([#3828](https://github.com/aliyun/terraform-provider-alicloud/issues/3828))
- data/alicloud_ess_scheduler_tasks: Fixes the converting type error([#3826](https://github.com/aliyun/terraform-provider-alicloud/issues/3826))

## 1.130.0 (August 07, 2021)

- **New Resource:** `alicloud_ecp_key_pair` ([#3815](https://github.com/aliyun/terraform-provider-alicloud/issues/3815))
- **New Resource:** `alicloud_kvstore_audit_log_config`([#3812](https://github.com/aliyun/terraform-provider-alicloud/issues/3812))
- **New Resource:** `alicloud_alb_security_policy`([#3809](https://github.com/aliyun/terraform-provider-alicloud/issues/3809))
- **New Resource:** `alicloud_ecd_policy_group`([#3808](https://github.com/aliyun/terraform-provider-alicloud/issues/3808))
- **New Resource:** `alicloud_event_bridge_event_source`([#3806](https://github.com/aliyun/terraform-provider-alicloud/issues/3806))
- **New Resource:** `alicloud_cloud_firewall_control_policy_order`([#3804](https://github.com/aliyun/terraform-provider-alicloud/issues/3804))
- **New Resource:** `alicloud_sae_config_map` ([#3801](https://github.com/aliyun/terraform-provider-alicloud/issues/3801))
- **New Resource:** `alicloud_alb_security_policy` ([#3809](https://github.com/aliyun/terraform-provider-alicloud/issues/3809))
- **New Data Source:** `alicloud_ecp_key_pairs`([#3815](https://github.com/aliyun/terraform-provider-alicloud/issues/3815))
- **New Data Source:** `alicloud_alb_security_policies`([#3809](https://github.com/aliyun/terraform-provider-alicloud/issues/3809))
- **New Data Source:** `alicloud_ecd_policy_groups`([#3808](https://github.com/aliyun/terraform-provider-alicloud/issues/3808))
- **New Data Source:** `alicloud_event_bridge_event_sources`([#3806](https://github.com/aliyun/terraform-provider-alicloud/issues/3806))
- **New Data Source:** `alicloud_sae_config_maps`([#3801](https://github.com/aliyun/terraform-provider-alicloud/issues/3801))

ENHANCEMENTS:

- testcase: Modify getting default vpc filter in the testcase([#3814](https://github.com/aliyun/terraform-provider-alicloud/issues/3814))
- resource/alicloud_alidns_record: Fixes the LastOperationNotFinished when creating several records one time([#3813](https://github.com/aliyun/terraform-provider-alicloud/issues/3813))
- resource/alicloud_polardb_cluster: Adds new attribute db_cluster_ip_array to modify security ips array name([#3798](https://github.com/aliyun/terraform-provider-alicloud/issues/3798))
- resource/resource_alicloud_cs_kubernetes_permissions: User authorization may be cleared when updating user permissions([#3807](https://github.com/aliyun/terraform-provider-alicloud/issues/3807))
- testcase/alicloud_sae_namespace: Improves its supported regions([#3793](https://github.com/aliyun/terraform-provider-alicloud/issues/3793)) 
- data/alicloud_nat_gateways: Removes the nat_type default value; improves the other testcases([#3762](https://github.com/aliyun/terraform-provider-alicloud/issues/3762))

BUG FIXES:

- resource/alicloud_event_bridge_event_bus: Fixes Count Exceed Limit Bug([#3806](https://github.com/aliyun/terraform-provider-alicloud/issues/3806))
- resource/alicloud_db_instance: Fixes bug result of attribute ha_config not set Computed:true.([#3797](https://github.com/aliyun/terraform-provider-alicloud/issues/3797))

## 1.129.0 (July 30, 2021)

- **New Resource:** `alicloud_hbr_vault`([#3770](https://github.com/aliyun/terraform-provider-alicloud/issues/3770))
- **New Resource:** `alicloud_event_bridge_event_bus`([#3783](https://github.com/aliyun/terraform-provider-alicloud/issues/3783))
- **New Resource:** `alicloud_ssl_certificates_service_certificate`([#3781](https://github.com/aliyun/terraform-provider-alicloud/issues/3781))
- **New Resource:** `alicloud_arms_alert_contact`([#3785](https://github.com/aliyun/terraform-provider-alicloud/issues/3785))
- **New Resource:** `alicloud_event_bridge_rule`([#3788](https://github.com/aliyun/terraform-provider-alicloud/issues/3788))
- **New Resource:** `alicloud_cloud_firewall_control_policy`([#3787](https://github.com/aliyun/terraform-provider-alicloud/issues/3787))  
- **New Resource:** `alicloud_event_bridge_slr`([#3775](https://github.com/aliyun/terraform-provider-alicloud/issues/3775))
- **New Resource:** `alicloud_sae_namespace`([#3786](https://github.com/aliyun/terraform-provider-alicloud/issues/3786))
- **New Data Source:** `alicloud_hbr_vaults`([#3770](https://github.com/aliyun/terraform-provider-alicloud/issues/3770))
- **New Data Source:** `alicloud_event_bridge_event_buses`([#3783](https://github.com/aliyun/terraform-provider-alicloud/issues/3783))
- **New Data Source:** `alicloud_ssl_certificates_service_certificates`([#3781](https://github.com/aliyun/terraform-provider-alicloud/issues/3781))
- **New Data Source:** `alicloud_ssl_certificates_service_certificatess`([#3785](https://github.com/aliyun/terraform-provider-alicloud/issues/3785))
- **New Data Source:** `alicloud_event_bridge_rules`([#3788](https://github.com/aliyun/terraform-provider-alicloud/issues/3788))
- **New Data Source:** `alicloud_cloud_firewall_control_policies`([#3787](https://github.com/aliyun/terraform-provider-alicloud/issues/3787))
- **New Data Source:** `alicloud_sae_namespaces`([#3786](https://github.com/aliyun/terraform-provider-alicloud/issues/3786))

ENHANCEMENTS:

- resource/alicloud_cs_kuberneters: Removes the useless diffFunc([#3772](https://github.com/aliyun/terraform-provider-alicloud/issues/3772))
- resource/alicloud_db_instance:Adds new attribute storage_auto_scale,storge_thireshold and storage_upper_bound to support storage auto-scaling([#3774](https://github.com/aliyun/terraform-provider-alicloud/issues/3774))
- resource/alicloud_amqp_instance: Supports to modify the attribute storage_size([#3778](https://github.com/aliyun/terraform-provider-alicloud/issues/3778))
- resource/alicloud_event_bridge_slr: Add resource not exist code.([#3790](https://github.com/aliyun/terraform-provider-alicloud/issues/3790))
- datasource/alicloud_amqp_queues: Improves the setting attribute 'attributes'([#3779](https://github.com/aliyun/terraform-provider-alicloud/issues/3779))

BUG FIXES:

- resource/alicloud_cs_kubernetes_permissions: Fixes grant permission error([#3782](https://github.com/aliyun/terraform-provider-alicloud/issues/3782))
- datasource/alicloud_log_service: Fixes endpoint connection timeout bug in log service([#3768](https://github.com/aliyun/terraform-provider-alicloud/issues/3768))
- resource/alicloud_ddoscoo_instance: Fixes the NotApplicable error when creating the instance([#3789](https://github.com/aliyun/terraform-provider-alicloud/issues/3789))

## 1.128.0 (July 24, 2021)

- **New Resource:** `alicloud_amqp_instance`([#3764](https://github.com/aliyun/terraform-provider-alicloud/issues/3764))
- **New Resource:** `alicloud_amqp_exchange`([#3737](https://github.com/aliyun/terraform-provider-alicloud/issues/3737))
- **New Resource:** `alicloud_cassandra_backup_plan`([#3733](https://github.com/aliyun/terraform-provider-alicloud/issues/3733))
- **New Resource:** `alicloud_cen_transit_router_peer_attachment`([#3753](https://github.com/aliyun/terraform-provider-alicloud/issues/3753))
- **New Data Source:** `alicloud_amqp_instances`([#3764](https://github.com/aliyun/terraform-provider-alicloud/issues/3764))
- **New Data Source:** `alicloud_amqp_exchanges`([#3737](https://github.com/aliyun/terraform-provider-alicloud/issues/3737))
- **New Data Source:** `alicloud_cassandra_backup_plans`([#3733](https://github.com/aliyun/terraform-provider-alicloud/issues/3733))
- **New Data Source:** `alicloud_cen_transit_router_peer_attachments`([#3753](https://github.com/aliyun/terraform-provider-alicloud/issues/3753))
- **New Data Source:** `alicloud_kvstore_permission`([#3759](https://github.com/aliyun/terraform-provider-alicloud/issues/3759))

ENHANCEMENTS:

- resource/alicloud_db_readonly_instance：Adds new attributes such as upgrade_kernel_version_enabled, upgrade_time, switch_time and target_minor_version to support Update minor engine version.([#3729](https://github.com/aliyun/terraform-provider-alicloud/issues/3729))
- resource/alicloud_serverless_kubernetes: Removes the deprecated attribute private_zone default value to fix an issue where the ASK cluster service discovery was not working([#3738](https://github.com/aliyun/terraform-provider-alicloud/issues/3738))
- resource/alicloud_disk: delete and recreate disk if snapshot_id changed([#3361](https://github.com/aliyun/terraform-provider-alicloud/issues/3361))
- resource/alicloud_cen_instance: Upgrades its dependence sdk([#3742](https://github.com/aliyun/terraform-provider-alicloud/issues/3742))
- resource/alicloud_route_table: Removes the specified expectedError into Retry Process with Delete Method([#3746](https://github.com/aliyun/terraform-provider-alicloud/issues/3746))
- resource/alicloud_db_instance: Adds engine limitation before invoking ModifySQLCollectorRetention([#3754](https://github.com/aliyun/terraform-provider-alicloud/issues/3754))
- resource/alicloud_db_instance: Adds attributes ha_config and manual_ha_time to support ModifyHASwitchConfig(enable or disable automatic primary/secondary switchover).([#3755](https://github.com/aliyun/terraform-provider-alicloud/issues/3755))
- resource/alicloud_kvstore_instance: Adds parameter dry_run([#3761](https://github.com/aliyun/terraform-provider-alicloud/issues/3761))
- resource/alicloud_db_instance: Checks db_instance's status before updating sql_collector_status attribute([#3760](https://github.com/aliyun/terraform-provider-alicloud/issues/3760)) 
- resource/alicloud_kvstore_instance: Adds new attribute secondary_zone_id to support secondary zone([#3757](https://github.com/aliyun/terraform-provider-alicloud/issues/3757))
- resource/alicloud_polardb_cluster: Adds new attribute security_group_ids to support setting security group([#3752](https://github.com/aliyun/terraform-provider-alicloud/issues/3752))  
- provider: Sets old sdk config EnableAsync to false; Close the location client after it invoked([#3756](https://github.com/aliyun/terraform-provider-alicloud/issues/3756))
- vendor: Improves the vendor dependence github.com/sirupsen/logrus([#3747](https://github.com/aliyun/terraform-provider-alicloud/issues/3747))
- testcase: Improves the amqp resources testcase([#3765](https://github.com/aliyun/terraform-provider-alicloud/issues/3765))



BUG FIXES:

- resource/alicloud_fc_service: Fixes the bug when there is no need to retry([#3741](https://github.com/aliyun/terraform-provider-alicloud/issues/3741))
- doc/alicloud_gpdb_elastic_instance: Fixes some Example Usage Parameter([#3749](https://github.com/aliyun/terraform-provider-alicloud/issues/3749))


## 1.127.0 (July 16, 2021)

- **New Resource:** `alicloud_cs_autoscaling_config`([#3734](https://github.com/aliyun/terraform-provider-alicloud/issues/3734))
- **New Resource:** `alicloud_gpdb_elastic_instance`([#3727](https://github.com/aliyun/terraform-provider-alicloud/issues/3727))
- **New Resource:** `alicloud_amqp_queue`([#3720](https://github.com/aliyun/terraform-provider-alicloud/issues/3720))
- **New Data Source:** `alicloud_amqp_queues`([#3720](https://github.com/aliyun/terraform-provider-alicloud/issues/3720))

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool: Adds new attributes platform, scaling_policy, instances, keep_instance_name and format_disk([#3734](https://github.com/aliyun/terraform-provider-alicloud/issues/3734))
- client/bssopenapiClient: Improves the bss openapi endpoint to avoid the NotApplicable error; Fixes the alidns_instance setting domain_numbers failed issue([#3713](https://github.com/aliyun/terraform-provider-alicloud/issues/3713))
- resource/alicloud_datahub_project: Upgrades it dependence sdk([#3723](https://github.com/aliyun/terraform-provider-alicloud/issues/3723))
- resource/alicloud_datahub_project: Improves its dependece([#3725](https://github.com/aliyun/terraform-provider-alicloud/issues/3725))
- Reset the resource event_bus and schema_group and its datasource([#3721](https://github.com/aliyun/terraform-provider-alicloud/issues/3721))
- provider: Sets the max idle conns to 500 in the client; Adds docs unit statement for the provider attribute client_read_timeout and client_connect_timeout([#3728](https://github.com/aliyun/terraform-provider-alicloud/issues/3728))
- ci: Upgrades the ci go version to 1.15.10([#3732](https://github.com/aliyun/terraform-provider-alicloud/issues/3732))
- docs: Improves the docs parsing subcategory faild error([#3722](https://github.com/aliyun/terraform-provider-alicloud/issues/3722))
- docs/alicloud_db_instance: Improves its docs by adding a blank line to fix it error formate([#3730](https://github.com/aliyun/terraform-provider-alicloud/issues/3730))

BUG FIXES:

- resource/alicloud_slb_listener: Fixes the default parameter when updating the specified parameter with SetLoadBalancerHTTPSListenerAttribute Method([#3735](https://github.com/aliyun/terraform-provider-alicloud/issues/3735))
- resource/alicloud_db_readonly_instance and alicloud_db_instance: Fixes the diff error caused by ca_type, acl, and replication_acl([#3731](https://github.com/aliyun/terraform-provider-alicloud/issues/3731))
- testcase: Fixed cen ci test.([#3719](https://github.com/aliyun/terraform-provider-alicloud/issues/3719))

## 1.126.0 (July 12, 2021)

- **New Resource:** `alicloud_amqp_virtual_host`([#3714](https://github.com/aliyun/terraform-provider-alicloud/issues/3714))
- **New Resource:** `alicloud_eip_address`([#3682](https://github.com/aliyun/terraform-provider-alicloud/issues/3682))
- **New Resource:** `alicloud_cen_transit_router`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_route_table`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_route_table_association`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_route_table_propagation`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_route_entry`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_vbr_attachment`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Resource:** `alicloud_cen_transit_router_vpc_attachment`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_amqp_virtual_hosts`([#3714](https://github.com/aliyun/terraform-provider-alicloud/issues/3714))
- **New Data Source:** `alicloud_cen_transit_routers`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_route_tables`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_route_table_associations`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_route_table_propagations`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_route_entries`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_vbr_attachments`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_cen_transit_router_vpc_attachments`([#3706](https://github.com/aliyun/terraform-provider-alicloud/issues/3706))
- **New Data Source:** `alicloud_log_projects`([#3691](https://github.com/aliyun/terraform-provider-alicloud/issues/3691))
- **New Data Source:** `alicloud_log_stores`([#3691](https://github.com/aliyun/terraform-provider-alicloud/issues/3691))
- **New Data Source:** `alicloud_event_bridge_service`([#3691](https://github.com/aliyun/terraform-provider-alicloud/issues/3691))
- **New Data Source:** `alicloud_eip_addresses`([#3682](https://github.com/aliyun/terraform-provider-alicloud/issues/3682))

ENHANCEMENTS:

- resource/alicloud_mongodb_sharding_instance: The attribute shard_list supports to set readonly_replicas; Supports setting self-timeout([#3718](https://github.com/aliyun/terraform-provider-alicloud/issues/3718))
- resource/alicloud_db_instance：Adds new attributes such as upgrade_kernel_version_enabled, upgrade_time, switch_time and target_minor_version to support Update minor engine version.([#3692](https://github.com/aliyun/terraform-provider-alicloud/issues/3692))
- resource/alicloud_polardb_cluster: Enlarges the timeout after modifying the tde_status([#3699](https://github.com/aliyun/terraform-provider-alicloud/issues/3699))
- resource/alicloud_db_instance: Adds new attributes connection_string_prefix and port to support Modify db instance connection_string_prefix or port.([#3703](https://github.com/aliyun/terraform-provider-alicloud/issues/3703))
- resource/alicloud_db_account: Modify attribute account_name limited length to 2-63 for PostgreSQL.([#3707](https://github.com/aliyun/terraform-provider-alicloud/issues/3707))
- resource/alicloud_db_backup_policy: Adds instance status judgement, and call API ModifyBackupPolicy if the status is Running.([#3708](https://github.com/aliyun/terraform-provider-alicloud/issues/3708))
- resource/alicloud_gpdb_instance: Fixes the InvalidPayType error([#3709](https://github.com/aliyun/terraform-provider-alicloud/issues/3709))
- testcase: Improves the direct mail receivers testcase([#3687](https://github.com/aliyun/terraform-provider-alicloud/issues/3687))
- testcase: Improves the sweeper test to avoid unsupported region([#3688](https://github.com/aliyun/terraform-provider-alicloud/issues/3688))
- testcase: Limit test region with event bridge service.([#3697](https://github.com/aliyun/terraform-provider-alicloud/issues/3697))
- docs/alicloud_actiontrail_trail: Adds 'is_organization_trail' attribute description in the docs([#3695](https://github.com/aliyun/terraform-provider-alicloud/issues/3695))
- docs: Adds note for alicloud_polardb_cluster docs for ‘encrypt_new_tables’([#3702](https://github.com/aliyun/terraform-provider-alicloud/issues/3702))
- client/bssopenapiClient: Improves the bss openapi endpoint to avoid the NotApplicable error; Fixes the alidns_instance setting domain_numbers failed issue([#3713](https://github.com/aliyun/terraform-provider-alicloud/issues/3713))

BUG FIXES:

- resource/alicloud_mongodb_instance: Fixes the setting replication_factor failed error([#3717](https://github.com/aliyun/terraform-provider-alicloud/issues/3717))
- resource/alicloud_mongodb_instance: Fixes the ProxyError issue when invoking the DescribeMongoDBTDEInfo API([#3716](https://github.com/aliyun/terraform-provider-alicloud/issues/3716))
- testcase: Fixed the 'isp' filter bug for Eip Address.([#3710](https://github.com/aliyun/terraform-provider-alicloud/issues/3710))

## 1.125.0 (July 03, 2021)

- **New Resource:** `alicloud_direct_mail_receivers`([#3684](https://github.com/aliyun/terraform-provider-alicloud/issues/3684))
- **New Data Source:** `alicloud_direct_mail_receiverses`([#3684](https://github.com/aliyun/terraform-provider-alicloud/issues/3684))

ENHANCEMENTS:

- resource/alicloud_log_audit: Adds a limitation that there does not allow the variable_map setting the key with suffix _policy_setting([#3685](https://github.com/aliyun/terraform-provider-alicloud/issues/3685))
- resource/alicloud_db_instance: Adds more attribute to support security_ips, including db_instance_ip_array_name, db_instance_ip_array_attribute , security_ip_type, whitelist_network_type, modify_mode([#3662](https://github.com/aliyun/terraform-provider-alicloud/issues/3662))
- resource/alicloud_db_instance: Adds new attribute private_ip_address and supports to change VPC or vSwitch([#3676](https://github.com/aliyun/terraform-provider-alicloud/issues/3676))
- resource/alicloud_ddoscoo_instance: Adds product_type to differ international and domestic accounts when managing instances([#3679](https://github.com/aliyun/terraform-provider-alicloud/issues/3679))
- provider: Adds new attribute client_read_timeout and client_connect_timeout to support setting self-define timeout([#3677](https://github.com/aliyun/terraform-provider-alicloud/issues/3677))
- resource/alicloud_elasticsearch_instance: Adds new attribute setting_config([#3675](https://github.com/aliyun/terraform-provider-alicloud/issues/3675))
- datasource/alicloud_resource_manager_accounts: Exports new attributes 'account_name'.([#3681](https://github.com/aliyun/terraform-provider-alicloud/issues/3681))
- testcase: Improves the direct mail receivers testcase([#3687](https://github.com/aliyun/terraform-provider-alicloud/issues/3687))

BUG FIXES:

- resource/alicloud_log_audit: Fixes sls audit bug when setting the attribute multi_account([#3678](https://github.com/aliyun/terraform-provider-alicloud/issues/3678))
- resource/alicloud_cr_ee_instance: Fixes the error NotApplicable when creating and reading the resource([#3680](https://github.com/aliyun/terraform-provider-alicloud/issues/3680))
- resoure/alicloud_hbase_instance: Fixes the error "rpc error: code = Internal desc = grpc: error while marshaling: string field contains invalid UTF-8" when getting hbase instance([#3683](https://github.com/aliyun/terraform-provider-alicloud/issues/3683))

## 1.124.4 (June 25, 2021)

ENHANCEMENTS:

- docs: Modify the docs attribute available version([#3670](https://github.com/aliyun/terraform-provider-alicloud/issues/3670))
- resource/alicloud_kms_alias: Upgrades its dependence SDK([#3647](https://github.com/aliyun/terraform-provider-alicloud/issues/3647))
- resource/alicloud_kms_key_version: Upgrades its dependence SDK; Removes the computed attribute creation_date([#3648](https://github.com/aliyun/terraform-provider-alicloud/issues/3648))
- resource/alicloud_kms_ciphertext: Upgrades its dependence sdk; Improves the kms key testcases([#3649](https://github.com/aliyun/terraform-provider-alicloud/issues/3649))
- datasource/alicloud_kms_plaintext: Upgrades its dependence sdk([#3650](https://github.com/aliyun/terraform-provider-alicloud/issues/3650))
- datasource/alicloud_kms_secret_versions: Upgredes its dependence sdk([#3653](https://github.com/aliyun/terraform-provider-alicloud/issues/3653))
- resource/alicloud_kms_ciphertext: Upgrades its dependence sdk([#3655](https://github.com/aliyun/terraform-provider-alicloud/issues/3655))
- service_kms/Decrypt: Upgrades its dependence sdk; kms_service/SetResourceTags: Upgrades its dependence sdk; Removes the KMS go sdk([#3656](https://github.com/aliyun/terraform-provider-alicloud/issues/3656))
- resource/alicloud_db_instance: Adds several attributes to enable ssl, like ssl_enabled, ca_type , server_cert, client_ca_cert and so on([#3615](https://github.com/aliyun/terraform-provider-alicloud/issues/3615))
- resource/alicloud_eip: Adds new attribute deletion_protection to support deletion protection feature([#3664](https://github.com/aliyun/terraform-provider-alicloud/issues/3664))
- resource/alicloud_nat_gateway: Adds new attribute deletion_protection to support deletion protection feature([#3665](https://github.com/aliyun/terraform-provider-alicloud/issues/3665))
- resource/alicloud_common_bandwidth_package: Adds new attribute deletion_protection to support deletion protection feature([#3666](https://github.com/aliyun/terraform-provider-alicloud/issues/3666))

BUG FIXES:

- testcase: Fixes the incorrect data type([#3669](https://github.com/aliyun/terraform-provider-alicloud/issues/3669))
- resource/alicloud_snat_entry: Fixes the concurrence issue which throwing the error OperationFailed.Throttling([#3657](https://github.com/aliyun/terraform-provider-alicloud/issues/3657))
- resource/alicloud_cr_ee_instance: Fixes the NotApplicable error for international site account([#3651](https://github.com/aliyun/terraform-provider-alicloud/issues/3651))
- resource/alicloud_emr_cluster: Fix emr cluster task scale up([#3658](https://github.com/aliyun/terraform-provider-alicloud/issues/3658))
- docs: Corrects the spelling error([#3659](https://github.com/aliyun/terraform-provider-alicloud/issues/3659))

## 1.124.3 (June 18, 2021)

ENHANCEMENTS:

- resource/alicloud_log_audit: Returns the multi accounts while setting it into state([#3637](https://github.com/aliyun/terraform-provider-alicloud/issues/3637))
- resource/alicloud_ess_scalingconfiguration: Adds new attributes performance_level and system_disk_performance_level to support performance level([#3632](https://github.com/aliyun/terraform-provider-alicloud/issues/3632))
- resource/alicloud_polardb_cluster: Adds new attribute encrypt_new_tables([#3630](https://github.com/aliyun/terraform-provider-alicloud/issues/3630))
- datasource/alicloiud_db_instances: Outputs more attributes, like creator, delete_date, description, encryption_key, encryption_key_status and so on([#3623](https://github.com/aliyun/terraform-provider-alicloud/issues/3623))

BUG FIXES:

- resource/alicloud_mse_cluster: Corrects the attribute cluster_specification valid values([#3644](https://github.com/aliyun/terraform-provider-alicloud/issues/3644))
- resource/alicloud_resource_manager_account: Fixes import resoruce failed cause by 'payer_account_id'([#3643](https://github.com/aliyun/terraform-provider-alicloud/issues/3643))
- resource/alicloud_snat_entry: Fixes the UnknownError when creating a new snat entry by adding Idempotent and retry strategy([#3639](https://github.com/aliyun/terraform-provider-alicloud/issues/3639))
- resource/alicloud_db_instance: Fixes the OperationDenied.DBInstanceStatus error after modifying parameters; Improves some testcases([#3638](https://github.com/aliyun/terraform-provider-alicloud/issues/3638))
- resource/alicloud_db_readonly_instance: Fixes the OperationDenied.PrimaryDBInstanceStatus by adding retry when it happened([#3635](https://github.com/aliyun/terraform-provider-alicloud/issues/3635))
- resource/alicloud_oos_template: Fixes the tags diff bug caused by without ingore system tags([#3634](https://github.com/aliyun/terraform-provider-alicloud/issues/3634))
- docs: Corrects the mse_cluster docs error([#3636](https://github.com/aliyun/terraform-provider-alicloud/issues/3636))

## 1.124.2 (June 12, 2021)

ENHANCEMENTS:

- docs: add note for alicloud_kvstore_instance ssl_enable and correct the alicloud_mse_cluster net_type valid values([#3619](https://github.com/aliyun/terraform-provider-alicloud/issues/3619))

BUG FIXES:

- resource/alicloud_network_acl: Fixes the entries sort error because of the sort means priority([#3627](https://github.com/aliyun/terraform-provider-alicloud/issues/3627))
- resource/alicloud_kms_secret: Fixes the Forbidden.ResourceNotFound error when deleting([#3626](https://github.com/aliyun/terraform-provider-alicloud/issues/3626))
- resource/alicloud_ecs_disk: Fixes the creating disk error cause by ModifyDiskChargeType; Fixes the diff bug when category is cloud_essd([#3625](https://github.com/aliyun/terraform-provider-alicloud/issues/3625))
- resource/alicloud_elasitcsearch_instance: Fixes the enable_kibana_private_network is not effect error when the first creation.([#3622](https://github.com/aliyun/terraform-provider-alicloud/issues/3622))
- resource/alicloud_network_acl: Fixes deleting the acl failed cause by there exists bound resources.([#3620](https://github.com/aliyun/terraform-provider-alicloud/issues/3620))
- resource/alicloud_instance: Fixes setting tags failed bug when the tag count is more than 10([#3618](https://github.com/aliyun/terraform-provider-alicloud/issues/3618))

## 1.124.1 (June 5, 2021)

ENHANCEMENTS:

- ci: Adds ci test for OOS and Eci resources and data sources([#3611](https://github.com/aliyun/terraform-provider-alicloud/issues/3611))
- resource/alicloud_pvtz_zone_record: Fixes the 'record_id' diff error caused by using the incorrect type([#3610](https://github.com/aliyun/terraform-provider-alicloud/issues/3610))
- docs: Improve the docs([#3609](https://github.com/aliyun/terraform-provider-alicloud/issues/3609))
- resource/alicloud_slb_server_group: Adds Computed for the attribute servers to meet scenario when using resource alicloud_ess_scalinggroup_vserver_groups([#3607](https://github.com/aliyun/terraform-provider-alicloud/issues/3607)) 
- resource/alicloud_kms_key: Adds limitation for pending_window_in_days when deprecating the deletion_window_in_days([#3594](https://github.com/aliyun/terraform-provider-alicloud/issues/3594)) 
- resource/alicloud_config_aggregate_config_rule: Adds DiffSuppressFunc for 'maximum_execution_frequency'([#3592](https://github.com/aliyun/terraform-provider-alicloud/issues/3592)) 
- resource/alicloud_cms_alarm: Adds statistics more valid values: Value, Sum, Count([#3274](https://github.com/aliyun/terraform-provider-alicloud/issues/3274))
- resource/alicloud_db_instance: Adds ssl related attributes, like ca_type, server_cert, server_key, client_ca_cert, client_crl_enabled, client_cert_revocation_list, acl, replication_acl([#3573](https://github.com/aliyun/terraform-provider-alicloud/issues/3573))

BUG FIXES:

- resource/alicloud_network_acl: Fixes attributes diff caused by 'resources'([#3597](https://github.com/aliyun/terraform-provider-alicloud/issues/3597)) 
- resource/alicloud_api_gateway_api: Fixes the bug (issues #2276) when setting the attribute constant_parameters([#3605](https://github.com/aliyun/terraform-provider-alicloud/issues/3605)) 
- resource/alicloud_network_acl: Fixes destroy resource failed caused by 'resources'([#3601](https://github.com/aliyun/terraform-provider-alicloud/issues/3601)) 
- resource/alicloud_log_audit：Fixes log audit bug when setting multi_account; Adds missing domain when invoking the request([#3595](https://github.com/aliyun/terraform-provider-alicloud/issues/3595))
- resource/alicloud_slb_load_balancer: Fixes create the payasyougo instance failed caused by 'instance_charge_type'([#3598](https://github.com/aliyun/terraform-provider-alicloud/issues/3598))
- resource/alicloud_alidns_instance: Sets renew_period renew_status to state; Fixes force replacement bug because there is no API can return; Upgrades its dependence SDK([#3599](https://github.com/aliyun/terraform-provider-alicloud/issues/3599))
- resource/alicloud_kvstore_instance: Converts auto_renew attribute to bool before saving([#3065](https://github.com/aliyun/terraform-provider-alicloud/issues/3065))

## 1.124.0 (May 29, 2021)

- **New Resource:** `alicloud_config_aggregate_config_rule`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Resource:** `alicloud_config_aggregate_compliance_pack`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Resource:** `alicloud_config_compliance_pack`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Resource:** `alicloud_config_aggregator`([#3567](https://github.com/aliyun/terraform-provider-alicloud/issues/3567)) 
- **New Resource:** `alicloud_cr_ee_instance`([#3560](https://github.com/aliyun/terraform-provider-alicloud/issues/3560)) 
- **New Data Source:** `alicloud_config_aggregate_config_rules`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Data Source:** `alicloud_config_aggregate_compliance_packs`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Data Source:** `alicloud_config_compliance_packs`([#3561](https://github.com/aliyun/terraform-provider-alicloud/issues/3561)) 
- **New Data Source:** `alicloud_config_aggregators`([#3567](https://github.com/aliyun/terraform-provider-alicloud/issues/3567)) 

ENHANCEMENTS:

- resource/alicloud_kms_key: Adds limitation for pending_window_in_days when deprecating the deletion_window_in_days([#3594](https://github.com/aliyun/terraform-provider-alicloud/issues/3594))
- resource/alicloud_config_aggregate_config_rule: Adds DiffSuppressFunc for 'maximum_execution_frequency' for 'maximum_execution_frequency' (([#3592](https://github.com/aliyun/terraform-provider-alicloud/issues/3592)))  
- resource/aliclous_kvstore_instance: support change private connection port([#3587](https://github.com/aliyun/terraform-provider-alicloud/issues/3587))
- resource/alicloud_polardb_cluster: supports transform pay_type; add modify db_node_class and renewal_status asynchronous waiting; add PrePaid cluster can not be release.([#3586](https://github.com/aliyun/terraform-provider-alicloud/issues/3586))
- resource/alicloud_fc_function: Enlarges the attribute memory_size max value to 32768([#3589](https://github.com/aliyun/terraform-provider-alicloud/issues/3589))
- resource/alicloud_elasticsearch_instance: Upgrades its dependence sdk([#3568](https://github.com/aliyun/terraform-provider-alicloud/issues/3568))
- resource/alicloud_network_acl: Support attributes 'resources' for network ACL.([#3575](https://github.com/aliyun/terraform-provider-alicloud/issues/3575)) 
- resource/alicloud_network_acl_attachment: Deprecated from version 1.124.0.([#3575](https://github.com/aliyun/terraform-provider-alicloud/issues/3575)) 
- resource/alicloud_kms_secret: Adds new attributes enable_automatic_rotation and rotation_interval; Upgrades its dependence sdk([#3574](https://github.com/aliyun/terraform-provider-alicloud/issues/3574))
- resource/alicloud_log_store: Adds new attribute encrypt_conf to support encrypt logstore([#3576](https://github.com/aliyun/terraform-provider-alicloud/issues/3576))
- datasource/alicloud_ots_service: Adds support for auto-retry when happened the timeout; docs: Update the next version to 1.123.1([#3569](https://github.com/aliyun/terraform-provider-alicloud/issues/3569))
- docs: Updates alicloud_fc_function max memory_size to 32768([#3590](https://github.com/aliyun/terraform-provider-alicloud/issues/3590)) 
- docs: Update ACK resources and datasources subcategory([#3577](https://github.com/aliyun/terraform-provider-alicloud/issues/3577))
- testcase: Add param pending_window_in_days to fix alicloud_kms_secret test error.([#3585](https://github.com/aliyun/terraform-provider-alicloud/issues/3585))
- testcase: Improves the elasitcsearch instance testcase([#3572](https://github.com/aliyun/terraform-provider-alicloud/issues/3572))
- ci: Removes the usless jobs and change job task go verion to 12 to avoid download dependence always([#3571](https://github.com/aliyun/terraform-provider-alicloud/issues/3571))

BUG FIXES:

- resource/alicloud_vpc: Fixes force replacement bug caused by 'enable_ipv6'([#3581](https://github.com/aliyun/terraform-provider-alicloud/issues/3581)) 
- resource/alicloud_mongodb_instance: Fixes the parsing replication_factor error when it is empty([#3570](https://github.com/aliyun/terraform-provider-alicloud/issues/3570))
- testcase: Fixes the sweeper test error caused by new resource ecs_network_interface([#3578](https://github.com/aliyun/terraform-provider-alicloud/issues/3578))
- testcase: Fixes the ecs_network_interface sweeper testcase bug([#3583](https://github.com/aliyun/terraform-provider-alicloud/issues/3583))

## 1.123.1 (May 22, 2021)

ENHANCEMENTS:

- resource/alicloud_mongodb_instance: Fixes the parsing replication_factor error when it is empty([#3570](https://github.com/aliyun/terraform-provider-alicloud/issues/3570))
- resource/alicloud_cs_kubernetes_nood_pool: Adds supports to create spot instance, set public IP and resource_group_id; resource/alicloud_cs_serverless_kubernetes: Support to set coredns as service discovery, time zone and sls log config; resource/alicloud_cs_managed_kubernetes: Fixes the bug that upgrades the cluster after creating it.([#3558](https://github.com/aliyun/terraform-provider-alicloud/issues/3558))
- resource/alicloud_ecs_dedicated_host: Adds new attributes cpu_over_commit_ratio, dedicated_host_cluster_id and min_quantity; Its datasource adds new attributes operation_locks; Updates its dependence SDK([#3548](https://github.com/aliyun/terraform-provider-alicloud/issues/3548))
- resource/alicloud_kms_key: Deprecates the key_state and use status instead; Its datasource supports filters and more output attributes; Upgrades its dependence sdk([#3555](https://github.com/aliyun/terraform-provider-alicloud/issues/3555))
- docs: Updates the ACK code in the docs([#3547](https://github.com/aliyun/terraform-provider-alicloud/issues/3547))
- docs: Rename Server Load Balancer(SLB) to Classic Load Balancer(CLB)([#3556](https://github.com/aliyun/terraform-provider-alicloud/issues/3556))
- ci: Adds the color output when running the test([#3544](https://github.com/aliyun/terraform-provider-alicloud/issues/3544))

BUG FIXES:

- datasource/alicloud_ram_groups: Fixes the crash bug that parsing failed; datasource/alicloud_ram_roles: Fixes the fetching failed when the role is too many; resource/alicloud_ram_login_profile: Fixes the deleting error EntityNotExist.User([#3543](https://github.com/aliyun/terraform-provider-alicloud/issues/3543))
- datasource/alicloud_ecs_disks: Add judgment to assertion([#3553](https://github.com/aliyun/terraform-provider-alicloud/issues/3553))
- testcase: remove import check from alicloud_ecs_network_interface multi testcase and sweep skip resource not has name([#3545](https://github.com/aliyun/terraform-provider-alicloud/issues/3545))
- testcase: skip unsupport region for alicloud_kms_key([#3564](https://github.com/aliyun/terraform-provider-alicloud/issues/3564))
- testcase: Fix deprecated field for slb listener testcase([#3562](https://github.com/aliyun/terraform-provider-alicloud/issues/3562))

## 1.123.0 (May 14, 2021)

- **New Resource:** `alicloud_ddoscoo_domain_resource`([#3530](https://github.com/aliyun/terraform-provider-alicloud/issues/3530))
- **New Resource:** `alicloud_ddoscoo_port`([#3530](https://github.com/aliyun/terraform-provider-alicloud/issues/3530))
- **New Data Source:** `alicloud_ddoscoo_domain_resources`([#3530](https://github.com/aliyun/terraform-provider-alicloud/issues/3530))
- **New Data Source:** `alicloud_ddoscoo_ports`([#3530](https://github.com/aliyun/terraform-provider-alicloud/issues/3530))

ENHANCEMENTS:

- resource/alicloud_vpc: Improves the vpc attribute limitation by adding ConflictWith for enable_ipv6 and cidr_block([#3535](https://github.com/aliyun/terraform-provider-alicloud/issues/3535))
- resource/alicloud_mongodb_instance: Reset replicationFactor to replication_factor when setting iinto state([#3537](https://github.com/aliyun/terraform-provider-alicloud/issues/3537))
- resource/alicloud_db_instance: encryption_key supports SqlServer([#3538](https://github.com/aliyun/terraform-provider-alicloud/issues/3538))
- resource/alicloud_alikafka_topic: Enlarges the partition_num limitation to 360 and adds more supported regions statement in docs([#3539](https://github.com/aliyun/terraform-provider-alicloud/issues/3539))
- testcast: Adds ddoscoo support region([#3536](https://github.com/aliyun/terraform-provider-alicloud/issues/3536))
- ci: Improves the ci task to output test result coverage([#3541](https://github.com/aliyun/terraform-provider-alicloud/issues/3541))

BUG FIXES:

- resource/alicloud_log_oss_shipper: Fixes the AK not exist error when using sts([#3528](https://github.com/aliyun/terraform-provider-alicloud/issues/3528))
- resource/alicloud_fc_trigger: Removes the empty payload to fix the diff error([#3531](https://github.com/aliyun/terraform-provider-alicloud/issues/3531))
- resource/alicloud_mongodb_instance: Fixes describeing tde status bug when db instance type is single([#3533](https://github.com/aliyun/terraform-provider-alicloud/issues/3533))
- resource/alicloud_slb_server_group: Removes the attribute servers Computed to fix the diff bug when there is no any server ids([#3540](https://github.com/aliyun/terraform-provider-alicloud/issues/3540))
- datasource/alicloud_vpcs: Fixes the vpc datasource bug while invoking the DescribeRouteTableList([#3529](https://github.com/aliyun/terraform-provider-alicloud/issues/3529))

## 1.122.1 (May 8, 2021)

ENHANCEMENTS:

- resource/alicloud_kvstore_instance: Fixes the attribute config does not affect bug when creating a new resource([#3523](https://github.com/aliyun/terraform-provider-alicloud/issues/3523))
- resource/alicloud_ecs_disk: delete param type default ​​and enumerated values([#3522](https://github.com/aliyun/terraform-provider-alicloud/issues/3522))
- resource/alicloud_rds_account: add validFunc for param account name([#3527](https://github.com/aliyun/terraform-provider-alicloud/issues/3527))
- datasource: use Compile replace MustComplile, Catch the error([#3524](https://github.com/aliyun/terraform-provider-alicloud/issues/3524))
- testcase: Fixes the polardb cluster resource and datasource testcase([#3526](https://github.com/aliyun/terraform-provider-alicloud/issues/3526))
- docs: Improves the cs_kubernetes docs([#3512](https://github.com/aliyun/terraform-provider-alicloud/issues/3512))
- docs: update alidns_domain([#3519](https://github.com/aliyun/terraform-provider-alicloud/issues/3519))
- readme: Adds supported version statement([#3513](https://github.com/aliyun/terraform-provider-alicloud/issues/3513))
- ci: Adds compatible test for the provider([#3514](https://github.com/aliyun/terraform-provider-alicloud/issues/3514))
- examples: Removes the useless examples and replaces the deprecated attributes([#3515](https://github.com/aliyun/terraform-provider-alicloud/issues/3515))

## 1.122.0 (April 30, 2021)

- **New Resource:** `alicloud_auto_snapshot_policy_attachment`([#3503](https://github.com/aliyun/terraform-provider-alicloud/issues/3503))
- **New Resource:** `alicloud_cs_kubernetes_permission`([#3495](https://github.com/aliyun/terraform-provider-alicloud/issues/3495))
- **New Resource:** `alicloud_ecs_disk`([#3443](https://github.com/aliyun/terraform-provider-alicloud/issues/3443))
- **New Data Source:** `alicloud_cs_kubernetes_permissions`([#3495](https://github.com/aliyun/terraform-provider-alicloud/issues/3495))
- **New Data Source:** `alicloud_vpc_flow_log`([#3477](https://github.com/aliyun/terraform-provider-alicloud/issues/3477))

ENHANCEMENTS:

- resource/alicloud_network_acl: Supports setting timeout; Adds new attributes status, ingress acl entries and egress acl entries; Upgrades its dependence SDK; Adds its datasource([#3444](https://github.com/aliyun/terraform-provider-alicloud/issues/3444))
- resource/alicloud_disk: Renames alicloud_disk to alicloud_ecs_disk; Deprecates the name and use disk_name instead; Adds more attribute, like payment_type, encrypt_algorithm, auto_snapshot and so on; Upgrades the its dependence sdk([#3443](https://github.com/aliyun/terraform-provider-alicloud/issues/3443)) 
- testcase: Improves the image and instance testcases([#3510](https://github.com/aliyun/terraform-provider-alicloud/issues/3510))
- testcase: Improves the instance testcases([#3504](https://github.com/aliyun/terraform-provider-alicloud/issues/3504))
- testcase: Improves the ess scaling testcase and trigger job([#3502](https://github.com/aliyun/terraform-provider-alicloud/issues/3502))
- testcase: Improves the sweeper testcase([#3498](https://github.com/aliyun/terraform-provider-alicloud/issues/3498))
- testcase: Improves resource alicloud_instance testcase for attribute data_disks([#3497](https://github.com/aliyun/terraform-provider-alicloud/issues/3497))
- testcase: Fixes the has deprecated attribute([#3496](https://github.com/aliyun/terraform-provider-alicloud/issues/3496))
- testcase: Improves the testcase of scaling configurations and manager policy ([#3494](https://github.com/aliyun/terraform-provider-alicloud/issues/3494))
- docs: Fixes TSDB instance document error([#3500](https://github.com/aliyun/terraform-provider-alicloud/issues/3500))
- ci: Improves the ci test in parsing func methods([#3492](https://github.com/aliyun/terraform-provider-alicloud/issues/3492))

BUG FIXES:

- resource/alicloud_log_oss_shipper: Fixes sls oss shipper token bug which unsupporting security token([#3508](https://github.com/aliyun/terraform-provider-alicloud/issues/3508))

## 1.121.3 (April 24, 2021)

ENHANCEMENTS:

- resource/alicloud_polardb_cluster: Improves the attribute tde_status using standard values([#3490](https://github.com/aliyun/terraform-provider-alicloud/issues/3490))
- resource/alicloud_db_instance: Supports to encrypt the disk for MSSQL([#3486](https://github.com/aliyun/terraform-provider-alicloud/issues/3486))
- resource/alicloud_polardb_cluster: Supports new attribute tde_status for PolarDB Mysql([#3485](https://github.com/aliyun/terraform-provider-alicloud/issues/3485))
- testcase: Skipes ResourceManager testcase while the resource directory is not enabled([#3475](https://github.com/aliyun/terraform-provider-alicloud/issues/3475))
- docs/alicloud_vswitch: Replaces deprecated availability_zone with zone _id in the all of docs examples([#3481](https://github.com/aliyun/terraform-provider-alicloud/issues/3481))
- docs: Improves the docs for the attribute period note([#3489](https://github.com/aliyun/terraform-provider-alicloud/issues/3489))
- ci: Improves the running ci testcase and got failed count([#3478](https://github.com/aliyun/terraform-provider-alicloud/issues/3478))
- ci: improve ci testcase by adding point-to-point test when there is a merg([#3472](https://github.com/aliyun/terraform-provider-alicloud/issues/3472))
- ci: Improves the ci-test to get the precise test case([#3483](https://github.com/aliyun/terraform-provider-alicloud/issues/3483))

BUG FIXES:

- resource/alicloud_adb_db_connection: Adds retry error code IncorrectDBInstanceState to fix deleting adb connection failed error([#3491](https://github.com/aliyun/terraform-provider-alicloud/issues/3491))
- datasource/alicloud_nat_gateways: Recovers the ip_lists type to fix the missing expected error([#3480](https://github.com/aliyun/terraform-provider-alicloud/issues/3480))
- ci: Fixes the ci test bug when running the aliyun oss ls command([#3482](https://github.com/aliyun/terraform-provider-alicloud/issues/3482))
- ci: Fixes the CI bug and update changelog([#3469](https://github.com/aliyun/terraform-provider-alicloud/issues/3469))
- ci: improves the test scripts to fix missing parameter bug([#3474](https://github.com/aliyun/terraform-provider-alicloud/issues/3474))

## 1.121.2 (April 18, 2021)

ENHANCEMENTS:

- resource/alicloud_nas_file_system: Removes the attribute kms_key_id because of it does not support all of users([#3464](https://github.com/aliyun/terraform-provider-alicloud/issues/3464))
- resource/alicloud_nas_file_system: Adds new attribute encrypt_type and kms_key_id to support encrypt the resource data([#3431](https://github.com/aliyun/terraform-provider-alicloud/issues/3431))
- resource/alicloud_oss_bucket: Adds attributes created_before_date , expired_object_delete_marker , abort_multipart_upload , noncurrent_version_expiration and noncurrent_version_transition([#3441](https://github.com/aliyun/terraform-provider-alicloud/issues/3441))
- resource/alicloud_instance: Deprecates the useless attribute internet_max_bandwidth_in([#3445](https://github.com/aliyun/terraform-provider-alicloud/issues/3445))
- resource/alicloud_polardb_cluster: Sets attribute vswitch_id to Computed and improve its testcase([#3456](https://github.com/aliyun/terraform-provider-alicloud/issues/3456))
- testcase: Adds the sag qos sweeper test([#3435](https://github.com/aliyun/terraform-provider-alicloud/issues/3435))
- testcase: Improves the hbase and market testcases([#3453](https://github.com/aliyun/terraform-provider-alicloud/issues/3453))
- testcase: Improve hbase instance testcase([#3454](https://github.com/aliyun/terraform-provider-alicloud/issues/3454))
- errors.go: Improves the retry strategy by supporting error code Throttling and ServiceUnavailable([#3437](https://github.com/aliyun/terraform-provider-alicloud/issues/3437))
- errors.go: Improves the connection faild error by adding another error([#3452](https://github.com/aliyun/terraform-provider-alicloud/issues/3452))
- errors: Adds retry error code for throttling error([#3462](https://github.com/aliyun/terraform-provider-alicloud/issues/3462))
- ci: Sync the provider repo to oss to avoid network faild when running in China([#3468](https://github.com/aliyun/terraform-provider-alicloud/issues/3468))

BUG FIXES:

- resource/alicloud_adb_db_cluster: Fixes the diff bug caused by attribute payment_type and db_cluster_category([#3466](https://github.com/aliyun/terraform-provider-alicloud/issues/3466))
- resource/nat_gateway: Recovers the snat_table_ids and forward_table_ids data type to fix the format error([#3432](https://github.com/aliyun/terraform-provider-alicloud/issues/3432))
- resource/alicloud_cen_bandwidth_package: Fixes the parsing expire time failed error which only work in PrePaid([#3436](https://github.com/aliyun/terraform-provider-alicloud/issues/3436))
- resource/alicloud_cen_bandwidth_package: Fixes the InvalidStatus.Resource error when updating this resource([#3440](https://github.com/aliyun/terraform-provider-alicloud/issues/3440))
- resource/alicloud_sag_qos_car & alicloud_sag_qos_policy: Fixes the error ResourceInOperating in concurrent scenario([#3446](https://github.com/aliyun/terraform-provider-alicloud/issues/3446))
- resource/alicloud_network_acl: Fixes the Throttling error when describing the resources([#3447](https://github.com/aliyun/terraform-provider-alicloud/issues/3447))
- resource/alicloud_mongodb_instance: Fixes the InstanceStatusInvalid error when ModifySecurityGroupConfiguration([#3449](https://github.com/aliyun/terraform-provider-alicloud/issues/3449))
- resource/alicloud_cen_xxx: Adds the retry strategy to fix the connection error when fetching the resources([#3450](https://github.com/aliyun/terraform-provider-alicloud/issues/3450))
- resource/alicloud_polardb_account: Adds the retry strategy to fix the ConcurrentTaskExceeded error when update the resources([#3456](https://github.com/aliyun/terraform-provider-alicloud/issues/3456))
- resource/alicloud_nat_gateway: Fixes the specification diff bug; Fixes the period diff bug([#3458](https://github.com/aliyun/terraform-provider-alicloud/issues/3458))
- datasource/alicloud_cms_service: Adds error code Has.effect.suit to avoid needless error when repeated opening([#3463](https://github.com/aliyun/terraform-provider-alicloud/issues/3463))
- testcase/alicloud_cms_alarm_contact: Improves the docs and adds limitation descriptions for attribute name; Fixes the its testcase([#3439](https://github.com/aliyun/terraform-provider-alicloud/issues/3439))
- testcase/alicloud_adb_connection: Fixes its testcase caused by missing mode([#3467](https://github.com/aliyun/terraform-provider-alicloud/issues/3467))
- docs/alicloud_alidns_domain: Corrects the dns_servers spelling error([#3434](https://github.com/aliyun/terraform-provider-alicloud/issues/3434))
- locations: Fixes fetching endpoint failed error because of network connection failed([#3459](https://github.com/aliyun/terraform-provider-alicloud/issues/3459))

## 1.121.1 (April 13, 2021)

ENHANCEMENTS:

- resource/alicloud_ecs_key_pair: Supports retry strategy when deleting to fix the error InvalidParameter.KeypairAlreadyAttachedInstance([#3423](https://github.com/aliyun/terraform-provider-alicloud/issues/3423))
- testcase: Improves the mongodb and ess scaling configuration testcase([#3422](https://github.com/aliyun/terraform-provider-alicloud/issues/3422))
- testcase: Improves the snat entry testcase results from using the new data type([#3424](https://github.com/aliyun/terraform-provider-alicloud/issues/3424))

BUG FIXES:

- docs/alicloud_alidns_domain: Corrects the dns_servers spelling error([#3434](https://github.com/aliyun/terraform-provider-alicloud/issues/3434))
- resource/nat_gateway: Recovers the snat_table_ids and forward_table_ids data type to fix the format error([#3432](https://github.com/aliyun/terraform-provider-alicloud/issues/3432))
- resource/alicloud_adb_db_cluster: Fixes the crash error([#3429](https://github.com/aliyun/terraform-provider-alicloud/issues/3429))
- testcase: Fixes the mongodb and ess testcases([#3421](https://github.com/aliyun/terraform-provider-alicloud/issues/3421))
- docs/zones: Fixes the docs spelling error in the datasource alicloud_xxx_zones([#3425](https://github.com/aliyun/terraform-provider-alicloud/issues/3425))

## 1.121.0 (April 10, 2021)

- **New Resource:** `alicloud_log_oss_shipper`([#3414](https://github.com/aliyun/terraform-provider-alicloud/issues/3414))

ENHANCEMENTS:

- resource/alicloud_db_readonly_instance: Adds force_restart to fix the crash error when modifying the parameters([#3419](https://github.com/aliyun/terraform-provider-alicloud/issues/3419))
- resource/alicloud_polardb_endpoint: Supports new attributes ssl_enabled and net_type([#3408](https://github.com/aliyun/terraform-provider-alicloud/issues/3408))
- resource/alicloud_disk: Sets the attribute kms_key_id to forceNew results from there is no API can update it in local place([#3409](https://github.com/aliyun/terraform-provider-alicloud/issues/3409))
- resource/alicloud_kvstore_instance: Deprecates attributes node_type and it is useless for this resource([#3411](https://github.com/aliyun/terraform-provider-alicloud/issues/3411))
- resource/alicloud_ecs_key_pair: Deprecates the key_name and use key_pair_name instead; Upgrades the its dependence sdk([#3413](https://github.com/aliyun/terraform-provider-alicloud/issues/3413))
- resource/alicloud_nat_gateway: Deprecates name, instance_charge_type and using standard nat_gateway_name and payment_type instead; Supports new attributes 'tags' and 'internet_charge_type'; Upgrade its depend sdk([#3415](https://github.com/aliyun/terraform-provider-alicloud/issues/3415))
- resource/alicloud_fc_function: Attribute code_checksum supports undating in place([#3416](https://github.com/aliyun/terraform-provider-alicloud/issues/3416))
- resource/alicloud_adb_cluster: Upgrades to alicloud_adb_db_cluster; Adds new attributes 'compute_resource', 'db_cluster_class', 'elastic_io_resource', 'mode', 'modify_type', 'payment_type', 'resource_group_id', 'status' attributes; Upgrades its dependence SDK([#3295](https://github.com/aliyun/terraform-provider-alicloud/issues/3295))

## 1.120.0 (April 02, 2021)

- **New Resource:** `alicloud_resource_manager_control_policy`([#3383](https://github.com/aliyun/terraform-provider-alicloud/issues/3383))
- **New Resource:** `alicloud_ga_forwarding_rule`([#3384](https://github.com/aliyun/terraform-provider-alicloud/issues/3384))
- **New Resource:** `alicloud_ecs_snapshot`([#3403](https://github.com/aliyun/terraform-provider-alicloud/issues/3403))
- **Data Source:** `alicloud_resource_manager_control_policies`([#3383](https://github.com/aliyun/terraform-provider-alicloud/issues/3383))
- **Data Source:** `alicloud_ga_forwarding_rules`([#3384](https://github.com/aliyun/terraform-provider-alicloud/issues/3384))
- **Data Source:** `alicloud_sae_service`([#3390](https://github.com/aliyun/terraform-provider-alicloud/issues/3390))
- **Data Source:** `alicloud_rds_accounts`([#3399](https://github.com/aliyun/terraform-provider-alicloud/issues/3399))
- **Data Source:** `alicloud_ecs_snapshots`([#3403](https://github.com/aliyun/terraform-provider-alicloud/issues/3403))

ENHANCEMENTS:

- resource/alicloud_common_bandwidth_package: Renames the name to bandwidth_package_name; Adds new field status; Upgrades its dependence sdk [([#3376](https://github.com/aliyun/terraform-provider-alicloud/issues/3376)))
- resource/alicloud_route_table: Adds retry code to avoid concurrency issues when deleting([#3377](https://github.com/aliyun/terraform-provider-alicloud/issues/3377))
- resource/alicloud_quotas_xxx: Supports setting SourceIp to avoid useless error when using sts to operate([#3388](https://github.com/aliyun/terraform-provider-alicloud/issues/3388))
- resource/alicloud_resource_resource_manager_resource_directory: Supports enable or disable control policy by attribute status([#3391](https://github.com/aliyun/terraform-provider-alicloud/issues/3391))
- resource/alicloud_cs_kunernetes: Supports disk performance level selection, managed cluster migration and cluster tag update([#3397](https://github.com/aliyun/terraform-provider-alicloud/issues/3397))
- resource/alicloud_ecs_snapshot: Deprecates the name and use snapshot_name instead; Adds more attributes; Upgrades the its dependence sdk([#3403](https://github.com/aliyun/terraform-provider-alicloud/issues/3403))
- datasource/alicloud_instance_types: Adds new attribute system_disk_category to filter instance types([#3404](https://github.com/aliyun/terraform-provider-alicloud/issues/3404))
- testcase: Improves the polardb and the related resource testcases([#3379](https://github.com/aliyun/terraform-provider-alicloud/issues/3379))
- testcase: upgrade kvstore instance test case([#3386](https://github.com/aliyun/terraform-provider-alicloud/issues/3386))
- testcase: Skip alidns_domain_attachment test case because of PrePaid and international region([#3387](https://github.com/aliyun/terraform-provider-alicloud/issues/3387))
- testcase: Adds sweeper test for the resource alicloud_cs_kubernetes([#3389](https://github.com/aliyun/terraform-provider-alicloud/issues/3389))
- errors.go: Improves parsing error efficience([#3378](https://github.com/aliyun/terraform-provider-alicloud/issues/3378))
- errors.go: Improves the error matching function to avoid some useless error [3406]

BUG FIXES:
- resource/alicloud_emr_cluster: Fixes the attribute use_local_metadb diff bug([#3401](https://github.com/aliyun/terraform-provider-alicloud/issues/3401))
- resource/alicloud_alikafka_instance: Fixes creating error ONS_SYSTEM_ERROR and deleting timeout error([#3380](https://github.com/aliyun/terraform-provider-alicloud/issues/3380))
- resource/alicloud_snat_entry: Adds retry code to fix the creating error InternalError([#3382](https://github.com/aliyun/terraform-provider-alicloud/issues/3382))
- resource/alicloud_ga_forwarding_rule: improve ga_forwarding_rule([#3392](https://github.com/aliyun/terraform-provider-alicloud/issues/3392))
- resource/ga_bandwidth_package_id: Upgrades the resource id using both bandwidth package id and accelerator id([#3393](https://github.com/aliyun/terraform-provider-alicloud/issues/3393))
- resource/alicloud_havip: Adds its datasource; adds new attributes havip_name and status; upgrades its dependence sdk([#3394](https://github.com/aliyun/terraform-provider-alicloud/issues/3394))
- resource/alicloud_keypair_attachment: Fix KeyPairAttachment bug when the key pair name contains colon([#3395](https://github.com/aliyun/terraform-provider-alicloud/issues/3395))

## 1.119.1 (March 26, 2021)

ENHANCEMENTS:

- resource/alicloud_route_table: Adds retry code to avoid concurrency issues when deleting([#3377](https://github.com/aliyun/terraform-provider-alicloud/issues/3377))
- resource/alicloud_cs_managed_kubernetes: Supports setting essd disk performance and automatic disk snapshot policies for cluster and node pool nodes.([#3371](https://github.com/aliyun/terraform-provider-alicloud/issues/3371))
- resource/alicloud_forward_entry: Renames the name to forward_entry_name; Supports new attribute protocol; Upgrades the resource SDK([#3368](https://github.com/aliyun/terraform-provider-alicloud/issues/3368))
- resource/alicloud_eip_association: Enlarges the deletion timeout to avoid deleting it failed([#3366](https://github.com/aliyun/terraform-provider-alicloud/issues/3366))
- resource/alicloud_eip_assocition: Enlarges the client connection timeout to avoid connecting failed([#3365](https://github.com/aliyun/terraform-provider-alicloud/issues/3365))
- resource/alicloud_mongodb_instance: Removes the field tde_status forceNew and supports modifying it online([#3360](https://github.com/aliyun/terraform-provider-alicloud/issues/3360))
- resource/alicloud_ga_listener: Supports protocol HTTP and HTTPS([#3358](https://github.com/aliyun/terraform-provider-alicloud/issues/3358))
- resource/alicloud_snat_entry: Adds new attribute status and supports self-define timeout; Upgrades the resource dependent sdk([#3357](https://github.com/aliyun/terraform-provider-alicloud/issues/3357))
- resource/alicloud_vswitch: Leverages the specified error code to add retry strategy when creating or deleting vswitch([#3356](https://github.com/aliyun/terraform-provider-alicloud/issues/3356))
- testcase: Modify the image name_regex to ^ubuntu to avoid the needless test failed([#3367](https://github.com/aliyun/terraform-provider-alicloud/issues/3367))

BUG FIXES:

- resource/alicloud_vpc,alicloud_vswitch: Fixes DependencyViolation error when deleting vpc and vswitch([#3370](https://github.com/aliyun/terraform-provider-alicloud/issues/3370))
- resource/alicloud_eip_association: Fixes the connection timeout when getting Eip resource([#3369](https://github.com/aliyun/terraform-provider-alicloud/issues/3369))

## 1.119.0 (March 19, 2021)

- **New Resource:** `alicloud_rds_parameter_group`([#3343](https://github.com/aliyun/terraform-provider-alicloud/issues/3343))
- **Data Source:** `alicloud_rds_parameter_groups`([#3343](https://github.com/aliyun/terraform-provider-alicloud/issues/3343)) 

ENHANCEMENTS:

- resource/alicloud_cs_kubernetes_node_pool: Supports new feature including subscription charge type, installing cloud momitor, setting node unschedulable([#3351](https://github.com/aliyun/terraform-provider-alicloud/issues/3351))
- resource/alicloud_ga_bandwidth_package: Supports updating attributebandwidth([#3346](https://github.com/aliyun/terraform-provider-alicloud/issues/3346))
- resource/alicloud_alikafka_topic: Supports setting self-define create timeout([#3345](https://github.com/aliyun/terraform-provider-alicloud/issues/3345))
- resource/alicloud_vswitch: Upgrades vswitch including deprecating name and availability_zone, adding vswitch_name and zone_id, using new sdk([#3342](https://github.com/aliyun/terraform-provider-alicloud/issues/3342))
- resource/alicloud_alicloud_tsdb_instance: Improves codes by modifying its conversion function name([#3337](https://github.com/aliyun/terraform-provider-alicloud/issues/3337))
- resource/alicloud_vpc: Adds new features including renaming name to vpc_name, enabling ipv6, setting user_cidrs and upgrading sdk([#3328](https://github.com/aliyun/terraform-provider-alicloud/issues/3328))
- datasource/alicloud_cms_monitor_group_instances: Rename instanceses to instances([#3349](https://github.com/aliyun/terraform-provider-alicloud/issues/3349))
- testcase: Improves the fc sweeper test with adding deleting fc-eni([#3354](https://github.com/aliyun/terraform-provider-alicloud/issues/3354))
- testcase: Adds supported regions for vpc testcase([#3353](https://github.com/aliyun/terraform-provider-alicloud/issues/3353))
- testcase: Upgrades alicloud_vpc and alicloud_vswitch testcases including change field name to vpc_name and vswitch_name([#3344](https://github.com/aliyun/terraform-provider-alicloud/issues/3344))
- testcase: Improves the mns and nas filesystem testcase by skipping needless cases([#3339](https://github.com/aliyun/terraform-provider-alicloud/issues/3339))

BUG FIXES:

- resource/alicloud_keypair_attachment: Fix DescribeKeyPairAttachment bug(#3338) when the key pair name contains colon([#3341](https://github.com/aliyun/terraform-provider-alicloud/issues/3341))
- resource/alicloud_cs_kubernetes: Fixes GetClusterConfig failed error when the cluster state is failed([#3340](https://github.com/aliyun/terraform-provider-alicloud/issues/3340))
- datasource/alicloud_fc_service: Fixes enable fc service twice error and supports idempotent([#3348](https://github.com/aliyun/terraform-provider-alicloud/issues/3348))

## 1.118.0 (March 12, 2021)

FEATURES:

- **Data Source:** `alicloud_mns_service`([#3325](https://github.com/aliyun/terraform-provider-alicloud/issues/3325))
- **Data Source:** `alicloud_dataworks_service`([#3333](https://github.com/aliyun/terraform-provider-alicloud/issues/3333))

ENHANCEMENTS:

- resource/alicloud_cms_group_metric_rule: Adds NotFount error code to avoid needless error after deleting the resource([#3317](https://github.com/aliyun/terraform-provider-alicloud/issues/3317))
- testcase: Improves the ResourceManager sweep testcase([#3320](https://github.com/aliyun/terraform-provider-alicloud/issues/3320))
- testcase: Improves ess test case([#3321](https://github.com/aliyun/terraform-provider-alicloud/issues/3321))
- resource/alicloud_cdn_domain_new: Removes the maxitems limit for it attributes `sources` and can support setting multiple values([#3323](https://github.com/aliyun/terraform-provider-alicloud/issues/3323))
- testcase: Adds regionId for ecs auto snap policy sweeper testcase.([#3326](https://github.com/aliyun/terraform-provider-alicloud/issues/3326))
- docs: Corrects the resource alicloud_alidns_instance website sidebar names([#3329](https://github.com/aliyun/terraform-provider-alicloud/issues/3329))
- testcase: Improve the resource fc_domain ci test case([#3331](https://github.com/aliyun/terraform-provider-alicloud/issues/3331))
- resource/alicloud_actiontrail_trail: Upgrades the api version of actiontrail to deprecate the attribute `mns_topic_arn` and `role_name` and add new attribute `oss_write_role_arn`([#3334](https://github.com/aliyun/terraform-provider-alicloud/issues/3334))
- resource/alicloud_ram_policy: Deletes all of policy versions when deleting one ram policy([#3332](https://github.com/aliyun/terraform-provider-alicloud/issues/3332))

BUG FIXES:

- testcase: Fix dms user datasource test bug.([#3324](https://github.com/aliyun/terraform-provider-alicloud/issues/3324))
- testcase: Fix resource alicloud_resource_cdn_domain_new test case.([#3327](https://github.com/aliyun/terraform-provider-alicloud/issues/3327))
- testcase: Fix resource manager sweeper test case([#3330](https://github.com/aliyun/terraform-provider-alicloud/issues/3330))
- resource/alicloud_cs_kubernetes: Fix the resource crash error when creating dedicated cluster in v1.117.0([#3335](https://github.com/aliyun/terraform-provider-alicloud/issues/3335))


## 1.117.0 (March 05, 2021)

- **New Resource:** `alicloud_vpc_flow_log`([#3290](https://github.com/aliyun/terraform-provider-alicloud/issues/3290))
- **New Resource:** `alicloud_brain_industrial_pid_loop`([#3252](https://github.com/aliyun/terraform-provider-alicloud/issues/3252))
- **Data Source:** `alicloud_brain_industrial_pid_loops`([#3252](https://github.com/aliyun/terraform-provider-alicloud/issues/3252))
- **Data Source:** `alicloud_maxcompute_service`([#3304](https://github.com/aliyun/terraform-provider-alicloud/issues/3304))
- **Data Source:** `alicloud_cloud_storage_gateway_service`([#3308](https://github.com/aliyun/terraform-provider-alicloud/issues/3308))
- **Data Source:** `alicloud_ecs_auoto_snapshot_policies`([#3309](https://github.com/aliyun/terraform-provider-alicloud/issues/3309))

IMPROVEMENTS:

- support load balancer spec([#3305](https://github.com/aliyun/terraform-provider-alicloud/issues/3305))
- resource/alicloud_brain_industrial_pid_project: fix name spelling mistake([#3310](https://github.com/aliyun/terraform-provider-alicloud/issues/3310))
- resource/alicloud_eip_association: supports importing feature([#3312](https://github.com/aliyun/terraform-provider-alicloud/issues/3312))
- product/quotas: rename ApplicationInfo to QuotaApplication.([#3311](https://github.com/aliyun/terraform-provider-alicloud/issues/3311))
- resource/image_copy: adding missing status when waiting for available([#3314](https://github.com/aliyun/terraform-provider-alicloud/issues/3314))
- resource alicloud_snapshot_policy renamed to alicloud_ecs_auto_snapshot_policy([#3309](https://github.com/aliyun/terraform-provider-alicloud/issues/3309))

BUG FIXES:

- fix ack_service type parameter([#3307](https://github.com/aliyun/terraform-provider-alicloud/issues/3307))

## 1.116.0 (February 27, 2021)

- **New Resource:** `alicloud_ecs_hpc_cluster`([#3303](https://github.com/aliyun/terraform-provider-alicloud/issues/3303))
- **New Resource:** `alicloud_cloud_storage_gateway_storage_bundle`([#3297](https://github.com/aliyun/terraform-provider-alicloud/issues/3297))
- **New Resource:** `alicloud_ecs_command`([#3296](https://github.com/aliyun/terraform-provider-alicloud/issues/3296))
- **New Resource:** `alicloud_quotas_quota_alarm`([#3293](https://github.com/aliyun/terraform-provider-alicloud/issues/3293))
- **Data Source:** `alicloud_ecs_hpc_clusters`([#3303](https://github.com/aliyun/terraform-provider-alicloud/issues/3303))
- **Data Source:** `alicloud_cloud_storage_gateway_storage_bundles`([#3297](https://github.com/aliyun/terraform-provider-alicloud/issues/3297))
- **Data Source:** `alicloud_ecs_commands`([#3296](https://github.com/aliyun/terraform-provider-alicloud/issues/3296))
- **Data Source:** `alicloud_cr_service`([#3294](https://github.com/aliyun/terraform-provider-alicloud/issues/3294))
- **Data Source:** `alicloud_quotas_quota_alarms`([#3293](https://github.com/aliyun/terraform-provider-alicloud/issues/3293))
- **Data Source:** `alicloud_vs_service`([#3292](https://github.com/aliyun/terraform-provider-alicloud/issues/3292))

IMPROVEMENTS:

- change ecs endpoint([#3299](https://github.com/aliyun/terraform-provider-alicloud/issues/3299))
- resource/alicloud_privatelink: Add compute for bandwidth([#3291](https://github.com/aliyun/terraform-provider-alicloud/issues/3291))
- Add auto retry for cms_group_metric_rule, fix ons_instance datasource crash error and modify jsonpath get response deal([#3288](https://github.com/aliyun/terraform-provider-alicloud/issues/3288))
- add support 'Australia' of 'alicloud_cen_bandwidth_package'([#3287](https://github.com/aliyun/terraform-provider-alicloud/issues/3287))
- Modify security_group_rule describe method retry timeout([#3282](https://github.com/aliyun/terraform-provider-alicloud/issues/3282))
- change dms to common([#3280](https://github.com/aliyun/terraform-provider-alicloud/issues/3280))
- update changelog([#3279](https://github.com/aliyun/terraform-provider-alicloud/issues/3279))

## 1.115.1 (February 07, 2021)

IMPROVEMENTS:

- update go vendors([#3281](https://github.com/aliyun/terraform-provider-alicloud/issues/3281))
- datasource/ram_policies: support system policy type to filter policies([#3276](https://github.com/aliyun/terraform-provider-alicloud/issues/3276))
- fix the error of parameters description in alicloud_polardb_cluster's doc([#3272](https://github.com/aliyun/terraform-provider-alicloud/issues/3272))
- resource/alicloud_hbase_cluster: add some value check; remove classic([#3174](https://github.com/aliyun/terraform-provider-alicloud/issues/3174))

## 1.115.0 (February 07, 2021)

- **New Resource:** `alicloud_cms_monitor_group_instances`([#3267](https://github.com/aliyun/terraform-provider-alicloud/issues/3267))
- **New Resource:** `alicloud_quotas_application_info`([#3261](https://github.com/aliyun/terraform-provider-alicloud/issues/3261))
- **Data Source:** `alicloud_iot_service`([#3270](https://github.com/aliyun/terraform-provider-alicloud/issues/3270))
- **Data Source:** `alicloud_cms_monitor_group_instanceses`([#3267](https://github.com/aliyun/terraform-provider-alicloud/issues/3267))
- **Data Source:** `alicloud_brain_industrial_service`([#3266](https://github.com/aliyun/terraform-provider-alicloud/issues/3266))
- **Data Source:** `alicloud_quotas_quotas`([#3265](https://github.com/aliyun/terraform-provider-alicloud/issues/3265))
- **Data Source:** `alicloud_quotas_application_infos`([#3261](https://github.com/aliyun/terraform-provider-alicloud/issues/3261))

IMPROVEMENTS:

- resource/privatelink_vpc_endpoint_zone: Add wait state for create([#3278](https://github.com/aliyun/terraform-provider-alicloud/issues/3278))
- resource support update resource_group_id([#3277](https://github.com/aliyun/terraform-provider-alicloud/issues/3277))
- change pvtz to common sdk([#3275](https://github.com/aliyun/terraform-provider-alicloud/issues/3275))
- Change NAS to common SDK([#3273](https://github.com/aliyun/terraform-provider-alicloud/issues/3273))
- changelog([#3268](https://github.com/aliyun/terraform-provider-alicloud/issues/3268))

## 1.114.1 (February 01, 2021)

IMPROVEMENTS:

- remove useless docs([#3269](https://github.com/aliyun/terraform-provider-alicloud/issues/3269))

BUG FIXES:

- Fix the client bug for central resource ([#3264](https://github.com/aliyun/terraform-provider-alicloud/issues/3264))

## 1.114.0 (January 29, 2021)

- **New Resource:** `alicloud_ram_saml_provider`([#3235](https://github.com/aliyun/terraform-provider-alicloud/issues/3235))
- **Data Source:** `alicloud_fnf_service`([#3258](https://github.com/aliyun/terraform-provider-alicloud/issues/3258))
- **Data Source:** `alicloud_pvtz_service`([#3237](https://github.com/aliyun/terraform-provider-alicloud/issues/3237))
- **Data Source:** `alicloud_ram_saml_providers`([#3235](https://github.com/aliyun/terraform-provider-alicloud/issues/3235))

IMPROVEMENTS:

- resource/alicloud_ga_xxx: adding retry error code([#3260](https://github.com/aliyun/terraform-provider-alicloud/issues/3260))
- Update SDK to v1.61.877([#3251](https://github.com/aliyun/terraform-provider-alicloud/issues/3251))
- generate ram policy from amp([#3249](https://github.com/aliyun/terraform-provider-alicloud/issues/3249))
- update changelog([#3248](https://github.com/aliyun/terraform-provider-alicloud/issues/3248))
- Change ResourceManager to common SDK([#3247](https://github.com/aliyun/terraform-provider-alicloud/issues/3247))
- resource/alicloud_polardb_cluster: support enable audit log collector([#3246](https://github.com/aliyun/terraform-provider-alicloud/issues/3246))
- add type attribute for ack_service([#3244](https://github.com/aliyun/terraform-provider-alicloud/issues/3244))
- improve datasource alicloud_db_instance_classes and engines([#3236](https://github.com/aliyun/terraform-provider-alicloud/issues/3236))
- improve docs subcategory([#3233](https://github.com/aliyun/terraform-provider-alicloud/issues/3233))
- support emr importer feature and optimized test case([#3232](https://github.com/aliyun/terraform-provider-alicloud/issues/3232))
- resource/alicloud_kvstore_instance: Modify code of private_connection_prefix([#3231](https://github.com/aliyun/terraform-provider-alicloud/issues/3231))
- update: add support for nat from normal to enhanced([#3230](https://github.com/aliyun/terraform-provider-alicloud/issues/3230))
- change oos to common([#3227](https://github.com/aliyun/terraform-provider-alicloud/issues/3227))
- datasource/alicloud_oss_service: supporting more opened error codes([#3226](https://github.com/aliyun/terraform-provider-alicloud/issues/3226))
- update changelog([#3225](https://github.com/aliyun/terraform-provider-alicloud/issues/3225))
- Modify Ons product to common type([#3218](https://github.com/aliyun/terraform-provider-alicloud/issues/3218))
- Remove duplicate `tags`([#3200](https://github.com/aliyun/terraform-provider-alicloud/issues/3200))
- Remove Japan site([#2999](https://github.com/aliyun/terraform-provider-alicloud/issues/2999))

BUG FIXES:

- fix ga doc resource create error([#3257](https://github.com/aliyun/terraform-provider-alicloud/issues/3257))
- fix err when delete adb cluster([#3234](https://github.com/aliyun/terraform-provider-alicloud/issues/3234))

## 1.113.0 (January 15, 2021)

- **New Resource:** `alicloud_eipanycast_anycast_eip_address_attachment`([#3215](https://github.com/aliyun/terraform-provider-alicloud/issues/3215))
- **New Resource:** `alicloud_brain_industrial_pid_project`([#3212](https://github.com/aliyun/terraform-provider-alicloud/issues/3212))
- **New Resource:** `alicloud_ga_ip_set`([#3211](https://github.com/aliyun/terraform-provider-alicloud/issues/3211))
- **New Resource:** `alicloud_brain_industrial_pid_organization`([#3209](https://github.com/aliyun/terraform-provider-alicloud/issues/3209))
- **New Resource:** `alicloud_ga_bandwidth_package_attachment`([#3207](https://github.com/aliyun/terraform-provider-alicloud/issues/3207))
- **New Resource:** `alicloud_cms_monitor_group`([#3204](https://github.com/aliyun/terraform-provider-alicloud/issues/3204))
- **New Resource:** `alicloud_ga_endpoint_group`([#3202](https://github.com/aliyun/terraform-provider-alicloud/issues/3202))
- **New Resource:** `alicloud_eipanycast_anycast_eip_address`([#3198](https://github.com/aliyun/terraform-provider-alicloud/issues/3198))
- **Data Source:** `alicloud_privatelink_service`([#3224](https://github.com/aliyun/terraform-provider-alicloud/issues/3224))
- **Data Source:** `alicloud_ack_service`([#3221](https://github.com/aliyun/terraform-provider-alicloud/issues/3221))
- **Data Source:** `alicloud_brain_industrial_pid_projects`([#3212](https://github.com/aliyun/terraform-provider-alicloud/issues/3212))
- **Data Source:** `alicloud_ga_ip_sets`([#3211](https://github.com/aliyun/terraform-provider-alicloud/issues/3211))
- **Data Source:** `alicloud_brain_industrial_pid_organizations`([#3209](https://github.com/aliyun/terraform-provider-alicloud/issues/3209))
- **Data Source:** `alicloud_cms_monitor_groups`([#3204](https://github.com/aliyun/terraform-provider-alicloud/issues/3204))
- **Data Source:** `alicloud_ga_endpoint_groups`([#3202](https://github.com/aliyun/terraform-provider-alicloud/issues/3202))
- **Data Source:** `alicloud_eipanycast_anycast_eip_addresses`([#3198](https://github.com/aliyun/terraform-provider-alicloud/issues/3198))

IMPROVEMENTS:

- resource/alicloud_nat_gateway: offline Normal NatGateway([#3219](https://github.com/aliyun/terraform-provider-alicloud/issues/3219))
- resource/tsdb_instance: Add resource no found error code([#3217](https://github.com/aliyun/terraform-provider-alicloud/issues/3217))
- update pipeline([#3216](https://github.com/aliyun/terraform-provider-alicloud/issues/3216))
- Add sweeper for privatelink and ros([#3214](https://github.com/aliyun/terraform-provider-alicloud/issues/3214))
- Modify asynchronous to synchronous when delete adb cluster([#3190](https://github.com/aliyun/terraform-provider-alicloud/issues/3190))

BUG FIXES:

- fix some test case([#3222](https://github.com/aliyun/terraform-provider-alicloud/issues/3222))
- fix cs_edge_kubernetes missing force_update parameter([#3220](https://github.com/aliyun/terraform-provider-alicloud/issues/3220))
- testcast/tsdb_instance: fix valid zones([#3213](https://github.com/aliyun/terraform-provider-alicloud/issues/3213))
- datasource/alicloud_api_gateway_apis: fix testcaas error([#3210](https://github.com/aliyun/terraform-provider-alicloud/issues/3210))

## 1.112.0 (January 12, 2021)

- **New Resource:** `alicloud_ga_bandwidth_package`([#3194](https://github.com/aliyun/terraform-provider-alicloud/issues/3194))
- **New Resource:** `alicloud_tsdb_instance`([#3192](https://github.com/aliyun/terraform-provider-alicloud/issues/3192))
- **Data Source:** `alicloud_ga_bandwidth_packages`([#3194](https://github.com/aliyun/terraform-provider-alicloud/issues/3194))
- **Data Source:** `alicloud_tsdb_instances`([#3192](https://github.com/aliyun/terraform-provider-alicloud/issues/3192))
- **Data Source:** `alicloud_tsdb_zones`([#3192](https://github.com/aliyun/terraform-provider-alicloud/issues/3192))
- **Data Source:** `alicloud_fc_service`([#3191](https://github.com/aliyun/terraform-provider-alicloud/issues/3191))

IMPROVEMENTS:

- Feature/modify tde with custom key for mysql([#3208](https://github.com/aliyun/terraform-provider-alicloud/issues/3208))
- sync the alikafka sdk vendor([#3206](https://github.com/aliyun/terraform-provider-alicloud/issues/3206))
- change actiontrail to common([#3193](https://github.com/aliyun/terraform-provider-alicloud/issues/3193))
- improve slb test cases([#3188](https://github.com/aliyun/terraform-provider-alicloud/issues/3188))
- mysql ModifyDBInstanceTDE support custom EncryptionKey([#3186](https://github.com/aliyun/terraform-provider-alicloud/issues/3186))
- change mse cluster to common([#3184](https://github.com/aliyun/terraform-provider-alicloud/issues/3184))
- alikafka support new params when create instance([#3183](https://github.com/aliyun/terraform-provider-alicloud/issues/3183))
- update changelog([#3180](https://github.com/aliyun/terraform-provider-alicloud/issues/3180))
- resource/alicloud_vpc: supports new attribute secondary_cidr_blocks([#3152](https://github.com/aliyun/terraform-provider-alicloud/issues/3152))

BUG FIXES:

- resource/alicloud_alikafka_instance: fix test case param error([#3203](https://github.com/aliyun/terraform-provider-alicloud/issues/3203))
- fix/alicloud_slb: fix the diff bug when setting ipv6([#3187](https://github.com/aliyun/terraform-provider-alicloud/issues/3187))
- fix/provider: improve endpoint when building a new client([#3185](https://github.com/aliyun/terraform-provider-alicloud/issues/3185))

## 1.111.0 (December 31, 2020)

- **New Resource:** `alicloud_ga_listener`([#3173](https://github.com/aliyun/terraform-provider-alicloud/issues/3173))
- **New Resource:** `alicloud_resource_manager_shared_resource`([#3168](https://github.com/aliyun/terraform-provider-alicloud/issues/3168))
- **New Resource:** `alicloud_resource_manager_shared_target`([#3168](https://github.com/aliyun/terraform-provider-alicloud/issues/3168))
- **New Resource:** `alicloud_eci_container_group`([#3166](https://github.com/aliyun/terraform-provider-alicloud/issues/3166))
- **New Resource:** `alicloud_privatelink_vpc_endpoint_zone`([#3163](https://github.com/aliyun/terraform-provider-alicloud/issues/3163))
- **New Resource:** `alicloud_ga_accelerator`([#3162](https://github.com/aliyun/terraform-provider-alicloud/issues/3162))
- **New Resource:** `alicloud_resource_manager_resource_share`([#3158](https://github.com/aliyun/terraform-provider-alicloud/issues/3158))
- **Data Source:** `alicloud_dcdn_service`([#3177](https://github.com/aliyun/terraform-provider-alicloud/issues/3177))
- **Data Source:** `alicloud_ga_listeners`([#3173](https://github.com/aliyun/terraform-provider-alicloud/issues/3173))
- **Data Source:** `alicloud_resource_manager_shared_resources`([#3168](https://github.com/aliyun/terraform-provider-alicloud/issues/3168))
- **Data Source:** `alicloud_resource_manager_shared_targets`([#3168](https://github.com/aliyun/terraform-provider-alicloud/issues/3168))
- **Data Source:** `alicloud_datahub_service`([#3167](https://github.com/aliyun/terraform-provider-alicloud/issues/3167))
- **Data Source:** `alicloud_eci_container_groups`([#3166](https://github.com/aliyun/terraform-provider-alicloud/issues/3166))
- **Data Source:** `alicloud_ons_service`([#3164](https://github.com/aliyun/terraform-provider-alicloud/issues/3164))
- **Data Source:** `alicloud_privatelink_vpc_endpoint_zones`([#3163](https://github.com/aliyun/terraform-provider-alicloud/issues/3163))
- **Data Source:** `alicloud_ga_accelerators`([#3162](https://github.com/aliyun/terraform-provider-alicloud/issues/3162))
- **Data Source:** `alicloud_cms_service`([#3161](https://github.com/aliyun/terraform-provider-alicloud/issues/3161))
- **Data Source:** `alicloud_resource_manager_resource_shares`([#3158](https://github.com/aliyun/terraform-provider-alicloud/issues/3158))

IMPROVEMENTS:

- resource/alicloud_db_account_privilege: add retry for error InvalidDBNotFound([#3176](https://github.com/aliyun/terraform-provider-alicloud/issues/3176))
- data/alicloud_kms_service: adding note for terms of service([#3175](https://github.com/aliyun/terraform-provider-alicloud/issues/3175))
- resource/alicloud_privatelink_xxx: update security_group_id to security_group_ids([#3172](https://github.com/aliyun/terraform-provider-alicloud/issues/3172))
- Feature: alicloud_cs_kubernetes_node_pool support autoscaling nodepool([#3171](https://github.com/aliyun/terraform-provider-alicloud/issues/3171))
- Modify the method of setting id for cms_site_monitor resource([#3170](https://github.com/aliyun/terraform-provider-alicloud/issues/3170))
- resource/alicloud_log_project: supports Tags([#3169](https://github.com/aliyun/terraform-provider-alicloud/issues/3169))
- Add Not Found error for DescribeMetricRuleList Api([#3160](https://github.com/aliyun/terraform-provider-alicloud/issues/3160))
- update changelog([#3159](https://github.com/aliyun/terraform-provider-alicloud/issues/3159))

BUG FIXES:

- resource/alicloud_db_account_privilege: fix deleting other privileges bug([#3178](https://github.com/aliyun/terraform-provider-alicloud/issues/3178))
- fix pvtz_zone_record paging error([#3165](https://github.com/aliyun/terraform-provider-alicloud/issues/3165))

## 1.110.0 (December 26, 2020)

- **New Resource:** `alicloud_privatelink_vpc_endpoint_service_resource`([#3154](https://github.com/aliyun/terraform-provider-alicloud/issues/3154))
- **New Resource:** `alicloud_privatelink_vpc_endpoint_service_user`([#3153](https://github.com/aliyun/terraform-provider-alicloud/issues/3153))
- **New Resource:** `alicloud_privatelink_vpc_endpoint_connection`([#3145](https://github.com/aliyun/terraform-provider-alicloud/issues/3145))
- **Data Source:** `alicloud_privatelink_vpc_endpoint_service_resources`([#3154](https://github.com/aliyun/terraform-provider-alicloud/issues/3154))
- **Data Source:** `alicloud_privatelink_vpc_endpoint_service_users`([#3153](https://github.com/aliyun/terraform-provider-alicloud/issues/3153))
- **Data Source:** `alicloud_privatelink_vpc_endpoint_connections`([#3145](https://github.com/aliyun/terraform-provider-alicloud/issues/3145))

IMPROVEMENTS:

- Feature/rds disk encryption for mysql([#3156](https://github.com/aliyun/terraform-provider-alicloud/issues/3156))
- resource disk_attachment support import([#3151](https://github.com/aliyun/terraform-provider-alicloud/issues/3151))
- Add NotFound Message for cms_alarm resource([#3148](https://github.com/aliyun/terraform-provider-alicloud/issues/3148))
- resource/alicloud_fnf_flow: Add enumerate value for 'type'([#3146](https://github.com/aliyun/terraform-provider-alicloud/issues/3146))
- update changelog([#3142](https://github.com/aliyun/terraform-provider-alicloud/issues/3142))
- resource/zone_attachment:upgrade zone_attachment to teadsl sdk([#3125](https://github.com/aliyun/terraform-provider-alicloud/issues/3125))
- rsource/alicloud_maxcompute_project: Generated by apispec([#3087](https://github.com/aliyun/terraform-provider-alicloud/issues/3087))

BUG FIXES:

- datasource/fnf_flows,fnf_schedules: fix datasource([#3157](https://github.com/aliyun/terraform-provider-alicloud/issues/3157))
- resource/alicloud_security_group_rule: Fix batch creation bug([#3149](https://github.com/aliyun/terraform-provider-alicloud/issues/3149))

## 1.109.1 (December 21, 2020)

IMPROVEMENTS:

- Feature: managedk8s support zero node, management nodepool and remove nodepool nodes([#3140](https://github.com/aliyun/terraform-provider-alicloud/issues/3140))

BUG FIXES:

- resource/ecs_instance: fix the period bug([#3130](https://github.com/aliyun/terraform-provider-alicloud/issues/3130))

## 1.109.0 (December 19, 2020)

- **New Resource:** `alicloud_privatelink_vpc_endpoint`([#3134](https://github.com/aliyun/terraform-provider-alicloud/issues/3134))
- **New Resource:** `alicloud_privatelink_vpc_endpoint_service`([#3126](https://github.com/aliyun/terraform-provider-alicloud/issues/3126))
- **Data Source:** `alicloud_privatelink_vpc_endpoints`([#3134](https://github.com/aliyun/terraform-provider-alicloud/issues/3134))
- **Data Source:** `alicloud_privatelink_vpc_endpoint_services`([#3126](https://github.com/aliyun/terraform-provider-alicloud/issues/3126))

IMPROVEMENTS:

- Modify the Supported value of the attribute in the alicloud_elasticsearch_instance([#3136](https://github.com/aliyun/terraform-provider-alicloud/issues/3136))
- resource/alicloud_hbase_cluster: support new field immediate_delete_flag and cloud_essd([#3133](https://github.com/aliyun/terraform-provider-alicloud/issues/3133))
- resource/alicloud_db_backup_policy: remove the uncertain valid values([#3132](https://github.com/aliyun/terraform-provider-alicloud/issues/3132))
- UPDATE CHANGELOG([#3124](https://github.com/aliyun/terraform-provider-alicloud/issues/3124))
- Generator dcdn_domain resource and datasource by common api([#3123](https://github.com/aliyun/terraform-provider-alicloud/issues/3123))
- resource/alicloud_db_instance: support encryption_key for PG([#3121](https://github.com/aliyun/terraform-provider-alicloud/issues/3121))
- adapter zone record datasource and resource([#3117](https://github.com/aliyun/terraform-provider-alicloud/issues/3117))

BUG FIXES:

- resource/alicloud_instance: fix ecs disk performance tf plan bug([#3139](https://github.com/aliyun/terraform-provider-alicloud/issues/3139))
- fix privatelink client code error([#3129](https://github.com/aliyun/terraform-provider-alicloud/issues/3129))

## 1.108.0 (December 11, 2020)

- **New Resource:** `alicloud_ros_template`([#3113](https://github.com/aliyun/terraform-provider-alicloud/issues/3113))
- **Data Source:** `alicloud_kms_service`([#3116](https://github.com/aliyun/terraform-provider-alicloud/issues/3116))
- **Data Source:** `alicloud_ros_templates`([#3113](https://github.com/aliyun/terraform-provider-alicloud/issues/3113))

IMPROVEMENTS:

- add ecs instance system_disk_performance_level and datadisk performamce_level params([#3120](https://github.com/aliyun/terraform-provider-alicloud/issues/3120))
- resource/alicloud_pvtz_zone: change to tea dsl sdk([#3094](https://github.com/aliyun/terraform-provider-alicloud/issues/3094))

BUG FIXES:

- fix product pvtz gettting endpoint bug([#3122](https://github.com/aliyun/terraform-provider-alicloud/issues/3122))
- BugFix: v1.103.2 upgrade error, connections return error([#3118](https://github.com/aliyun/terraform-provider-alicloud/issues/3118))

## 1.107.0 (December 8, 2020)

- **New Resource:** `alicloud_ros_stack_group` (([#3109](https://github.com/aliyun/terraform-provider-alicloud/issues/3109)))
- **Data Source:** `alicloud_ros_stack_groups` (([#3109](https://github.com/aliyun/terraform-provider-alicloud/issues/3109)))

IMPROVEMENTS:

- resource/alicloud_instance: fix period does not work bug([#3114](https://github.com/aliyun/terraform-provider-alicloud/issues/3114))
- Resource/pvtz_zone: Change IsEOFError to NeedRetry (([#3108](https://github.com/aliyun/terraform-provider-alicloud/issues/3108)))
- resource/alicloud_kvstore_instance: Add a restriction !d.IsNewResource for the update of param private_connection_prefix. (([#3107](https://github.com/aliyun/terraform-provider-alicloud/issues/3107)))
- Error: Change IsEOFError to NeedRerty (([#3106](https://github.com/aliyun/terraform-provider-alicloud/issues/3106)))
- resource/alicloud_hbase_instance: change core_disk_instance to optional (([#3105](https://github.com/aliyun/terraform-provider-alicloud/issues/3105)))
- Resource/security_group_rule: Add retry wait for rule exist. (([#3102](https://github.com/aliyun/terraform-provider-alicloud/issues/3102)))
- datasource/ros_stacks: Add tags and parameters for output. (([#3101](https://github.com/aliyun/terraform-provider-alicloud/issues/3101)))

## 1.106.0 (December 4, 2020)

- **New Resource:** `alicloud_ros_change_set`([#3083](https://github.com/aliyun/terraform-provider-alicloud/issues/3083))
- **Data Source:** `alicloud_hbase_instance_types`([#3091](https://github.com/aliyun/terraform-provider-alicloud/issues/3091))
- **Data Source:** `alicloud_ros_change_sets`([#3083](https://github.com/aliyun/terraform-provider-alicloud/issues/3083))

IMPROVEMENTS:

- Add flow contral retry for alicloud_cms_site_monitor([#3099](https://github.com/aliyun/terraform-provider-alicloud/issues/3099))
- update ci pipeline([#3098](https://github.com/aliyun/terraform-provider-alicloud/issues/3098))
- datasource/ros: update datasource testcase name.([#3097](https://github.com/aliyun/terraform-provider-alicloud/issues/3097))

BUG FIXES:

- fix create dbinstance type conversion error([#3089](https://github.com/aliyun/terraform-provider-alicloud/issues/3089))

## 1.105.0 (November 28, 2020)

- **New Resource:** `alicloud_fnf_schedule`([#3078](https://github.com/aliyun/terraform-provider-alicloud/issues/3078))
- **New Resource:** `alicloud_fnf_flow`([#3057](https://github.com/aliyun/terraform-provider-alicloud/issues/3057))
- **New Resource:** `alicloud_edas_k8s_application`([#3039](https://github.com/aliyun/terraform-provider-alicloud/issues/3039))
- **Data Source:** `alicloud_fnf_schedules`([#3078](https://github.com/aliyun/terraform-provider-alicloud/issues/3078))
- **Data Source:** `alicloud_fnf_flows`([#3057](https://github.com/aliyun/terraform-provider-alicloud/issues/3057))

IMPROVEMENTS:

- resource/alicloud_cs_kubernetes_node_pool：supports outputing asg id([#3082](https://github.com/aliyun/terraform-provider-alicloud/issues/3082))
- test/alicloud_kvstore_instance_test: Not test upgrade 2.0 to 4.0 for memcache([#3077](https://github.com/aliyun/terraform-provider-alicloud/issues/3077))
- resource/alicloud_ram_role: add attribute max_session_duration([#3074](https://github.com/aliyun/terraform-provider-alicloud/issues/3074))
- Add support to create fnf_flow region for test case and adjust the samplevalue of name in testcase([#3073](https://github.com/aliyun/terraform-provider-alicloud/issues/3073))
- add fnf_flow ci test([#3071](https://github.com/aliyun/terraform-provider-alicloud/issues/3071))
- resource/alicloud_kvstore_instance: Skip test for classic network instance([#3069](https://github.com/aliyun/terraform-provider-alicloud/issues/3069))
- resource/alicloud_kms_secret: Add retry strategy for update and delete([#3068](https://github.com/aliyun/terraform-provider-alicloud/issues/3068))
- resource/mongodb_sharding_instance: add tags argument([#3061](https://github.com/aliyun/terraform-provider-alicloud/issues/3061))
- resource/waf_instance,waf_domain: upgrade to teadsl sdk([#3059](https://github.com/aliyun/terraform-provider-alicloud/issues/3059))
- resource/alicloud_kvstore_instance: Support modify private connection string([#3058](https://github.com/aliyun/terraform-provider-alicloud/issues/3058))
- Update sdk to 1.61.684 and compatible with cms_alarm attribute type([#3055](https://github.com/aliyun/terraform-provider-alicloud/issues/3055))
- add a method to check whether an error is EOF([#3054](https://github.com/aliyun/terraform-provider-alicloud/issues/3054))
- enlarge sdk connect timeout to avoid network error([#3052](https://github.com/aliyun/terraform-provider-alicloud/issues/3052))
- resource/alicloud_db_readwrite_splitting_connection:upgrade resource teadsl sdk([#3051](https://github.com/aliyun/terraform-provider-alicloud/issues/3051))
- update changelog([#3050](https://github.com/aliyun/terraform-provider-alicloud/issues/3050))
- resource/alicloud_hbase_instance: supports more resource attributes([#3035](https://github.com/aliyun/terraform-provider-alicloud/issues/3035))
- make sure LB is active before creating vgroups([#2700](https://github.com/aliyun/terraform-provider-alicloud/issues/2700))

BUG FIXES:

- resource/alicloud_db_instance: fix db eof error([#3081](https://github.com/aliyun/terraform-provider-alicloud/issues/3081))
- fix var name for account type in alicloud_db_account([#3076](https://github.com/aliyun/terraform-provider-alicloud/issues/3076))
- resource/alicloud_instance: fix the period diff error when auto_renew is true([#3072](https://github.com/aliyun/terraform-provider-alicloud/issues/3072))
- fix managedK8s connections return null, Detach the default node pool node and support: certificate_authority([#3070](https://github.com/aliyun/terraform-provider-alicloud/issues/3070))
- resource/alicloud_db_backup_policy: fix InvalidParameters error([#3067](https://github.com/aliyun/terraform-provider-alicloud/issues/3067))
- fix acl update only ingress or egress error([#3064](https://github.com/aliyun/terraform-provider-alicloud/issues/3064))
- fix rds teadsl setting autoretry and add `Post https` error retry([#3053](https://github.com/aliyun/terraform-provider-alicloud/issues/3053))

## 1.104.0 (November 20, 2020)

- **New Resource:** `alicloud_cms_group_metric_rule`([#3044](https://github.com/aliyun/terraform-provider-alicloud/issues/3044))
- **New Resource:** `alicloud_fc_alias`([#3038](https://github.com/aliyun/terraform-provider-alicloud/issues/3038))
- **Data Source:** `alicloud_cms_group_metric_rules`([#3044](https://github.com/aliyun/terraform-provider-alicloud/issues/3044))

IMPROVEMENTS:

- resource/alicloud_kvstore_instance: Add ModifyBackupPolicy for resource and Deprecated alicloud_kvstore_backup_policy([#3049](https://github.com/aliyun/terraform-provider-alicloud/issues/3049))
- Modify NewCommonRequest endpoint loading method([#3047](https://github.com/aliyun/terraform-provider-alicloud/issues/3047))
- supports Finance and Gov region([#3046](https://github.com/aliyun/terraform-provider-alicloud/issues/3046))
- resource/alicloud_db_connection:upgrade teadsl sdk([#3045](https://github.com/aliyun/terraform-provider-alicloud/issues/3045))
- resource/alicloud_db_readonly_instance:upgrade teadsl sdk([#3043](https://github.com/aliyun/terraform-provider-alicloud/issues/3043))
- config/rule: Update config rule attribute and add sweep function for config rule([#3042](https://github.com/aliyun/terraform-provider-alicloud/issues/3042))
- resource/alicloud_db_database:upgrade teadsl sdk([#3040](https://github.com/aliyun/terraform-provider-alicloud/issues/3040))
- resource/alicloud_db_instance:upgrade teadsl sdk([#3036](https://github.com/aliyun/terraform-provider-alicloud/issues/3036))
- resource/alicloud_slb_listener: Supporting new field ca_certificate_id([#3033](https://github.com/aliyun/terraform-provider-alicloud/issues/3033))
- resource/alicloud_db_backup_policy:upgrade teadsl sdk([#3031](https://github.com/aliyun/terraform-provider-alicloud/issues/3031))
- Convert ons_instance to common Api([#3029](https://github.com/aliyun/terraform-provider-alicloud/issues/3029))
- resource/alicloud_db_account_privilege:upgrade to teadsl sdk([#3027](https://github.com/aliyun/terraform-provider-alicloud/issues/3027))
- correct docs provider version from 1.104.0 to 1.103.2([#3026](https://github.com/aliyun/terraform-provider-alicloud/issues/3026))
- resource/alicloud_db_account:adapt to teadsl sdk and support temporary ak([#3025](https://github.com/aliyun/terraform-provider-alicloud/issues/3025))
- update changelog([#3024](https://github.com/aliyun/terraform-provider-alicloud/issues/3024))

BUG FIXES:

- fix:get db readwrite splitting connection([#3032](https://github.com/aliyun/terraform-provider-alicloud/issues/3032))
- Fixed bug of converting charge_tyep to Prepaid([#3028](https://github.com/aliyun/terraform-provider-alicloud/issues/3028))

## 1.103.2 (November 14, 2020)

IMPROVEMENTS:

- resource/alicloud_readonly_instance: Enlarging the createing timeout to 60min([#3023](https://github.com/aliyun/terraform-provider-alicloud/issues/3023))
- TestCase/Cen: Add sweep function for cen_instance_attachemt and cen_route_service([#3022](https://github.com/aliyun/terraform-provider-alicloud/issues/3022))
- resource/alicloud_db_instance: Improve its testcase by adding timeouts for vswitch([#3020](https://github.com/aliyun/terraform-provider-alicloud/issues/3020))
- Updata alibaba-cloud-sdk-go to v1.61.623 and make the drds_instance struct compatible([#3017](https://github.com/aliyun/terraform-provider-alicloud/issues/3017))
- Add asynchronous for kms secret([#3007](https://github.com/aliyun/terraform-provider-alicloud/issues/3007))
- resource/alicloud_pvtz_zone_record: Support setting new attribute remark([#3006](https://github.com/aliyun/terraform-provider-alicloud/issues/3006))
- resource/alicloud_kvstore_instance: Add constant auto_pay for kvstore api ModifyInstanceSpec([#3003](https://github.com/aliyun/terraform-provider-alicloud/issues/3003))
- Cleanup after release 1.103.1([#2997](https://github.com/aliyun/terraform-provider-alicloud/issues/2997))
- update changelog([#2993](https://github.com/aliyun/terraform-provider-alicloud/issues/2993))
- Create cluster parameters aligned with the ACK([#2990](https://github.com/aliyun/terraform-provider-alicloud/issues/2990))

BUG FIXES:

- resource/alicloud_elasticsearch_instance: fix schema details for 'description' and 'zone_count'([#3018](https://github.com/aliyun/terraform-provider-alicloud/issues/3018))

## 1.103.1 (November 06, 2020)

IMPROVEMENTS:

- ci test supports network acl([#2995](https://github.com/aliyun/terraform-provider-alicloud/issues/2995))
- Increase sls retry type([#2992](https://github.com/aliyun/terraform-provider-alicloud/issues/2992))
- Modify the order of updating the interface([#2983](https://github.com/aliyun/terraform-provider-alicloud/issues/2983))
- Modify the way of obtaining Drds instance vpc id([#2981](https://github.com/aliyun/terraform-provider-alicloud/issues/2981))
- update changelog([#2978](https://github.com/aliyun/terraform-provider-alicloud/issues/2978))

BUG FIXES:

- fix(alicloud_eip): delete it failed error([#2996](https://github.com/aliyun/terraform-provider-alicloud/issues/2996))
- fix client bug when loading endpoint([#2994](https://github.com/aliyun/terraform-provider-alicloud/issues/2994))
- fix network acl error([#2986](https://github.com/aliyun/terraform-provider-alicloud/issues/2986))
- fix auto_provisioning_group and reserved_instance set attribute failed bug([#2972](https://github.com/aliyun/terraform-provider-alicloud/issues/2972))

## 1.103.0 (October 30, 2020)

- **New Resource:** `alicloud_cs_edge_kubernetes`([#2871](https://github.com/aliyun/terraform-provider-alicloud/issues/2871))
- **Data Source:** `alicloud_cs_edge_kubernetes_clusters`([#2871](https://github.com/aliyun/terraform-provider-alicloud/issues/2871))

IMPROVEMENTS:

- improve fc service docs([#2975](https://github.com/aliyun/terraform-provider-alicloud/issues/2975))
- improve memcache test case([#2974](https://github.com/aliyun/terraform-provider-alicloud/issues/2974))
- change nat bandwidth pachage to use commonApi instead of sdk([#2971](https://github.com/aliyun/terraform-provider-alicloud/issues/2971))
- Support modify maintain time for kvstore instance and Supplementary documentation for kvstore connection([#2962](https://github.com/aliyun/terraform-provider-alicloud/issues/2962))
- improve(slb) update slb listener scheduler([#2960](https://github.com/aliyun/terraform-provider-alicloud/issues/2960))
- update changelog([#2959](https://github.com/aliyun/terraform-provider-alicloud/issues/2959))
- change sdk to common api([#2958](https://github.com/aliyun/terraform-provider-alicloud/issues/2958))
- add sweep for Resource Manager testcase([#2955](https://github.com/aliyun/terraform-provider-alicloud/issues/2955))

BUG FIXES:

- fix API Gateway App list tags failed([#2973](https://github.com/aliyun/terraform-provider-alicloud/issues/2973))
- fix the managed k8s does not display connections information([#2970](https://github.com/aliyun/terraform-provider-alicloud/issues/2970))
- Fix cdn_domain_config import bug([#2967](https://github.com/aliyun/terraform-provider-alicloud/issues/2967))
- fix(alicloud_kvstore_instance): security_group_id diff error and SSLDisableStateExistsFault error([#2963](https://github.com/aliyun/terraform-provider-alicloud/issues/2963))

## 1.102.0 (October 23, 2020)

- **Data Source:** `alicloud_kvstore_accounts`([#2952](https://github.com/aliyun/terraform-provider-alicloud/issues/2952))
- **Data Source:** `alicloud_enhanced_nat_available_zones`([#2907](https://github.com/aliyun/terraform-provider-alicloud/issues/2907))

IMPROVEMENTS:

- improve ci test by removing debug print([#2954](https://github.com/aliyun/terraform-provider-alicloud/issues/2954))
- improve validation of resource alicloud_polardb_endpoint_address's parameter connection_prefix([#2953](https://github.com/aliyun/terraform-provider-alicloud/issues/2953))
- Resource alicloud_adb_clusters add optional parameter: status and improve validation of resource alicloud_adb_connection's parameter connection_prefix([#2949](https://github.com/aliyun/terraform-provider-alicloud/issues/2949))
- add example usage for RDS Instance([#2945](https://github.com/aliyun/terraform-provider-alicloud/issues/2945))
- Support multiple security_group_id and Set connection_domain as output param([#2943](https://github.com/aliyun/terraform-provider-alicloud/issues/2943))
- support new region cn-guangzhou([#2941](https://github.com/aliyun/terraform-provider-alicloud/issues/2941))
- support datasource for CEN Route Service([#2939](https://github.com/aliyun/terraform-provider-alicloud/issues/2939))
- improve cas certificate testcase([#2936](https://github.com/aliyun/terraform-provider-alicloud/issues/2936))
- applying tea dsl sdk to vpc resource([#2935](https://github.com/aliyun/terraform-provider-alicloud/issues/2935))
- using tea dsl sdk to init client([#2934](https://github.com/aliyun/terraform-provider-alicloud/issues/2934))
- update changelog([#2928](https://github.com/aliyun/terraform-provider-alicloud/issues/2928))
- feat: resource ess_scaling_group suppors new field group_deletion_protection([#2927](https://github.com/aliyun/terraform-provider-alicloud/issues/2927))

BUG FIXES:

- fix(eip_association): TaskConflict error caused by clientToken([#2951](https://github.com/aliyun/terraform-provider-alicloud/issues/2951))
- fix (db_instance): vswitch_id suppress diff error when creating a new one([#2950](https://github.com/aliyun/terraform-provider-alicloud/issues/2950))
- fix config bug when running sweeper test([#2946](https://github.com/aliyun/terraform-provider-alicloud/issues/2946))
- fix maxcompute doc subcategory([#2942](https://github.com/aliyun/terraform-provider-alicloud/issues/2942))
- fix disk, keypair and image random diff bug([#2938](https://github.com/aliyun/terraform-provider-alicloud/issues/2938))
- fix alicloud_security_group tags random diff bug([#2937](https://github.com/aliyun/terraform-provider-alicloud/issues/2937))
- fix the test case of cms_alarm and add errorCode for cms_contact([#2932](https://github.com/aliyun/terraform-provider-alicloud/issues/2932))
- fix document for RDS instance([#2931](https://github.com/aliyun/terraform-provider-alicloud/issues/2931))
- fix oss_bucket document format is not correct([#2930](https://github.com/aliyun/terraform-provider-alicloud/issues/2930))
- fix testcase: replace alicloud_zones with alicloud_kvstore_zones([#2926](https://github.com/aliyun/terraform-provider-alicloud/issues/2926))
- feat: supported to specify slave zones([#2924](https://github.com/aliyun/terraform-provider-alicloud/issues/2924))

## 1.101.0 (October 16, 2020)

- **New Resource:** `alicloud_cms_alarm_contact_group`([#2885](https://github.com/aliyun/terraform-provider-alicloud/issues/2885))
- **New Resource:** `alicloud_kvstore_connection`([#2867](https://github.com/aliyun/terraform-provider-alicloud/issues/2867))
- **Data Source:** `alicloud_cms_alarm_contact_groups`([#2885](https://github.com/aliyun/terraform-provider-alicloud/issues/2885))
- **Data Source:** `alicloud_kvstore_connections`([#2867](https://github.com/aliyun/terraform-provider-alicloud/issues/2867))

IMPROVEMENTS:

- resource_alicloud_instance add system_disk_name and system_disk_description params([#2920](https://github.com/aliyun/terraform-provider-alicloud/issues/2920))
- remove unsupported field resource_group_id from resource cs_kubernetes_node_pool([#2919](https://github.com/aliyun/terraform-provider-alicloud/issues/2919))
- Skip testcase with invalid region for Cloud Config([#2918](https://github.com/aliyun/terraform-provider-alicloud/issues/2918))
- Support service version in FC([#2917](https://github.com/aliyun/terraform-provider-alicloud/issues/2917))
- Correct the alicloud_polardb_cluster and alicloud_polardb_account_privilege's example usage([#2916](https://github.com/aliyun/terraform-provider-alicloud/issues/2916))
- sync vendor using go mod([#2915](https://github.com/aliyun/terraform-provider-alicloud/issues/2915))
- resource alicloud_alikafka_instance supports end_point([#2912](https://github.com/aliyun/terraform-provider-alicloud/issues/2912))
- elasticsearch instance support configuration 'client node' and 'protocol'([#2910](https://github.com/aliyun/terraform-provider-alicloud/issues/2910))
- resource alicloud_polardb_account_privilege supports DMLOnly and DMLOnly and then improve its docs([#2906](https://github.com/aliyun/terraform-provider-alicloud/issues/2906))
- Exclude unsupported regions for dms enterprise([#2903](https://github.com/aliyun/terraform-provider-alicloud/issues/2903))
- update changelog([#2902](https://github.com/aliyun/terraform-provider-alicloud/issues/2902))
- Creating a cluster response increases: cluster_spec([#2898](https://github.com/aliyun/terraform-provider-alicloud/issues/2898))
- alicloud_log_alert: support message center type([#2897](https://github.com/aliyun/terraform-provider-alicloud/issues/2897))
- disable validate disk category on ack cluster([#2886](https://github.com/aliyun/terraform-provider-alicloud/issues/2886))
- added create emr cluster request params validation([#2786](https://github.com/aliyun/terraform-provider-alicloud/issues/2786))

BUG FIXES:

- fix testcase: replace alicloud_zones with alicloud_kvstore_zones([#2925](https://github.com/aliyun/terraform-provider-alicloud/issues/2925))
- fix datasource ids bug([#2911](https://github.com/aliyun/terraform-provider-alicloud/issues/2911))
- bugfix: implement DiffSuppressFunc for chart list of log dashboard and pass required fields on update([#2891](https://github.com/aliyun/terraform-provider-alicloud/issues/2891))

## 1.100.1 (October 13, 2020)

IMPROVEMENTS:

- update go vendors([#2904](https://github.com/aliyun/terraform-provider-alicloud/issues/2904))
- improve cs test cases([#2901](https://github.com/aliyun/terraform-provider-alicloud/issues/2901))
- update sdk v1.61.557([#2900](https://github.com/aliyun/terraform-provider-alicloud/issues/2900))
- improve invoking api by tea dsl conn([#2899](https://github.com/aliyun/terraform-provider-alicloud/issues/2899))
- add valid value Australia for resource cen_bandwidth_package and update vendor([#2896](https://github.com/aliyun/terraform-provider-alicloud/issues/2896))

BUG FIXES:

- Fix edas bug([#2676](https://github.com/aliyun/terraform-provider-alicloud/issues/2676))

## 1.100.0 (October 12, 2020)

- **New Resource:** `alicloud_fc_function_async_invoke_config`([#2873](https://github.com/aliyun/terraform-provider-alicloud/issues/2873))

IMPROVEMENTS:

- add valid value Australia for resource cen_bandwidth_package and update vendor([#2895](https://github.com/aliyun/terraform-provider-alicloud/issues/2895))
- update ci test by adding config([#2894](https://github.com/aliyun/terraform-provider-alicloud/issues/2894))
- Create cluster support ResourceGroup and ACK-Pro([#2889](https://github.com/aliyun/terraform-provider-alicloud/issues/2889))
- update vendor for alikafka([#2883](https://github.com/aliyun/terraform-provider-alicloud/issues/2883))
- resource_manager_policy add validateJsonString and resource_manager_attachment support level 5 id([#2880](https://github.com/aliyun/terraform-provider-alicloud/issues/2880))
- dms user: replace some parameters for compatibility ([#2875](https://github.com/aliyun/terraform-provider-alicloud/issues/2875))
- feature: resource dms_enterprise_instance supports skip_test and deprecated instance_alias ([#2874](https://github.com/aliyun/terraform-provider-alicloud/issues/2874))
- UPDATE CHANGELOG ([#2869](https://github.com/aliyun/terraform-provider-alicloud/issues/2869))

BUG FIXES:

- Revert "Create cluster support ResourceGroup and ACK-Pro"([#2895](https://github.com/aliyun/terraform-provider-alicloud/issues/2895))
- Work around the SLS log project does not exist error([#2893](https://github.com/aliyun/terraform-provider-alicloud/issues/2893))
- bugfix: Upgrade github.com/aliyun/aliyun-log-go-sdk to v0.1.13([#2888](https://github.com/aliyun/terraform-provider-alicloud/issues/2888))

## 1.99.0 (September 28, 2020)

- **New Resource:** `alicloud_cms_alarm_contact`([#2870](https://github.com/aliyun/terraform-provider-alicloud/issues/2870))
- **New Resource:** `alicloud_cen_route_service`([#2868](https://github.com/aliyun/terraform-provider-alicloud/issues/2868))
- **New Resource:** `alicloud_config_delivery_channel`([#2865](https://github.com/aliyun/terraform-provider-alicloud/issues/2865))
- **New Resource:** `alicloud_config_configuration_recorder`([#2863](https://github.com/aliyun/terraform-provider-alicloud/issues/2863))
- **New Resource:** `alicloud_config_rule`([#2858](https://github.com/aliyun/terraform-provider-alicloud/issues/2858))
- **Data Source:** `alicloud_cms_alarm_contacts`([#2870](https://github.com/aliyun/terraform-provider-alicloud/issues/2870))
- **Data Source:** `alicloud_cen_route_services`([#2868](https://github.com/aliyun/terraform-provider-alicloud/issues/2868))
- **Data Source:** `alicloud_config_delivery_channels`([#2865](https://github.com/aliyun/terraform-provider-alicloud/issues/2865))
- **Data Source:** `alicloud_config_configuration_recorders`([#2863](https://github.com/aliyun/terraform-provider-alicloud/issues/2863))
- **Data Source:** `alicloud_config_rules`([#2858](https://github.com/aliyun/terraform-provider-alicloud/issues/2858))

IMPROVEMENTS:

- Use Alidns_domain_attachment instead dns_domain_attachment resource([#2878](https://github.com/aliyun/terraform-provider-alicloud/issues/2878))
- Add enum for 'Lang' attribute of cms_alarm_contact([#2877](https://github.com/aliyun/terraform-provider-alicloud/issues/2877))
- Remove the enum of 'line' attribute in alidns_record([#2872](https://github.com/aliyun/terraform-provider-alicloud/issues/2872))
- update vendor([#2866](https://github.com/aliyun/terraform-provider-alicloud/issues/2866))
- support more regions for alikafka([#2864](https://github.com/aliyun/terraform-provider-alicloud/issues/2864))
- Remove mutli filter conditions from alicloud_hbase_zones and alicloud…([#2862](https://github.com/aliyun/terraform-provider-alicloud/issues/2862))
- update go.sum([#2860](https://github.com/aliyun/terraform-provider-alicloud/issues/2860))
- UPDATE CHANGELOG([#2857](https://github.com/aliyun/terraform-provider-alicloud/issues/2857))

BUG FIXES:

- Fix elasticsearch untagResources failed error([#2876](https://github.com/aliyun/terraform-provider-alicloud/issues/2876))

## 1.98.0 (September 22, 2020)

- **New Resource:** `alicloud_fc_custom_domain`([#2828](https://github.com/aliyun/terraform-provider-alicloud/issues/2828))
- **Data Source:** `alicloud_cen_vbr_health_checks`([#2854](https://github.com/aliyun/terraform-provider-alicloud/issues/2854))
- **Data Source:** `alicloud_edas_services`([#2852](https://github.com/aliyun/terraform-provider-alicloud/issues/2852))
- **Data Source:** `alicloud_cdn_services`([#2850](https://github.com/aliyun/terraform-provider-alicloud/issues/2850))
- **Data Source:** `alicloud_fc_custom_domains`([#2828](https://github.com/aliyun/terraform-provider-alicloud/issues/2828))

IMPROVEMENTS:

- update go.sum([#2850](https://github.com/aliyun/terraform-provider-alicloud/issues/2850))
- feature(alicloud_ram_access_key): support outputting secret when pgp_key is not set([#2856](https://github.com/aliyun/terraform-provider-alicloud/issues/2856))
- feat(alicloud_dcdn_domain): support waiting timeout when updating it([#2855](https://github.com/aliyun/terraform-provider-alicloud/issues/2855))
- Add computed to the resource_group_id attribute of the alidns_domain([#2853](https://github.com/aliyun/terraform-provider-alicloud/issues/2853))
- add DiffSuppressFunc for resource_manager_policy field policy_document to match jsonstring diff([#2851](https://github.com/aliyun/terraform-provider-alicloud/issues/2851))
- improve cen resources' testcase([#2842](https://github.com/aliyun/terraform-provider-alicloud/issues/2842))
- upgrade resource and datasource for CEN Instance([#2840](https://github.com/aliyun/terraform-provider-alicloud/issues/2840))
- Improve resource ons_group and its datasource([#2838](https://github.com/aliyun/terraform-provider-alicloud/issues/2838))
- ram_user_policy_attachment support throttling.user error retry([#2837](https://github.com/aliyun/terraform-provider-alicloud/issues/2837))
- ram_role_policy_attachment support throttling.user error retry([#2835](https://github.com/aliyun/terraform-provider-alicloud/issues/2835))
- Add credit_specification parameter to ess scaling configuration([#2834](https://github.com/aliyun/terraform-provider-alicloud/issues/2834))
- remove the useless package in the go.sum([#2833](https://github.com/aliyun/terraform-provider-alicloud/issues/2833))
- upgrade resource alicloud_cen_bandwidth_package and its datasource([#2832](https://github.com/aliyun/terraform-provider-alicloud/issues/2832))
- UPDATECHANGELOG([#2831](https://github.com/aliyun/terraform-provider-alicloud/issues/2831))

BUG FIXES:

- fix oss endpoint in eu-central-1 issue([#2836](https://github.com/aliyun/terraform-provider-alicloud/issues/2836))

## 1.97.0 (September 18, 2020)

- **New Resource:** `alicloud_cen_instance_attachment`([#2822](https://github.com/aliyun/terraform-provider-alicloud/issues/2822))
- **New Resource:** `alicloud_ons_instance`([#2820](https://github.com/aliyun/terraform-provider-alicloud/issues/2820))
- **New Resource:** `alicloud_cs_node_pool`([#2787](https://github.com/aliyun/terraform-provider-alicloud/issues/2787))
- **Data Source:** `alicloud_cen_instance_attachments`([#2822](https://github.com/aliyun/terraform-provider-alicloud/issues/2822))
- **Data Source:** `alicloud_ons_instances`([#2820](https://github.com/aliyun/terraform-provider-alicloud/issues/2820))
- **Data Source:** `alicloud_nas_services`([#2813](https://github.com/aliyun/terraform-provider-alicloud/issues/2813))
- **Data Source:** `alicloud_oss_services`([#2812](https://github.com/aliyun/terraform-provider-alicloud/issues/2812))
- **Data Source:** `alicloud_ots_services`([#2807](https://github.com/aliyun/terraform-provider-alicloud/issues/2807))

IMPROVEMENTS:

- Compatible domain_group_name for alidns_domain_group([#2830](https://github.com/aliyun/terraform-provider-alicloud/issues/2830))
- Add errorcode for DeleteDomain api([#2829](https://github.com/aliyun/terraform-provider-alicloud/issues/2829))
- remove datasource alicloud_edas_application useless output([#2826](https://github.com/aliyun/terraform-provider-alicloud/issues/2826))
- add missing pull request([#2825](https://github.com/aliyun/terraform-provider-alicloud/issues/2825))
- improve resource ons_topic and its datasource([#2823](https://github.com/aliyun/terraform-provider-alicloud/issues/2823))
- update sdk v1.61.497([#2818](https://github.com/aliyun/terraform-provider-alicloud/issues/2818))
- resource alicloud_cen_instance_attachment docs and testcase support child_instance_type([#2817](https://github.com/aliyun/terraform-provider-alicloud/issues/2817))
- Adjust the document for Alidns([#2808](https://github.com/aliyun/terraform-provider-alicloud/issues/2808))
- Add waiting method for update scope([#2802](https://github.com/aliyun/terraform-provider-alicloud/issues/2802))
- UPDATE CHANGELOG([#2800](https://github.com/aliyun/terraform-provider-alicloud/issues/2800))
- improve(slb) update slb docs rules server_groups slbs([#2728](https://github.com/aliyun/terraform-provider-alicloud/issues/2728))
- Rewrote resource page to correct name([#2580](https://github.com/aliyun/terraform-provider-alicloud/issues/2580))
- datasource snapshots supports outputting tags([#2545](https://github.com/aliyun/terraform-provider-alicloud/issues/2545))

BUG FIXES:

- fix resource alicloud_api_gateway_api ConcurrencyLockTimeout error([#2827](https://github.com/aliyun/terraform-provider-alicloud/issues/2827))
- fix elasticsearch_instance return redundant tags issue([#2821](https://github.com/aliyun/terraform-provider-alicloud/issues/2821))
- fix cms testcase([#2819](https://github.com/aliyun/terraform-provider-alicloud/issues/2819))
- fix adb cluster testcase([#2816](https://github.com/aliyun/terraform-provider-alicloud/issues/2816))
- fix log.Fatal bug when using tea client([#2814](https://github.com/aliyun/terraform-provider-alicloud/issues/2814))
- fix getting oss endpoint bug([#2811](https://github.com/aliyun/terraform-provider-alicloud/issues/2811))
- fix elasticsearch_instance return redundant tags issue([#2810](https://github.com/aliyun/terraform-provider-alicloud/issues/2810))
- fix: db instance delay set is 30s([#2780](https://github.com/aliyun/terraform-provider-alicloud/issues/2780))
- fix_auto_provisioning_group([#2552](https://github.com/aliyun/terraform-provider-alicloud/issues/2552))

## 1.96.0 (September 13, 2020)

- **Data Source:** `alicloud_log_service`([#2804](https://github.com/aliyun/terraform-provider-alicloud/issues/2804))
- **Data Source:** `alicloud_api_gateway_service`([#2801](https://github.com/aliyun/terraform-provider-alicloud/issues/2801))

IMPROVEMENTS:

- improve resource alicloud_ess_scaling_rule docs([#2795](https://github.com/aliyun/terraform-provider-alicloud/issues/2795))
- Add retry and wait for cms api EnableMetricRules DisableMetricRules([#2794](https://github.com/aliyun/terraform-provider-alicloud/issues/2794))
- Add wait and retry for flow control([#2793](https://github.com/aliyun/terraform-provider-alicloud/issues/2793))
- PolarDB cluster support setting resource_group_id([#2792](https://github.com/aliyun/terraform-provider-alicloud/issues/2792))
- Support FC new features: custom container, new instance type and NAS integration([#2791](https://github.com/aliyun/terraform-provider-alicloud/issues/2791))
- update action trail docs subcategory([#2788](https://github.com/aliyun/terraform-provider-alicloud/issues/2788))
- UPDATE CHANGELOG([#2774](https://github.com/aliyun/terraform-provider-alicloud/issues/2774))

BUG FIXES:

- cms resource suppots assume role([#2803](https://github.com/aliyun/terraform-provider-alicloud/issues/2803))
- fix dcdn_domain the input parameter form of the scope attribute([#2797](https://github.com/aliyun/terraform-provider-alicloud/issues/2797))
- fix redis allocate public network([#2796](https://github.com/aliyun/terraform-provider-alicloud/issues/2796))

## 1.95.0 (September 03, 2020)

- **New Resource:** `alicloud_actiontrail_trail`([#2758](https://github.com/aliyun/terraform-provider-alicloud/issues/2758))
- **Data Source:** `alicloud_actiontrail_trails`([#2758](https://github.com/aliyun/terraform-provider-alicloud/issues/2758))

IMPROVEMENTS:

- remove the useless files in archives([#2784](https://github.com/aliyun/terraform-provider-alicloud/issues/2784))
- resource alicloud_disk supports setting performance_level([#2783](https://github.com/aliyun/terraform-provider-alicloud/issues/2783))
- add more ci test flag([#2782](https://github.com/aliyun/terraform-provider-alicloud/issues/2782))
- dns_instance and dns_domain renamed to alidns_instance, alidns_domain([#2776](https://github.com/aliyun/terraform-provider-alicloud/issues/2776))
- add force Unassociate for eip([#2772](https://github.com/aliyun/terraform-provider-alicloud/issues/2772))
- improve(alicloud_images): supports more filters([#2771](https://github.com/aliyun/terraform-provider-alicloud/issues/2771))
- Adjust the datasource testcase name([#2762](https://github.com/aliyun/terraform-provider-alicloud/issues/2762))
- upgrade resource and datasource for NAS MountTarget([#2759](https://github.com/aliyun/terraform-provider-alicloud/issues/2759))
- update resource markdown grammar([#2757](https://github.com/aliyun/terraform-provider-alicloud/issues/2757))
- upgrade datasource for NAS AccessGroup([#2746](https://github.com/aliyun/terraform-provider-alicloud/issues/2746))
- PolarDB support add or remove read-only nodes([#2745](https://github.com/aliyun/terraform-provider-alicloud/issues/2745))
- UPDATE CHANGELOG([#2731](https://github.com/aliyun/terraform-provider-alicloud/issues/2731))
- improve(slb) update docs([#2719](https://github.com/aliyun/terraform-provider-alicloud/issues/2719))

BUG FIXES:

- Fix the managed_kubernetes docs([#2785](https://github.com/aliyun/terraform-provider-alicloud/issues/2785))
- fix document of Hbase and Bastionhost([#2777](https://github.com/aliyun/terraform-provider-alicloud/issues/2777))
- fix dcdn_domain sources parameter for update method([#2773](https://github.com/aliyun/terraform-provider-alicloud/issues/2773))
- Fix cdn test case([#2760](https://github.com/aliyun/terraform-provider-alicloud/issues/2760))

## 1.94.0 (August 24, 2020)

- **New Resource:** `alicloud_dcdn_domain`([#2744](https://github.com/aliyun/terraform-provider-alicloud/issues/2744))
- **New Resource:** `alicloud_mse_cluster`([#2733](https://github.com/aliyun/terraform-provider-alicloud/issues/2733))
- **New Resource:** `alicloud_resource_manager_policy_attachment`([#2696](https://github.com/aliyun/terraform-provider-alicloud/issues/2696))
- **Data Source:** `alicloud_dcdn_domains`([#2744](https://github.com/aliyun/terraform-provider-alicloud/issues/2744))
- **Data Source:** `alicloud_mse_clusters`([#2733](https://github.com/aliyun/terraform-provider-alicloud/issues/2733))
- **Data Source:** `alicloud_resource_manager_policy_attachments`([#2696](https://github.com/aliyun/terraform-provider-alicloud/issues/2696))

IMPROVEMENTS:

- Support allocate and release public connection for redis([#2748](https://github.com/aliyun/terraform-provider-alicloud/issues/2748))
- Support to set warn and info level alarm([#2743](https://github.com/aliyun/terraform-provider-alicloud/issues/2743))
- waf domain support setting resource_group_id and more attributes([#2740](https://github.com/aliyun/terraform-provider-alicloud/issues/2740))
- resource dnat supports "import" feature([#2735](https://github.com/aliyun/terraform-provider-alicloud/issues/2735))
- Add func sweep and Change testcase frequency([#2726](https://github.com/aliyun/terraform-provider-alicloud/issues/2726))
- Correct provider docs order([#2723](https://github.com/aliyun/terraform-provider-alicloud/issues/2723))
- Remove github.com/hashicorp/terraform import and use terraform-plugin-sdk instead([#2722](https://github.com/aliyun/terraform-provider-alicloud/issues/2722))
- Add test sweep for eci_image_cache([#2720](https://github.com/aliyun/terraform-provider-alicloud/issues/2720))
- modify alicloud_cen_instance_attachment([#2714](https://github.com/aliyun/terraform-provider-alicloud/issues/2714))

BUG FIXES:

- fix the bug of create emr kafka cluster error([#2754](https://github.com/aliyun/terraform-provider-alicloud/issues/2754))
- fix common bandwidth package idempotent issue when Adding and Removeing instance([#2750](https://github.com/aliyun/terraform-provider-alicloud/issues/2750))
- fix website document error using `terraform` tag([#2749](https://github.com/aliyun/terraform-provider-alicloud/issues/2749))
- Fix registry rendering of page([#2747](https://github.com/aliyun/terraform-provider-alicloud/issues/2747))
- fix ci test website-test error([#2742](https://github.com/aliyun/terraform-provider-alicloud/issues/2742))
- fix datasource for ResourceManager for Policy Attachment([#2730](https://github.com/aliyun/terraform-provider-alicloud/issues/2730))
- fix_ecs_snapshot([#2709](https://github.com/aliyun/terraform-provider-alicloud/issues/2709))

## 1.93.0 (August 12, 2020)

- **New Resource:** `alicloud_oos_execution`([#2679](https://github.com/aliyun/terraform-provider-alicloud/issues/2679))
- **New Resource:** `alicloud_edas_k8s_cluster`([#2678](https://github.com/aliyun/terraform-provider-alicloud/issues/2678))
- **Data Source:** `alicloud_oos_execution`([#2679](https://github.com/aliyun/terraform-provider-alicloud/issues/2679))

IMPROVEMENTS:

- Add sweep func for adb cluster test([#2716](https://github.com/aliyun/terraform-provider-alicloud/issues/2716))
- Add default vpc for drds([#2713](https://github.com/aliyun/terraform-provider-alicloud/issues/2713))
- ADB MySQL output output connection string after creation([#2699](https://github.com/aliyun/terraform-provider-alicloud/issues/2699))
- add .goreleaser.yml([#2698](https://github.com/aliyun/terraform-provider-alicloud/issues/2698))
- transfer terraform-provider-alicloud to aliyun from terraform-providers([#2697](https://github.com/aliyun/terraform-provider-alicloud/issues/2697))
- Add purge cluster api for cassandra sweeper([#2693](https://github.com/aliyun/terraform-provider-alicloud/issues/2693))
- Add default vpc for mongodb([#2689](https://github.com/aliyun/terraform-provider-alicloud/issues/2689))
- Add default vpc for kvstore([#2688](https://github.com/aliyun/terraform-provider-alicloud/issues/2688))
- Add sweeper for cassandra cluster([#2687](https://github.com/aliyun/terraform-provider-alicloud/issues/2687))
- Support 'resoruce_group_id' attribute for ImportKeyPair([#2683](https://github.com/aliyun/terraform-provider-alicloud/issues/2683))
- Support to get NotFound error in read method([#2682](https://github.com/aliyun/terraform-provider-alicloud/issues/2682))
- UPDATE CHANGELOG([#2681](https://github.com/aliyun/terraform-provider-alicloud/issues/2681))
- Support specify security group when create instance([#2680](https://github.com/aliyun/terraform-provider-alicloud/issues/2680))
- improve(slb) update slb_backend_server add parameter server_ip([#2651](https://github.com/aliyun/terraform-provider-alicloud/issues/2651))

BUG FIXES:

- update: fix dnat query errror by only use forwardTableId([#2712](https://github.com/aliyun/terraform-provider-alicloud/issues/2712))
- fix: create rds sql_collector_status bug([#2690](https://github.com/aliyun/terraform-provider-alicloud/issues/2690))
- fix(edas): improve sweeper test([#2686](https://github.com/aliyun/terraform-provider-alicloud/issues/2686))
- fix cassandra doc and add describe not found error([#2685](https://github.com/aliyun/terraform-provider-alicloud/issues/2685))
- fix doc: attach AliyunMNSNotificationRolePolicy to role([#2572](https://github.com/aliyun/terraform-provider-alicloud/issues/2572))
- docs: fix typos and grammar in Alicloud Provider([#2559](https://github.com/aliyun/terraform-provider-alicloud/issues/2559))
- fix_markdown_auto_provisioning_group([#2543](https://github.com/aliyun/terraform-provider-alicloud/issues/2543))
- fix_markdown_snapshot_policy([#2540](https://github.com/aliyun/terraform-provider-alicloud/issues/2540))

## 1.92.0 (July 31, 2020)

- **New Resource:** `alicloud_oos_template`([#2670](https://github.com/aliyun/terraform-provider-alicloud/issues/2670))
- **Data Source:** `alicloud_oos_template`([#2670](https://github.com/aliyun/terraform-provider-alicloud/issues/2670))

IMPROVEMENTS:

- modify alicloud_cen_bandwidth_package_attachment([#2675](https://github.com/aliyun/terraform-provider-alicloud/issues/2675))
- UPDATE CHANGELOG([#2671](https://github.com/aliyun/terraform-provider-alicloud/issues/2671))
- upgrade resource of Nas AccessGroup([#2667](https://github.com/aliyun/terraform-provider-alicloud/issues/2667))
- Supports setting the kms id for oss bucket([#2662](https://github.com/aliyun/terraform-provider-alicloud/issues/2662))
- Support service_account_issuer and api_audiences in alicloud_cs_kubernetes and alicloud_cs_managed_kubernetes([#2573](https://github.com/aliyun/terraform-provider-alicloud/issues/2573))

BUG FIXES:

- Fix ess kms disk([#2668](https://github.com/aliyun/terraform-provider-alicloud/issues/2668))

## 1.91.0 (July 24, 2020)

- **New Resource:** `alicloud_ecs_dedicated_host`([#2652](https://github.com/aliyun/terraform-provider-alicloud/issues/2652))
- **Data Source:** `alicloud_ecs_dedicated_hosts`([#2652](https://github.com/aliyun/terraform-provider-alicloud/issues/2652))

IMPROVEMENTS:

- improve test case name([#2672](https://github.com/aliyun/terraform-provider-alicloud/issues/2672))
- update: add nat bound eip ipaddress([#2669](https://github.com/aliyun/terraform-provider-alicloud/issues/2669))
- correct log alert testcase name([#2663](https://github.com/aliyun/terraform-provider-alicloud/issues/2663))
- add example module for OSS bucket([#2661](https://github.com/aliyun/terraform-provider-alicloud/issues/2661))
- cs cluster support data disks([#2657](https://github.com/aliyun/terraform-provider-alicloud/issues/2657))
- drds support international site([#2654](https://github.com/aliyun/terraform-provider-alicloud/issues/2654))
- UPDATE CHANGELOG([#2649](https://github.com/aliyun/terraform-provider-alicloud/issues/2649))
- modify cen_instance([#2644](https://github.com/aliyun/terraform-provider-alicloud/issues/2644))
- add ability to enable ZRS on bucket creation([#2605](https://github.com/aliyun/terraform-provider-alicloud/issues/2605))

BUG FIXES:

- fix ddh testcase([#2665](https://github.com/aliyun/terraform-provider-alicloud/issues/2665))
- fix dms instance([#2656](https://github.com/aliyun/terraform-provider-alicloud/issues/2656))
- fix_markdown_ess_scheduled_task([#2655](https://github.com/aliyun/terraform-provider-alicloud/issues/2655))
- fix slb_listener creates NewCommonRequest error handling([#2653](https://github.com/aliyun/terraform-provider-alicloud/issues/2653))

## 1.90.1 (July 15, 2020)

IMPROVEMENTS:

- perf: rds ssl and tde limitation([#2645](https://github.com/aliyun/terraform-provider-alicloud/issues/2645))
- add isp support to cbwp([#2642](https://github.com/aliyun/terraform-provider-alicloud/issues/2642))
- Remove the resource_group_id parameter when querying the system disk([#2641](https://github.com/aliyun/terraform-provider-alicloud/issues/2641))
- Add 'testAcc' prefix for test case name([#2636](https://github.com/aliyun/terraform-provider-alicloud/issues/2636))
- Support DescribeInstanceSystemDisk method return the error message([#2635](https://github.com/aliyun/terraform-provider-alicloud/issues/2635))
- UPDATE CHANGELOG([#2634](https://github.com/aliyun/terraform-provider-alicloud/issues/2634))

BUG FIXES:

- fix cassandra doc ([#2648](https://github.com/aliyun/terraform-provider-alicloud/issues/2648))
- fix_markdown_ess_scheduled_task([#2647](https://github.com/aliyun/terraform-provider-alicloud/issues/2647))
- fix WAF instance testcase([#2640](https://github.com/aliyun/terraform-provider-alicloud/issues/2640))
- fix testcase name([#2638](https://github.com/aliyun/terraform-provider-alicloud/issues/2638))
- fix_instance([#2632](https://github.com/aliyun/terraform-provider-alicloud/issues/2632))

## 1.90.0 (July 10, 2020)

- **New Resource:** `alicloud_container_registry_enterprise_sync_rule`([#2607](https://github.com/aliyun/terraform-provider-alicloud/issues/2607))
- **New Resource:** `alicloud_dms_user`([#2604](https://github.com/aliyun/terraform-provider-alicloud/issues/2604))
- **Data Source:** `alicloud_cr_ee_sync_rules`([#2630](https://github.com/aliyun/terraform-provider-alicloud/issues/2630))
- **Data Source:** `alicloud_eci_image_cache`([#2627](https://github.com/aliyun/terraform-provider-alicloud/issues/2627))
- **Data Source:** `alicloud_waf_instance`([#2617](https://github.com/aliyun/terraform-provider-alicloud/issues/2617))
- **Data Source:** `alicloud_dms_user`([#2604](https://github.com/aliyun/terraform-provider-alicloud/issues/2604))

IMPROVEMENTS:

- support the CNAME of CDN domain new([#2622](https://github.com/aliyun/terraform-provider-alicloud/issues/2622))
- UPDATE CHANGELOG([#2594](https://github.com/aliyun/terraform-provider-alicloud/issues/2594))
- Feature/disable addon([#2590](https://github.com/aliyun/terraform-provider-alicloud/issues/2590))
- set system default and make fmt([#2480](https://github.com/aliyun/terraform-provider-alicloud/issues/2480))

BUG FIXES:

- fix_ess_scheduled_task([#2628](https://github.com/aliyun/terraform-provider-alicloud/issues/2628))
- fix testcase of WAF instance datasource([#2625](https://github.com/aliyun/terraform-provider-alicloud/issues/2625))
- fix oss lifecycle rule match the whole bucket by default([#2621](https://github.com/aliyun/terraform-provider-alicloud/issues/2621))
- fix ack uat([#2618](https://github.com/aliyun/terraform-provider-alicloud/issues/2618))

## 1.89.0 (July 03, 2020)

- **New Resource:** `alicloud_eci_image_cache`([#2615](https://github.com/aliyun/terraform-provider-alicloud/issues/2615))

IMPROVEMENTS:

- improve(alikafka): using default vswitch to run alikafka testcases([#2591](https://github.com/aliyun/terraform-provider-alicloud/issues/2591))
- run 'go mod vendor' to sync([#2587](https://github.com/aliyun/terraform-provider-alicloud/issues/2587))
- update waf SDK([#2616](https://github.com/aliyun/terraform-provider-alicloud/issues/2616))
- umodify cen_route_map([#2606](https://github.com/aliyun/terraform-provider-alicloud/issues/2606))
- modify cen_bandwidth_package([#2603](https://github.com/aliyun/terraform-provider-alicloud/issues/2603))
- support region cn-wulanchabu([#2599](https://github.com/aliyun/terraform-provider-alicloud/issues/2599))
- Add version_stage filter([#2597](https://github.com/aliyun/terraform-provider-alicloud/issues/2597))
- support releasing ddoscoo instance([#2595](https://github.com/aliyun/terraform-provider-alicloud/issues/2595))
- Support modify system_disk_size online([#2593](https://github.com/aliyun/terraform-provider-alicloud/issues/2593))
- Changelog([#2584](https://github.com/aliyun/terraform-provider-alicloud/issues/2584))

BUG FIXES:

- fix cms site monitor document([#2614](https://github.com/aliyun/terraform-provider-alicloud/issues/2614))
- fix_kms_ecs_disk([#2613](https://github.com/aliyun/terraform-provider-alicloud/issues/2613))
- fix_markdown_ess_notification([#2598](https://github.com/aliyun/terraform-provider-alicloud/issues/2598))
- fix kms secret, secret version doc([#2596](https://github.com/aliyun/terraform-provider-alicloud/issues/2596))
- fix testcase for pvtz_zone([#2592](https://github.com/aliyun/terraform-provider-alicloud/issues/2592))
- fix the dns_record test case bug([#2588](https://github.com/aliyun/terraform-provider-alicloud/issues/2588))
- fix_markdown_launch_template([#2541](https://github.com/aliyun/terraform-provider-alicloud/issues/2541))

## 1.88.0 (June 22, 2020)

- **New Resource:** `alicloud_cen_vbr_health_check`([#2575](https://github.com/aliyun/terraform-provider-alicloud/issues/2575))
- **Data Source:** `alicloud_cen_private_zones`([#2564](https://github.com/aliyun/terraform-provider-alicloud/issues/2564))
- **Data Source:** `alicloud_dms_enterprise_instances`([#2557](https://github.com/aliyun/terraform-provider-alicloud/issues/2557))
- **Data Source:** `alicloud_cassandra`([#2574](https://github.com/aliyun/terraform-provider-alicloud/issues/2574))
- **Data Source:** `alicloud_kms_secret_versions`([#2583](https://github.com/aliyun/terraform-provider-alicloud/issues/2583))

IMPROVEMENTS:

- skip instance prepaid testcase([#2585](https://github.com/aliyun/terraform-provider-alicloud/issues/2585))
- Support setting NO_PROXY and upgrade go sdk([#2581](https://github.com/aliyun/terraform-provider-alicloud/issues/2581))
- Features/atoscaler_use_worker_token([#2578](https://github.com/aliyun/terraform-provider-alicloud/issues/2578))
- Features/knock autoscaler off nodes([#2571](https://github.com/aliyun/terraform-provider-alicloud/issues/2571))
- modify cen_instance_attachment([#2566](https://github.com/aliyun/terraform-provider-alicloud/issues/2566))
- gpdb doc change "tf-gpdb-test"" to "tf-gpdb-test"([#2561](https://github.com/aliyun/terraform-provider-alicloud/issues/2561))
- UPDATE CHANGELOG([#2555](https://github.com/aliyun/terraform-provider-alicloud/issues/2555))
- cassandra cluster([#2522](https://github.com/aliyun/terraform-provider-alicloud/issues/2522))

BUG FIXES:

- Fix the fc-function testcase and markdown([#2569](https://github.com/aliyun/terraform-provider-alicloud/issues/2569))
- fix name spelling mistake([#2558](https://github.com/aliyun/terraform-provider-alicloud/issues/2558))

## 1.87.0 (June 12, 2020)

- **Data Source:** `alicloud_container_registry_enterprise_repos`([#2538](https://github.com/aliyun/terraform-provider-alicloud/issues/2538))
- **Data Source:** `alicloud_container_registry_enterprise_namespaces`([#2530](https://github.com/aliyun/terraform-provider-alicloud/issues/2530))
- **Data Source:** `alicloud_container_registry_enterprise_instances`([#2526](https://github.com/aliyun/terraform-provider-alicloud/issues/2526))
- **Data Source:** `alicloud_cen_route_maps`([#2554](https://github.com/aliyun/terraform-provider-alicloud/issues/2554))

IMPROVEMENTS:

- adapter schedulerrule([#2537](https://github.com/aliyun/terraform-provider-alicloud/issues/2537))
- UPDATE CHANGELOG([#2535](https://github.com/aliyun/terraform-provider-alicloud/issues/2535))
- improve_user_experience([#2491](https://github.com/aliyun/terraform-provider-alicloud/issues/2491))
- add testcase([#2556](https://github.com/aliyun/terraform-provider-alicloud/issues/2556))
- improve(elasticsearch): resource support to open or close network, and modify the kibana whitelist in private network([#2548](https://github.com/aliyun/terraform-provider-alicloud/issues/2548))
- support "resource_group_id" for Bastionhost Instance([#2544](https://github.com/aliyun/terraform-provider-alicloud/issues/2544))
- support "resource_group_id" for DBaudit Instance([#2539](https://github.com/aliyun/terraform-provider-alicloud/issues/2539))
- Automatically generate dns_domain datasource([#2549](https://github.com/aliyun/terraform-provider-alicloud/issues/2549))

BUG FIXES:

- Fix image export([#2542](https://github.com/aliyun/terraform-provider-alicloud/issues/2542))
- fix: perf create rds pg([#2533](https://github.com/aliyun/terraform-provider-alicloud/issues/2533))
- fix_markdown_ess_scalinggroup([#2529](https://github.com/aliyun/terraform-provider-alicloud/issues/2529))
- fix_markdown_image_import([#2520](https://github.com/aliyun/terraform-provider-alicloud/issues/2520))
- fix_markdown_disk([#2504](https://github.com/aliyun/terraform-provider-alicloud/issues/2504))
- fix_markdown_image_s([#2546](https://github.com/aliyun/terraform-provider-alicloud/issues/2546))

## 1.86.0 (June 05, 2020)

- **New Resource:** `alicloud_container_registry_enterprise_repo`([#2525](https://github.com/aliyun/terraform-provider-alicloud/issues/2525))
- **New Resource:** `alicloud_Container_registry_enterprise_namespace`([#2519](https://github.com/aliyun/terraform-provider-alicloud/issues/2519))
- **New Resource:** `alicloud_ddoscoo_scheduler_rule`([#2476](https://github.com/aliyun/terraform-provider-alicloud/issues/2476))
- **New Resource:** `alicloud_resource_manager_policies`([#2474](https://github.com/aliyun/terraform-provider-alicloud/issues/2474))
- **Data Source:** `alicloud_waf_domains`([#2498](https://github.com/aliyun/terraform-provider-alicloud/issues/2498))
- **Data Source:** `alicloud_kms_secrets`([#2515](https://github.com/aliyun/terraform-provider-alicloud/issues/2515))
- **Data Source:** `alicloud_alidns_domain_records`([#2503](https://github.com/aliyun/terraform-provider-alicloud/issues/2503))
- **Data Source:** `alicloud_resource_manager_resource_directories`([#2499](https://github.com/aliyun/terraform-provider-alicloud/issues/2499))
- **Data Source:** `alicloud_resource_manager_handshakes`([#2489](https://github.com/aliyun/terraform-provider-alicloud/issues/2489))
- **Data Source:** `alicloud_resource_manager_accounts`([#2488](https://github.com/aliyun/terraform-provider-alicloud/issues/2488))
- **Data Source:** `alicloud_resource_manager_roles`([#2483](https://github.com/aliyun/terraform-provider-alicloud/issues/2483))

IMPROVEMENTS:
- support "resource_group_id" for Elasticsearch instance([#2528](https://github.com/aliyun/terraform-provider-alicloud/issues/2528))
- Added new feature of encrypting data node disk([#2521](https://github.com/aliyun/terraform-provider-alicloud/issues/2521))
- support "resource_group_id" for Private Zone([#2518](https://github.com/aliyun/terraform-provider-alicloud/issues/2518))
- support "resource_group_id" for DB instance([#2514](https://github.com/aliyun/terraform-provider-alicloud/issues/2514))
- 更新sdk到v1.61.230([#2510](https://github.com/aliyun/terraform-provider-alicloud/issues/2510))
- support "resource_group_id" for kvstore instance([#2509](https://github.com/aliyun/terraform-provider-alicloud/issues/2509))
- Add Log Dashboard([#2502](https://github.com/aliyun/terraform-provider-alicloud/issues/2502))
- UPDATE CHANGELOG([#2497](https://github.com/aliyun/terraform-provider-alicloud/issues/2497))
- Control the instance start and stop through the status attribute([#2464](https://github.com/aliyun/terraform-provider-alicloud/issues/2464))

BUG FIXES:
- fix_markdown_image_import([#2516](https://github.com/aliyun/terraform-provider-alicloud/issues/2516))
- fix ecs 'status' attribute bug([#2512](https://github.com/aliyun/terraform-provider-alicloud/issues/2512))
- fix_markdown_ess_scalinggroup_vserver_groups([#2508](https://github.com/aliyun/terraform-provider-alicloud/issues/2508))
- fix_markdown_disk_attachment([#2501](https://github.com/aliyun/terraform-provider-alicloud/issues/2501))
- fix_markdown_disk_attachment([#2481](https://github.com/aliyun/terraform-provider-alicloud/issues/2481))

## 1.85.0 (May 29, 2020)

- **New Resource:** `alicloud_alidns_record`([#2495](https://github.com/aliyun/terraform-provider-alicloud/issues/2495))
- **New Resource:** `alicloud_kms_key`([#2444](https://github.com/aliyun/terraform-provider-alicloud/issues/2444))
- **New Resource:** `alicloud_kms_keyversion`([#2471](https://github.com/aliyun/terraform-provider-alicloud/issues/2471))
- **Data Source:** `alicloud_resource_manager_policy_versions`([#2496](https://github.com/aliyun/terraform-provider-alicloud/issues/2496))
- **Data Source:** `alicloud_kms_key_versions`([#2494](https://github.com/aliyun/terraform-provider-alicloud/issues/2494))
- **Data Source:** `alicloud_alidns_domain_group`([#2482](https://github.com/aliyun/terraform-provider-alicloud/issues/2482))

IMPROVEMENTS:

- 增加cdn_config删除错误码([#2490](https://github.com/aliyun/terraform-provider-alicloud/issues/2490))
- UPDATE CHANGELOG.md([#2477](https://github.com/aliyun/terraform-provider-alicloud/issues/2477))
- Alicloud edas docs modify([#2473](https://github.com/aliyun/terraform-provider-alicloud/issues/2473))

BUG FIXES:

- fix_markdown_reserved_instance([#2478](https://github.com/aliyun/terraform-provider-alicloud/issues/2478))
- fix_markdown_network_interfaces([#2475](https://github.com/aliyun/terraform-provider-alicloud/issues/2475))
- fix_apg([#2472](https://github.com/aliyun/terraform-provider-alicloud/issues/2472))

## 1.84.0 (May 22, 2020)

- **New Resource:** `alicloud_alidns_domain_group.`([#2454](https://github.com/aliyun/terraform-provider-alicloud/issues/2454))
- **New Resource:** `alicloud_resource_manager_resource_directory`([#2459](https://github.com/aliyun/terraform-provider-alicloud/issues/2459))
- **New Resource:** `alicloud_resource_manager_policy_version`([#2457](https://github.com/aliyun/terraform-provider-alicloud/issues/2457))
- **Data Source:** `alicloud_resource_manager_folders`([#2467](https://github.com/aliyun/terraform-provider-alicloud/issues/2467))
- **Data Source:** `alicloud_alidns_instance.`([#2468](https://github.com/aliyun/terraform-provider-alicloud/issues/2468))
- **Data Source:** `alicloud_resource_manager_resource_groups`([#2462](https://github.com/aliyun/terraform-provider-alicloud/issues/2462))

IMPROVEMENTS:

- Update CHANGELOG.md([#2455](https://github.com/aliyun/terraform-provider-alicloud/issues/2455))

BUG FIXES:

- fix autoscaler configmap update([#2377](https://github.com/aliyun/terraform-provider-alicloud/issues/2377))
- fix eip association failed cause by snat entry's snat_ip update bug([#2440](https://github.com/aliyun/terraform-provider-alicloud/issues/2440))
- fix_tag_validation([#2445](https://github.com/aliyun/terraform-provider-alicloud/issues/2445))
- fix polardb connection string output bug([#2453](https://github.com/aliyun/terraform-provider-alicloud/issues/2453))
- fix the bug of TestAccAlicloudEmrCluster_local_storage nodeCount less…([#2458](https://github.com/aliyun/terraform-provider-alicloud/issues/2458))
- fix_markdown_key_pair_attachment([#2460](https://github.com/aliyun/terraform-provider-alicloud/issues/2460))
- fix_finger_print([#2463](https://github.com/aliyun/terraform-provider-alicloud/issues/2463))
- fix_markdown_instance_type_families([#2465](https://github.com/aliyun/terraform-provider-alicloud/issues/2465))
- fix_markdown_alicloud_network_interface_attachment([#2469](https://github.com/aliyun/terraform-provider-alicloud/issues/2469))

## 1.83.0 (May 15, 2020)

- **New Resource:** `alicloud_waf_instance`([#2456](https://github.com/aliyun/terraform-provider-alicloud/issues/2456))
- **New Resource:** `alicloud_resource_manager_account`([#2441](https://github.com/aliyun/terraform-provider-alicloud/issues/2441))
- **New Resource:** `alicloud_resource_manager_policy`([#2439](https://github.com/aliyun/terraform-provider-alicloud/issues/2439))
- **New Resource:** `alicloud_resource_manager_handshake`([#2432](https://github.com/aliyun/terraform-provider-alicloud/issues/2432))
- **New Resource:** `alicloud_cen_private_zone`([#2421](https://github.com/aliyun/terraform-provider-alicloud/issues/2421))

BUG FIXES:

- fix_markdown_instance([#2436](https://github.com/aliyun/terraform-provider-alicloud/issues/2436))

## 1.82.0 (May 08, 2020)

- **New Resource:** `alicloud_resource_manager_handshake`([#2425](https://github.com/aliyun/terraform-provider-alicloud/issues/2425))
- **New Resource:** `alicloud_resource_manager_folder`([#2425](https://github.com/aliyun/terraform-provider-alicloud/issues/2425))
- **New Resource:** `alicloud_resource_manager_resource_group`([#2422](https://github.com/aliyun/terraform-provider-alicloud/issues/2422))
- **New Resource:** `alicloud_waf_domain`([#2414](https://github.com/aliyun/terraform-provider-alicloud/issues/2414))
- **New Resource:** `alicloud_resource_manager_role`([#2405](https://github.com/aliyun/terraform-provider-alicloud/issues/2405))
- **New Resource:** `alicloud_edas_application`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_deploy_group`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_application_scale`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_slb_attachment`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_cluster`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_instance_cluster_attachment`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_edas_application_deployment`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **New Resource:** `alicloud_cen_route_map`([#2371](https://github.com/aliyun/terraform-provider-alicloud/issues/2371))
- **Data Source:** `alicloud_edas_applications`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **Data Source:** `alicloud_edas_deploy_groups`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))
- **Data Source:** `alicloud_edas_clusters`([#2384](https://github.com/aliyun/terraform-provider-alicloud/issues/2384))

IMPROVEMENTS:

- ci supports edas and resourceManager dependencies([#2424](https://github.com/aliyun/terraform-provider-alicloud/issues/2424))
- add missing "security_group_id" attribute declaration to schema([#2417](https://github.com/aliyun/terraform-provider-alicloud/issues/2417))
- Update go sdk to 1.61.155([#2413](https://github.com/aliyun/terraform-provider-alicloud/issues/2413))
- optimized create emr cluster test case([#2397](https://github.com/aliyun/terraform-provider-alicloud/issues/2397))

BUG FIXES:

- fix_markdown_instance  documentation([#2430](https://github.com/aliyun/terraform-provider-alicloud/issues/2430))
- fix_markdown_slb_vpc  documentation([#2429](https://github.com/aliyun/terraform-provider-alicloud/issues/2429))
- fix log audit document  documentation([#2415](https://github.com/aliyun/terraform-provider-alicloud/issues/2415))
- Fix regression in writeToFile([#2412](https://github.com/aliyun/terraform-provider-alicloud/issues/2412))

## 1.81.0 (May 01, 2020)

- **New Resource:** `alicloud_hbase_instance`([#2395](https://github.com/aliyun/terraform-provider-alicloud/issues/2395))
- **New Resource:** `alicloud_adb_connection`([#2392](https://github.com/aliyun/terraform-provider-alicloud/issues/2392))
- **New Resource:** `alicloud_cs_kubernetes`([#2391](https://github.com/aliyun/terraform-provider-alicloud/issues/2391))
- **New Resource:** `alicloud_dms_enterprise_instance`([#2390](https://github.com/aliyun/terraform-provider-alicloud/issues/2390))
- **Data Source:** `alicloud_polardb_node_classes`([#2369](https://github.com/aliyun/terraform-provider-alicloud/issues/2369))

IMPROVEMENTS:

- Update go sdk to 1.61.155([#2413](https://github.com/aliyun/terraform-provider-alicloud/issues/2413))
- add test Parameter dependence([#2402](https://github.com/aliyun/terraform-provider-alicloud/issues/2402))
- improve dms docs([#2401](https://github.com/aliyun/terraform-provider-alicloud/issues/2401))
- Add sls log audit([#2389](https://github.com/aliyun/terraform-provider-alicloud/issues/2389))
- Update CHANGELOG.md([#2386](https://github.com/aliyun/terraform-provider-alicloud/issues/2386))
- return connection_string after polardb cluster created([#2379](https://github.com/aliyun/terraform-provider-alicloud/issues/2379))

BUG FIXES:

- Fix regression in writeToFile([#2412](https://github.com/aliyun/terraform-provider-alicloud/issues/2412))
- fix(log_audit): resolve cannot get region([#2411](https://github.com/aliyun/terraform-provider-alicloud/issues/2411))
- Let WriteFile return write/delete errors([#2408](https://github.com/aliyun/terraform-provider-alicloud/issues/2408))
- fix adb documents bug([#2388](https://github.com/aliyun/terraform-provider-alicloud/issues/2388))
- fix del rds ins task([#2387](https://github.com/aliyun/terraform-provider-alicloud/issues/2387))

## 1.80.1 (April 24, 2020)

IMPROVEMENTS:

- update emr tag resourceType from instance to cluste([#2383](https://github.com/aliyun/terraform-provider-alicloud/issues/2383))
- improve(cen_instances): support tags([#2376](https://github.com/aliyun/terraform-provider-alicloud/issues/2376))
- improve(sdk): upgraded the sdk and made compatibility([#2373](https://github.com/aliyun/terraform-provider-alicloud/issues/2373))
- Update oss_bucket.html.markdown([#2359](https://github.com/aliyun/terraform-provider-alicloud/issues/2359))

BUG FIXES:

- fix adb account & documents bug([#2382](https://github.com/aliyun/terraform-provider-alicloud/issues/2382))
- fix(oss): fix the bug of setting a object acl with the wrong option([#2366](https://github.com/aliyun/terraform-provider-alicloud/issues/2366))

## 1.80.0 (April 17, 2020)

- **New Resource:** `alicloud_dns_domain_attachmen`([#2365](https://github.com/aliyun/terraform-provider-alicloud/issues/2365))
- **New Resource:** `alicloud_dns_instance`([#2361](https://github.com/aliyun/terraform-provider-alicloud/issues/2361))
- **New Resource:** `alicloud_polardb_endpoint`([#2321](https://github.com/aliyun/terraform-provider-alicloud/issues/2321))
- **Data Source:** `alicloud_dns_domain_txt_guid`([#2357](https://github.com/aliyun/terraform-provider-alicloud/issues/2357))
- **Data Source:** `alicloud_kms_aliases`([#2353](https://github.com/aliyun/terraform-provider-alicloud/issues/2353))

IMPROVEMENTS:

- improve(cen_instance): support tags([#2374](https://github.com/aliyun/terraform-provider-alicloud/issues/2374))
- improve(rds_instance): remove checking zone id([#2372](https://github.com/aliyun/terraform-provider-alicloud/issues/2372))
- ADB support scale in/out([#2367](https://github.com/aliyun/terraform-provider-alicloud/issues/2367))
- improve(skd): upgraded the sdk and made compatibility([#2363](https://github.com/aliyun/terraform-provider-alicloud/issues/2363))
- improve(cen_flowlogs): append output_file([#2362](https://github.com/aliyun/terraform-provider-alicloud/issues/2362))
- remove checking instance type before creating ecs instance ang ess configuration([#2358](https://github.com/aliyun/terraform-provider-alicloud/issues/2358))

BUG FIXES:

- Fix alikafka topic tag crate bug([#2370](https://github.com/aliyun/terraform-provider-alicloud/issues/2370))
- Fix assign variable bug([#2368](https://github.com/aliyun/terraform-provider-alicloud/issues/2368))
- fix(oss): fix creation_date info displays incorrectly bug([#2364](https://github.com/aliyun/terraform-provider-alicloud/issues/2364))

## 1.79.0 (April 10, 2020)

- **New Resource:** `alicloud_auto_provisioning_group`([#2303](https://github.com/aliyun/terraform-provider-alicloud/issues/2303))

IMPROVEMENTS:

- optimize retryable request for alikafka([#2350](https://github.com/aliyun/terraform-provider-alicloud/issues/2350))
- Update data_source_alicloud_fc_triggers.go([#2348](https://github.com/aliyun/terraform-provider-alicloud/issues/2348))
- Add error retry in delete method([#2346](https://github.com/aliyun/terraform-provider-alicloud/issues/2346))
- improve(vpc): vpc and vswitch supported timeouts settings([#2345](https://github.com/aliyun/terraform-provider-alicloud/issues/2345))
- Update fc_function.html.markdown([#2342](https://github.com/aliyun/terraform-provider-alicloud/issues/2342))
- Update fc_trigger.html.markdown([#2341](https://github.com/aliyun/terraform-provider-alicloud/issues/2341))
- improve(polardb): modify the vsw specified([#2261](https://github.com/aliyun/terraform-provider-alicloud/issues/2261))
- eip associate add clientToken support([#2247](https://github.com/aliyun/terraform-provider-alicloud/issues/2247))

BUG FIXES:

- fix(polardb): fix the bug of parameters modification([#2354](https://github.com/aliyun/terraform-provider-alicloud/issues/2354))
- fix(ram): fix datasource ram users convince bug([#2352](https://github.com/aliyun/terraform-provider-alicloud/issues/2352))
- fix(rds): fix the bug of parameters modification([#2351](https://github.com/aliyun/terraform-provider-alicloud/issues/2351))
- fix(managed_kubernetes): resolve field version diff issue([#2349](https://github.com/aliyun/terraform-provider-alicloud/issues/2349))
- private_zone has the wrong description([#2344](https://github.com/aliyun/terraform-provider-alicloud/issues/2344))
- Fix create rds bug([#2343](https://github.com/aliyun/terraform-provider-alicloud/issues/2343))
- fix(db_instance): resolve deleting db instance bug([#2317](https://github.com/aliyun/terraform-provider-alicloud/issues/2317))
- user want api server's public ip when they set endpoint_public_access_enabled to true. the second parameter in DescribeClusterUserConfig is "privateIpAddress", so it should be endpoint_public_access_enabled's negative value([#2290](https://github.com/aliyun/terraform-provider-alicloud/issues/2290))



## 1.78.0 (April 03, 2020)

- **New Resource:** `alicloud_log_alert`([#2325](https://github.com/aliyun/terraform-provider-alicloud/issues/2325))
- **Data Source:** `alicloud_cen_flowlogs`([#2336](https://github.com/aliyun/terraform-provider-alicloud/issues/2336))

IMPROVEMENTS:

- improve(cen_flowlogs): add more parameters([#2338](https://github.com/aliyun/terraform-provider-alicloud/issues/2338))
- improve(mongodb): supported ssl setting([#2335](https://github.com/aliyun/terraform-provider-alicloud/issues/2335))
- Add statistics attribute support ErrorCodeMaximum for cms([#2328](https://github.com/aliyun/terraform-provider-alicloud/issues/2328))
- alicloud_kms_secret: mark secret_data as sensitive([#2322](https://github.com/aliyun/terraform-provider-alicloud/issues/2322))

BUG FIXES:

- fix create rds instance bug([#2334](https://github.com/aliyun/terraform-provider-alicloud/issues/2334))
- fix(nas_rule): resolve pagesize bug([#2330](https://github.com/aliyun/terraform-provider-alicloud/issues/2330))

## 1.77.0 (April 01, 2020)

- **New Resource:** `alicloud_kms_alias`([#2307](https://github.com/aliyun/terraform-provider-alicloud/issues/2307))
- **New Resource:** `alicloud_maxcompute_project`([#1681](https://github.com/aliyun/terraform-provider-alicloud/issues/1681))

IMPROVEMENTS:

- improve(kms_secret): improve tags([#2313](https://github.com/aliyun/terraform-provider-alicloud/issues/2313))

BUG FIXES:

- fix(ram_user): resolve importing ram user notfound bug([#2319](https://github.com/aliyun/terraform-provider-alicloud/issues/2319))
- fix adb ci bug([#2312](https://github.com/aliyun/terraform-provider-alicloud/issues/2312))
- fix(db_instance): resolve postgres testcase([#2311](https://github.com/aliyun/terraform-provider-alicloud/issues/2311))

## 1.76.0 (March 27, 2020)

- **New Resource:** `alicloud_kms_secret`([#2310](https://github.com/aliyun/terraform-provider-alicloud/issues/2310))

IMPROVEMENTS:

- change default autoscaler tag and refactor docs of managed kubernetes([#2309](https://github.com/aliyun/terraform-provider-alicloud/issues/2309))
- improve(sdk): update provider sdk and make it compatible([#2306](https://github.com/aliyun/terraform-provider-alicloud/issues/2306))
- add security group id and TDE for mongodb sharding([#2298](https://github.com/aliyun/terraform-provider-alicloud/issues/2298))
- improve cen_instance and cen_flowlog([#2297](https://github.com/aliyun/terraform-provider-alicloud/issues/2297))
- added support for isp_cities in site_monito([#2296](https://github.com/aliyun/terraform-provider-alicloud/issues/2296))
- add security group id for kvstore([#2292](https://github.com/aliyun/terraform-provider-alicloud/issues/2292))(https://github.com/aliyun/terraform-provider-alicloud/pull/2292))
- support parameter DesiredCapacity([#2277](https://github.com/aliyun/terraform-provider-alicloud/issues/2277))

BUG FIXES:

-fix(cen):modify resource_alicloud_cen_instance_grant([#2293](https://github.com/aliyun/terraform-provider-alicloud/issues/2293))


## 1.75.0 (March 20, 2020)

- **Data Source:** `alicloud_adb_zones`([#2248](https://github.com/aliyun/terraform-provider-alicloud/issues/2248))
- **Data Source:** `alicloud_slb_zones`([#2244](https://github.com/aliyun/terraform-provider-alicloud/issues/2244))
- **Data Source:** `alicloud_elasticsearch_zones`([#2243](https://github.com/aliyun/terraform-provider-alicloud/issues/2243))

IMPROVEMENTS:

- improve(db_instance): support force_restart([#2287](https://github.com/aliyun/terraform-provider-alicloud/issues/2287))
- improve the zones markdown([#2285](https://github.com/aliyun/terraform-provider-alicloud/issues/2285))
- Add Terway and other kubernetes params to resource([#2284](https://github.com/aliyun/terraform-provider-alicloud/issues/2284))

BUG FIXES:

- fix ADB data source zones([#2283](https://github.com/aliyun/terraform-provider-alicloud/issues/2283))
- fix polardb data source zones([#2274](https://github.com/aliyun/terraform-provider-alicloud/issues/2274))
- fix adb ci bug([#2272](https://github.com/aliyun/terraform-provider-alicloud/issues/2272))
- fix(cen):modify resource_alicloud_cen_instance_attachment([#2269](https://github.com/aliyun/terraform-provider-alicloud/issues/2269))

## 1.74.1 (March 17, 2020)

IMPROVEMENTS:

- improve(alikafka_instance): suspend kafka prepaid test([#2264](https://github.com/aliyun/terraform-provider-alicloud/issues/2264))
- improve(gpdb): modify the vsw specified([#2260](https://github.com/aliyun/terraform-provider-alicloud/issues/2260))
- improve(elasticsearch): modify the vsw specified([#2239](https://github.com/aliyun/terraform-provider-alicloud/issues/2239))

BUG FIXES:

- tagResource bug fix([#2266](https://github.com/aliyun/terraform-provider-alicloud/issues/2266))
- fix(kvstore_instance): resolve auto_renew incorrect value([#2265](https://github.com/aliyun/terraform-provider-alicloud/issues/2265))

## 1.74.0 (March 16, 2020)

- **Data Source:** `alicloud_fc_zones`([#2256](https://github.com/aliyun/terraform-provider-alicloud/issues/2256))
- **Data Source:** `alicloud_polardb_zones`([#2250](https://github.com/aliyun/terraform-provider-alicloud/issues/2250))

IMPROVEMENTS:

- improve(hbase): modify the vsw specified([#2259](https://github.com/aliyun/terraform-provider-alicloud/issues/2259))
- improve(elasticsearch): data_source support tags([#2257](https://github.com/aliyun/terraform-provider-alicloud/issues/2257))
- rename polardb test name([#2255](https://github.com/aliyun/terraform-provider-alicloud/issues/2255))
- corrct cen_flowlog docs([#2254](https://github.com/aliyun/terraform-provider-alicloud/issues/2254))
- Adjust the return error mode([#2252](https://github.com/aliyun/terraform-provider-alicloud/issues/2252))
- improve(elasticsearch): resource support tags([#2251](https://github.com/aliyun/terraform-provider-alicloud/issues/2251))

BUG FIXES:

- fix(cms_alarm): resolve the effective_interval default value([#2253](https://github.com/aliyun/terraform-provider-alicloud/issues/2253))

## 1.73.0 (March 13, 2020)

- **New Resource:** `alicloud_cen_flowlog`([#2229](https://github.com/aliyun/terraform-provider-alicloud/issues/2229))
- **Data Source:** `alicloud_gpdb_zones`([#2241](https://github.com/aliyun/terraform-provider-alicloud/issues/2241))
- **Data Source:** `alicloud_hbase_zones`([#2240](https://github.com/aliyun/terraform-provider-alicloud/issues/2240))
- **Data Source:** `alicloud_mongodb_zones`([#2238](https://github.com/aliyun/terraform-provider-alicloud/issues/2238))
- **Data Source:** `alicloud_kvstore_zones`([#2236](https://github.com/aliyun/terraform-provider-alicloud/issues/2236))
- **Data Source:** `alicloud_db_zones`([#2235](https://github.com/aliyun/terraform-provider-alicloud/issues/2235))

IMPROVEMENTS:

- improve(ecs): supported auto snapshop policy([#2245](https://github.com/aliyun/terraform-provider-alicloud/issues/2245))
- add flowlog docs in the alicloud.erb([#2237](https://github.com/aliyun/terraform-provider-alicloud/issues/2237))
- fix(elasticsearch): update the sdk([#2234](https://github.com/aliyun/terraform-provider-alicloud/issues/2234))
- add new version aliyungo([#2232](https://github.com/aliyun/terraform-provider-alicloud/issues/2232))
- terraform format examples [2231]
- Hbase tags([#2228](https://github.com/aliyun/terraform-provider-alicloud/issues/2228))
- mongodb support TDE [GH2207]

BUG FIXES:

- fix(cms_alarm): resolve the effective_interval format bug([#2242](https://github.com/aliyun/terraform-provider-alicloud/issues/2242))
- fix SQLServer testcase([#2233](https://github.com/aliyun/terraform-provider-alicloud/issues/2233))
- fix(es): fix ci bug([#2230](https://github.com/aliyun/terraform-provider-alicloud/issues/2230))

## 1.72.0 (March 06, 2020)

- **New Resource:** `alicloud_cms_site_monitor`([#2191](https://github.com/aliyun/terraform-provider-alicloud/issues/2191))
- **Data Source:** `alicloud_ess_alarms`([#2215](https://github.com/aliyun/terraform-provider-alicloud/issues/2215))
- **Data Source:** `alicloud_ess_notifications`([#2161](https://github.com/aliyun/terraform-provider-alicloud/issues/2161))
- **Data Source:** `alicloud_ess_scheduled_tasks`([#2160](https://github.com/aliyun/terraform-provider-alicloud/issues/2160))

IMPROVEMENTS:

- improve(mns_topic_subscription): remove the validate([#2225](https://github.com/aliyun/terraform-provider-alicloud/issues/2225))
- Support the parameter of 'protocol'([#2214](https://github.com/aliyun/terraform-provider-alicloud/issues/2214))
- improve sweeper test([#2212](https://github.com/aliyun/terraform-provider-alicloud/issues/2212))
- supported bootstrap action when create a new emr cluster instance([#2210](https://github.com/aliyun/terraform-provider-alicloud/issues/2210))

BUG FIXES:

- fix sweep test bug([#2223](https://github.com/aliyun/terraform-provider-alicloud/issues/2223))
- fix the bug of RAM user cannot be destroyed([#2219](https://github.com/aliyun/terraform-provider-alicloud/issues/2219))
- fix(elasticsearch_instance): resolve the ci bug([#2216](https://github.com/aliyun/terraform-provider-alicloud/issues/2216))
- fix(slb): fix slb listener fields and rules creation bug([#2209](https://github.com/aliyun/terraform-provider-alicloud/issues/2209))

## 1.71.2 (February 28, 2020)

IMPROVEMENTS:

- improve alikafka sweeper test([#2206](https://github.com/aliyun/terraform-provider-alicloud/issues/2206))
- added filter parameter instance type about data source emr_instance_t… ([#2205](https://github.com/aliyun/terraform-provider-alicloud/issues/2205))
- improve(polardb): fix update polardb cluster db_node_class will delete instance([#2203](https://github.com/aliyun/terraform-provider-alicloud/issues/2203))
- improve(cen): add more sweeper test for cen and update go sdk([#2201](https://github.com/aliyun/terraform-provider-alicloud/issues/2201))
- improve(mns_topic_subscription): supports json([#2200](https://github.com/aliyun/terraform-provider-alicloud/issues/2200))
- update go sdk to 1.61.1([#2197](https://github.com/aliyun/terraform-provider-alicloud/issues/2197))
- improve(snat): add snat_entry_name for this resource([#2196](https://github.com/aliyun/terraform-provider-alicloud/issues/2196))
- add sweeper for polardb and hbase([#2195](https://github.com/aliyun/terraform-provider-alicloud/issues/2195))
- improve(nat_gateways): add output vpc_id([#2194](https://github.com/aliyun/terraform-provider-alicloud/issues/2194))
- add retry for throttling when setting tags([#2193](https://github.com/aliyun/terraform-provider-alicloud/issues/2193))
- improve(client): remove useless goSdkMutex([#2192](https://github.com/aliyun/terraform-provider-alicloud/issues/2192))

BUG FIXES:

- fix(cms_alarm): resolve the creating rule dunplicated([#2211](https://github.com/aliyun/terraform-provider-alicloud/issues/2211))
- fix(ess): fix create ess scaling group error([#2208](https://github.com/aliyun/terraform-provider-alicloud/issues/2208))
- fix(ess): fix the bug of creating ess scaling group([#2204](https://github.com/aliyun/terraform-provider-alicloud/issues/2204))
fix(common_bandwidth): resolve BandwidthPackageOperation.conflict([#2199](https://github.com/aliyun/terraform-provider-alicloud/issues/2199))

## 1.71.1 (February 21, 2020)

IMPROVEMENTS:

- update SnatEntry test case([#2187](https://github.com/aliyun/terraform-provider-alicloud/issues/2187))
- improve(vpcs): support outputting tags([#2184](https://github.com/aliyun/terraform-provider-alicloud/issues/2184))
- improve(instance): remove sdk mutex and improve instance creating speed([#2181](https://github.com/aliyun/terraform-provider-alicloud/issues/2181))
- (improve market_products): supports more filter parameter([#2177](https://github.com/aliyun/terraform-provider-alicloud/issues/2177))
- add heyuan region and datasource market supports available_region([#2176](https://github.com/aliyun/terraform-provider-alicloud/issues/2176))
- improve(ecs_instance): add tags into runInstances request([#2175](https://github.com/aliyun/terraform-provider-alicloud/issues/2175))
- improve(ecs_instance): improve security groups([#2174](https://github.com/aliyun/terraform-provider-alicloud/issues/2174))
- improve(fc_function): remove useless code([#2173](https://github.com/aliyun/terraform-provider-alicloud/issues/2173))
- add support for create snat entry with source_dir([#2170](https://github.com/aliyun/terraform-provider-alicloud/issues/2170))

BUG FIXES:

- fix(instance): resolve LastTokenProcessing error when modifying nework spec([#2186](https://github.com/aliyun/terraform-provider-alicloud/issues/2186))
- fix(instance): resolve modifying network spec LastOrderProcessing error([#2185](https://github.com/aliyun/terraform-provider-alicloud/issues/2185))
- fix(instance): resolve volume_tags diff bug when new resource([#2182](https://github.com/aliyun/terraform-provider-alicloud/issues/2182))
- fix(image): fix the bug of created image by disk([#2180](https://github.com/aliyun/terraform-provider-alicloud/issues/2180))
- Fix creating instance with multiple security groups([#2168](https://github.com/aliyun/terraform-provider-alicloud/issues/2168))


## 1.71.0 (February 14, 2020)

- **New Resource:** `alicloud_adb_account`([#2169](https://github.com/aliyun/terraform-provider-alicloud/issues/2169))
- **New Resource:** `alicloud_adb_backup_policy`([#2169](https://github.com/aliyun/terraform-provider-alicloud/issues/2169))
- **Data Source:** `alicloud_adb_clusters`([#2153](https://github.com/aliyun/terraform-provider-alicloud/issues/2153))

IMPROVEMENTS:

- add market product image id([#2171](https://github.com/aliyun/terraform-provider-alicloud/issues/2171))
- fixed regional sts endpoint([#2167](https://github.com/aliyun/terraform-provider-alicloud/issues/2167))
- improve(cms): add computed for effective_interval([#2163](https://github.com/aliyun/terraform-provider-alicloud/issues/2163))

BUG FIXES:

- fix(ram_login_profile): resolve not found when deleting and deprecate alicloud_slb_attachment([#2164](https://github.com/aliyun/terraform-provider-alicloud/issues/2164))
- fix(db_account_privilege): resolve privilege timeout bug on PosrgreSql([#2159](https://github.com/aliyun/terraform-provider-alicloud/issues/2159))

## 1.70.3 (February 06, 2020)

IMPROVEMENTS:

- improve(db_instances): add more parameters([#2158](https://github.com/aliyun/terraform-provider-alicloud/issues/2158))
- improve(kvstore_account): correct test case([#2154](https://github.com/aliyun/terraform-provider-alicloud/issues/2154))

BUG FIXES:

- Update go SDK to fix redis bug([#2149](https://github.com/aliyun/terraform-provider-alicloud/issues/2149))

## 1.70.2 (January 31, 2020)

IMPROVEMENTS:

- improve(slb): improve set slb tags([#2147](https://github.com/aliyun/terraform-provider-alicloud/issues/2147))
- improve(ram_login_profile): resolve EntityNotExist.User([#2146](https://github.com/aliyun/terraform-provider-alicloud/issues/2146))
- improve client endpoint([#2144](https://github.com/aliyun/terraform-provider-alicloud/issues/2144))
- improve(client): add a method when load endpoint from local file ([#2141](https://github.com/aliyun/terraform-provider-alicloud/issues/2141))
- improve(error): remove useless error codes([#2140](https://github.com/aliyun/terraform-provider-alicloud/issues/2140))
- improve(provider): change IsExceptedError to IsExpectedErrors([#2139](https://github.com/aliyun/terraform-provider-alicloud/issues/2139))
- improve(instance): remove the useless method([#2138](https://github.com/aliyun/terraform-provider-alicloud/issues/2138))

BUG FIXES:

- fix(ram): resolve ram resources not found error([#2143](https://github.com/aliyun/terraform-provider-alicloud/issues/2143))
- fix(slb): resolve listTags throttling([#2142](https://github.com/aliyun/terraform-provider-alicloud/issues/2142))
- fix(instance): resolve the untag bug([#2137](https://github.com/aliyun/terraform-provider-alicloud/issues/2137))
- fix vpn bug([#2065](https://github.com/aliyun/terraform-provider-alicloud/issues/2065))

## 1.70.1 (January 23, 2020)

IMPROVEMENTS:

- added data source emr main versions parameter filter: cluster_type([#2130](https://github.com/aliyun/terraform-provider-alicloud/issues/2130))
- Features/upgrade cluster([#2129](https://github.com/aliyun/terraform-provider-alicloud/issues/2129))
- improve(mongodb_sharding): removing the limitation of node_storage([#2128](https://github.com/aliyun/terraform-provider-alicloud/issues/2128))
- improve(hbase): add precheck for the test cases([#2127](https://github.com/aliyun/terraform-provider-alicloud/issues/2127))
- Support update alikafka topic partition num and remark([#2096](https://github.com/aliyun/terraform-provider-alicloud/issues/2096))

BUG FIXES:

- fix the bug of create emr gateway failed and optimized status delay time([#2124](https://github.com/aliyun/terraform-provider-alicloud/issues/2124))

## 1.70.0 (January 17, 2020)

- **Data Source:** `alicloud_polardb_accounts`([#2091](https://github.com/aliyun/terraform-provider-alicloud/issues/2091))
- **Data Source:** `alicloud_polardb_databases`([#2091](https://github.com/aliyun/terraform-provider-alicloud/issues/2091))

IMPROVEMENTS:

- improve(slb_listener): add document for health_check_method([#2121](https://github.com/aliyun/terraform-provider-alicloud/issues/2121))
- modify:cen_instance_grant.html.markdown("alicloud_cen_instance_grant.foo")([#2120](https://github.com/aliyun/terraform-provider-alicloud/issues/2120))
- improve drds and rds sweeper test([#2119](https://github.com/aliyun/terraform-provider-alicloud/issues/2119))
- improve(kvstore_instance_classes): add validateFunc for engine([#2117](https://github.com/aliyun/terraform-provider-alicloud/issues/2117))
- improve(instance): close partial([#2115](https://github.com/aliyun/terraform-provider-alicloud/issues/2115))
- improve(instance): supports setting auto_release_time#2095([#2105](https://github.com/aliyun/terraform-provider-alicloud/issues/2105))
- improve(slb) update slb_listener add health_check_method([#2102](https://github.com/aliyun/terraform-provider-alicloud/issues/2102))
- improve(elasticsearch): resource support to renew a PrePaid instance([#2099](https://github.com/aliyun/terraform-provider-alicloud/issues/2099))
- improve(rds): feature rds support sql audit records([#2082](https://github.com/aliyun/terraform-provider-alicloud/issues/2082))

BUG FIXES:

- fix(drds_instance): resolve parsing response error([#2118](https://github.com/aliyun/terraform-provider-alicloud/issues/2118))
- fix:cen_instance.html.markdown(modify docs of name & description)([#2116](https://github.com/aliyun/terraform-provider-alicloud/issues/2116))
- fix(rds): fix rds modify sql collector policy bug([#2110](https://github.com/aliyun/terraform-provider-alicloud/issues/2110))
- fix(rds): fix rds modify db instance spec bug([#2108](https://github.com/aliyun/terraform-provider-alicloud/issues/2108))
- fix(drds_instance): resolve parsing failed when creating([#2106](https://github.com/aliyun/terraform-provider-alicloud/issues/2106))
- fix(snat_entry): resolve the error OperationUnsupported.EipNatBWPCheck([#2104](https://github.com/aliyun/terraform-provider-alicloud/issues/2104))
- fix(pvtz_zone): correct the docs error([#2097](https://github.com/aliyun/terraform-provider-alicloud/issues/2097))

## 1.69.1 (January 13, 2020)

IMPROVEMENTS:

- improve(market): supported new field 'search_term'([#2090](https://github.com/aliyun/terraform-provider-alicloud/issues/2090))

BUG FIXES:

- fix(instance_types): resolve a bug results from the filed spelling error([#2093](https://github.com/aliyun/terraform-provider-alicloud/issues/2093))

## 1.69.0 (January 13, 2020)

- **New Resource:** `alicloud_market_order`([#2084](https://github.com/aliyun/terraform-provider-alicloud/issues/2084))
- **New Resource:** `alicloud_image_import`([#2051](https://github.com/aliyun/terraform-provider-alicloud/issues/2051))
- **Data Source:** `alicloud_market_product`([#2070](https://github.com/aliyun/terraform-provider-alicloud/issues/2070))

IMPROVEMENTS:

- improve(api_gateway_group): add outputs sub_domain and vpc_domain([#2088](https://github.com/aliyun/terraform-provider-alicloud/issues/2088))
- improve(hbase): expose the hbase docs([#2087](https://github.com/aliyun/terraform-provider-alicloud/issues/2087))
- improve(pvtz): supports proxy_pattern, user_client_ip and lang([#2086](https://github.com/aliyun/terraform-provider-alicloud/issues/2086))
- improve(test): support force sleep while running testcase([#2081](https://github.com/aliyun/terraform-provider-alicloud/issues/2081))
- improve(emr): improve sweeper test for emr([#2078](https://github.com/aliyun/terraform-provider-alicloud/issues/2078))
- improve(slb): update slb_server_certificate([#2077](https://github.com/aliyun/terraform-provider-alicloud/issues/2077))
- improve(elasticsearch): resource elasticsearch_instance support update for instance_charge_type([#2073](https://github.com/aliyun/terraform-provider-alicloud/issues/2073))
- improve(instance_types): support gpu amount and gpu spec([#2069](https://github.com/aliyun/terraform-provider-alicloud/issues/2069))
- modify(market): modify the attributes of market products datasource([#2068](https://github.com/aliyun/terraform-provider-alicloud/issues/2068))
- improve(listener): supports description([#2067](https://github.com/aliyun/terraform-provider-alicloud/issues/2067))
- improve(testcase): change test image name_regex([#2066](https://github.com/aliyun/terraform-provider-alicloud/issues/2066))
- improve(instances): improve its efficiency when fetching its disk mappings([#2062](https://github.com/aliyun/terraform-provider-alicloud/issues/2062))
- improve(image): correct docs([#2061](https://github.com/aliyun/terraform-provider-alicloud/issues/2061))
- improve(instances): supports ram_role_name([#2060](https://github.com/aliyun/terraform-provider-alicloud/issues/2060))
- improve(db_instance): support security_group_ids([#2056](https://github.com/aliyun/terraform-provider-alicloud/issues/2056))
- improve(api): added app_code in attribute apps([#2055](https://github.com/aliyun/terraform-provider-alicloud/issues/2055))
- improve(rds): feature rds backup policy improve the functions([#2042](https://github.com/aliyun/terraform-provider-alicloud/issues/2042))

BUG FIXES:

- fix(ram_roles): getRole not found error([#2089](https://github.com/aliyun/terraform-provider-alicloud/issues/2089))
- fix(polardb): fix polardb add parameters bug([#2083](https://github.com/aliyun/terraform-provider-alicloud/issues/2083))
- fix(ecs): fix the bug of ecs instance not supported([#2063](https://github.com/aliyun/terraform-provider-alicloud/issues/2063))
- fix(image): fix image disk mapping size bug([#2052](https://github.com/aliyun/terraform-provider-alicloud/issues/2052))


## 1.68.0 (January 06, 2020)

- **New Resource:** `alicloud_export_image`([#2036](https://github.com/aliyun/terraform-provider-alicloud/issues/2036))
- **New Resource:** `alicloud_image_share_permission`([#2026](https://github.com/aliyun/terraform-provider-alicloud/issues/2026))
- **New Resource:** `alicloud_polardb_endpoint_address`([#2020](https://github.com/aliyun/terraform-provider-alicloud/issues/2020))
- **Data Source:** `alicloud_polardb_endpoints`([#2020](https://github.com/aliyun/terraform-provider-alicloud/issues/2020))

IMPROVEMENTS:

- improve(db_readonly_instance): supports tags([#2050](https://github.com/aliyun/terraform-provider-alicloud/issues/2050))
- improve(db_instance): support setting db_instance_storage_type([#2048](https://github.com/aliyun/terraform-provider-alicloud/issues/2048))
- switch r-kvstore sdk to r_kvstor([#2047](https://github.com/aliyun/terraform-provider-alicloud/issues/2047))
- ess-rules/groups/configrution three markdown files different with codes([#2046](https://github.com/aliyun/terraform-provider-alicloud/issues/2046))
- improve(polardb): feature polardb support tags #2045
- improve(slb): update slb_server_certificate([#2044](https://github.com/aliyun/terraform-provider-alicloud/issues/2044))
- Modify naming issues in alicloud_image_copy([#2040](https://github.com/aliyun/terraform-provider-alicloud/issues/2040))
- rollback hbase resource and datasource because of them need to be improved([#2034](https://github.com/aliyun/terraform-provider-alicloud/issues/2034))
- improve(sasl): Implement update method for sasl user([#2027](https://github.com/aliyun/terraform-provider-alicloud/issues/2027))


BUG FIXES:

- fix(security_group): fix enterprise sg does not support inner access policy from issue #1961 @yongzhang([#2049](https://github.com/aliyun/terraform-provider-alicloud/issues/2049))

## 1.67.0 (December 27, 2019)

- **New Resource:** `alicloud_hbase_instance`([#2012](https://github.com/aliyun/terraform-provider-alicloud/issues/2012))
- **New Resource:** `alicloud_polardb_account_privilege`([#2005](https://github.com/aliyun/terraform-provider-alicloud/issues/2005))
- **New Resource:** `alicloud_polardb_account`([#1998](https://github.com/aliyun/terraform-provider-alicloud/issues/1998))
- **Data Source:** `alicloud_hbase_instances`([#2012](https://github.com/aliyun/terraform-provider-alicloud/issues/2012))


IMPROVEMENTS:

- rollback hbase resource and datasource because of them need to be improved([#2033](https://github.com/aliyun/terraform-provider-alicloud/issues/2033))
- improve(ci): add hbase ci([#2031](https://github.com/aliyun/terraform-provider-alicloud/issues/2031))
- improve(mongodb): hidden some security ips([#2025](https://github.com/aliyun/terraform-provider-alicloud/issues/2025))
- improve(cdn_config): remove the args private_oss_tbl([#2024](https://github.com/aliyun/terraform-provider-alicloud/issues/2024))
- improve(ons): update sdk and remove PreventCache in ons([#2014](https://github.com/aliyun/terraform-provider-alicloud/issues/2014))
- add resource group id([#2010](https://github.com/aliyun/terraform-provider-alicloud/issues/2010))
- improve(kvstore): remove type 'Super' for kvstore([#2009](https://github.com/aliyun/terraform-provider-alicloud/issues/2009))
- improve(emr): support emr cluster tag([#2008](https://github.com/aliyun/terraform-provider-alicloud/issues/2008))
- feat(alicloud/yundun_bastionhost): Add support for Cloud Bastionhost([#2006](https://github.com/aliyun/terraform-provider-alicloud/issues/2006))

BUG FIXES:

- fix(rds): fix policy sqlserver test bug([#2030](https://github.com/aliyun/terraform-provider-alicloud/issues/2030))
- fix(rds): fix rds resource alicloud_db_backup_policy`s log_backup bug([#2017](https://github.com/aliyun/terraform-provider-alicloud/issues/2017))
- fix(db_backup_policy): fix postgresql backup policy bug([#2003](https://github.com/aliyun/terraform-provider-alicloud/issues/2003))


## 1.66.0 (December 20, 2019)

- **New Resource:** `alicloud_kvstore_account`([#1993](https://github.com/aliyun/terraform-provider-alicloud/issues/1993))
- **New Resource:** `alicloud_copy_image`([#1978](https://github.com/aliyun/terraform-provider-alicloud/issues/1978))
- **New Resource:** `alicloud_polardb_database`([#1996](https://github.com/aliyun/terraform-provider-alicloud/issues/1996))
- **New Resource:** `alicloud_polardb_backup_policy`([#1991](https://github.com/aliyun/terraform-provider-alicloud/issues/1991))
- **New Resource:** `alicloud_poloardb_cluster`([#1978](https://github.com/aliyun/terraform-provider-alicloud/issues/1978))
- **New Resource:** `alicloud_alikafka_sasl_acl` （[#2000](https://github.com/aliyun/terraform-provider-alicloud/issues/2000)
- **New Resource:** `alicloud_alikafka_sasl_user` （[#2000](https://github.com/aliyun/terraform-provider-alicloud/issues/2000)
- **Data Source:** `alicloud_poloardb_clusters`([#1978](https://github.com/aliyun/terraform-provider-alicloud/issues/1978))
- **Data Source:** `alicloud_alikafka_sasl_acls` （[#2000](https://github.com/aliyun/terraform-provider-alicloud/issues/2000)）
- **Data Source:** `alicloud_alikafka_sasl_users`（[#2000](https://github.com/aliyun/terraform-provider-alicloud/issues/2000)）

IMPROVEMENTS:


- improve(SLS): Support SLS logstore index json keys([#1999](https://github.com/aliyun/terraform-provider-alicloud/issues/1999))
- improve(acl): add missing tags for acl, keypair and son([#1997](https://github.com/aliyun/terraform-provider-alicloud/issues/1997))
- improve(market): product datasource supported name regex and ids filter([#1992](https://github.com/aliyun/terraform-provider-alicloud/issues/1992))
- improve(instance): improve auto_renew_period setting([#1990](https://github.com/aliyun/terraform-provider-alicloud/issues/1990))
- documenting the replica_set_name attribute in mongodb @chanind([#1989](https://github.com/aliyun/terraform-provider-alicloud/issues/1989))
- improve(period): improve computing period method([#1988](https://github.com/aliyun/terraform-provider-alicloud/issues/1988))
- improve(prepaid): support computing period by week([#1985](https://github.com/aliyun/terraform-provider-alicloud/issues/1985))
- improve(prepaid): add a method to fix period importer diff([#1984](https://github.com/aliyun/terraform-provider-alicloud/issues/1984))
- improve(mongoDB): supported field 'tags'([#1980](https://github.com/aliyun/terraform-provider-alicloud/issues/1980))
- add output to ssl vpn client cert @ionTea([#1979](https://github.com/aliyun/terraform-provider-alicloud/issues/1979))

BUG FIXES:

- fix(db_backup_policy): fix postgresql backup policy bug([#2002](https://github.com/aliyun/terraform-provider-alicloud/issues/2002))
- fix(fc): fixed bug from issue #1961 @yokzy88([#1987](https://github.com/aliyun/terraform-provider-alicloud/issues/1987))
- fix(vpn): fix bug from issue #1965 @chanind([#1981](https://github.com/aliyun/terraform-provider-alicloud/issues/1981))
- fix(vpn): added Computed to field `vswitch_id` @chanind([#1977](https://github.com/aliyun/terraform-provider-alicloud/issues/1977))

## 1.65.0 (December 13, 2019)

- **New Resource:** `alicloud_reserved_instance`([#1967](https://github.com/aliyun/terraform-provider-alicloud/issues/1967))
- **New Resource:** `alicloud_cs_kubernetes_autoscaler`([#1956](https://github.com/aliyun/terraform-provider-alicloud/issues/1956))
- **New Data Source:** `alicloud_caller_identity`([#1944](https://github.com/aliyun/terraform-provider-alicloud/issues/1944))
- **New Resource:** `alicloud_sag_client_user`([#1807](https://github.com/aliyun/terraform-provider-alicloud/issues/1807))

IMPROVEMENTS:

- improve(ess_vserver_groups): improve docs([#1976](https://github.com/aliyun/terraform-provider-alicloud/issues/1976))
- improve(kvstore_instance): set period using createtime and endtime([#1971](https://github.com/aliyun/terraform-provider-alicloud/issues/1971))
- improve(slb_server_group): set servers to computed and avoid diff when using ess_scaling_vserver_group([#1970](https://github.com/aliyun/terraform-provider-alicloud/issues/1970))
- improve(k8s):add AccessKey and AccessKeySecret instead of RamRole([#1966](https://github.com/aliyun/terraform-provider-alicloud/issues/1966))

BUG FIXES:

- fix(market): remove the suggested_price check for avoid the error of testcase([#1964](https://github.com/aliyun/terraform-provider-alicloud/issues/1964))
- fix(provider): Resolve issues from aone.([#1963](https://github.com/aliyun/terraform-provider-alicloud/issues/1963))
- fix(market): remove the tags check for avoid the error of testcase([#1962](https://github.com/aliyun/terraform-provider-alicloud/issues/1962))
- fix(alicloud/yundun_bastionhost): Bastionhost RAM policy authorization bug fix([#1960](https://github.com/aliyun/terraform-provider-alicloud/issues/1960))
- fix(datahub): fix updating datahub topic comment bug([#1959](https://github.com/aliyun/terraform-provider-alicloud/issues/1959))
- fix(kms): correct test case errors ([#1958](https://github.com/aliyun/terraform-provider-alicloud/issues/1958))
- fix(validator): update package github.com/denverdino/aliyungo/cdn([#1946](https://github.com/aliyun/terraform-provider-alicloud/issues/1946))

## 1.64.0 (December 06, 2019)

- **New Data Source:** `alicloud_market_products`([#1941](https://github.com/aliyun/terraform-provider-alicloud/issues/1941))
- **New Resource:** `alicloud_cloud_connect_network_attachment`([#1933](https://github.com/aliyun/terraform-provider-alicloud/issues/1933))
- **New Resource:** `alicloud_image`([#1913](https://github.com/aliyun/terraform-provider-alicloud/issues/1913))

IMPROVEMENTS:

- improve(docs): improve module guide([#1957](https://github.com/aliyun/terraform-provider-alicloud/issues/1957))
- improve(db_account_privilege): supports more privileges([#1945](https://github.com/aliyun/terraform-provider-alicloud/issues/1945))
- improve(datasources): remove sorted_by testcase results from some internal limitation([#1943](https://github.com/aliyun/terraform-provider-alicloud/issues/1943))
- improve(sdk): Updated sdk to v1.60.280 and modified drds fields([#1938](https://github.com/aliyun/terraform-provider-alicloud/issues/1938))
- improve(snat): update example to support for snat's creation with multi eips([#1931](https://github.com/aliyun/terraform-provider-alicloud/issues/1931))
- improve(ess): resource alicloud_ess_scalinggroup_vserver_groups support parameter([#1919](https://github.com/aliyun/terraform-provider-alicloud/issues/1919))
- improve(db_instance): make 'instance_types' 'db_instance_class' 'kvstore_instance_class' support price([#1749](https://github.com/aliyun/terraform-provider-alicloud/issues/1749))

BUG FIXES:

- fix(alikafka): fix bug in when doing alikafka instance multi acc test([#1947](https://github.com/aliyun/terraform-provider-alicloud/issues/1947))
- fix(CSKubernetes): fix 3az test case([#1942](https://github.com/aliyun/terraform-provider-alicloud/issues/1942))
- fix(cdn_domain_new): constant timeout waiting for server cert([#1937](https://github.com/aliyun/terraform-provider-alicloud/issues/1937))
- fix(pvtz_zone_record): allow SRV records([#1936](https://github.com/aliyun/terraform-provider-alicloud/issues/1936))
- fix(Serverless Kubernetes): fix #1867 add serverless kube_config([#1923](https://github.com/aliyun/terraform-provider-alicloud/issues/1923))

## 1.63.0 (December 02, 2019)

- **New Resource:** `alicloud_cloud_connect_network_grant`([#1921](https://github.com/aliyun/terraform-provider-alicloud/issues/1921))
- **New Data Source:** `alicloud_yundun_bastionhost_instances`([#1894](https://github.com/aliyun/terraform-provider-alicloud/issues/1894))
- **New Resource:** `alicloud_yundun_bastionhost_instance`([#1894](https://github.com/aliyun/terraform-provider-alicloud/issues/1894))
- **New Data Source:** `alicloud_kms_ciphertext`([#1858](https://github.com/aliyun/terraform-provider-alicloud/issues/1858))
- **New Data Source:** `alicloud_kms_plaintext`([#1858](https://github.com/aliyun/terraform-provider-alicloud/issues/1858))
- **New Resource:** `alicloud_kms_ciphertext`([#1858](https://github.com/aliyun/terraform-provider-alicloud/issues/1858))
- **New Resource:** `alicloud_sag_dnat_entry`([#1823](https://github.com/aliyun/terraform-provider-alicloud/issues/1823))

IMPROVEMENTS:

- improve(vpc): add module support for vpc, vswitch and route entry([#1934](https://github.com/aliyun/terraform-provider-alicloud/issues/1934))
- improve(db_instance): tags supports case sensitive([#1930](https://github.com/aliyun/terraform-provider-alicloud/issues/1930))
- improve(mongodb_instance): adding replica_set_name to output from alicloud_mongodb_instance([#1929](https://github.com/aliyun/terraform-provider-alicloud/issues/1929))
- improve(slb): add a new field delete_protection_validation([#1927](https://github.com/aliyun/terraform-provider-alicloud/issues/1927))
- improve(kms): improve kms testcases use new method([#1926](https://github.com/aliyun/terraform-provider-alicloud/issues/1926))
- improve(provider): added 'Computed : true' to all 'ids' fields.([#1924](https://github.com/aliyun/terraform-provider-alicloud/issues/1924))
- improve(validator): Delete TagNum Count([#1920](https://github.com/aliyun/terraform-provider-alicloud/issues/1920))
- improve(sag_dnat_entry): modify docs "add subcategory"([#1918](https://github.com/aliyun/terraform-provider-alicloud/issues/1918))
- improve(sdk): upgrade alibaba go sdk([#1917](https://github.com/aliyun/terraform-provider-alicloud/issues/1917))
- improve(db_database):update db_database doc([#1916](https://github.com/aliyun/terraform-provider-alicloud/issues/1916))
- improve(validator): shift validator to official ones([#1912](https://github.com/aliyun/terraform-provider-alicloud/issues/1912))
- improve(alikafka): Support pre paid instance & Support tag resource([#1873](https://github.com/aliyun/terraform-provider-alicloud/issues/1873))

BUG FIXES:

- fix(dns_record): fix dns_record testcase bug([#1892](https://github.com/aliyun/terraform-provider-alicloud/issues/1892))
- fix(ecs): FIX: query system disk does not exist because no resource_group_id is specified([#1884](https://github.com/aliyun/terraform-provider-alicloud/issues/1884))

## 1.62.2 (November 26, 2019)

IMPROVEMENTS:

- improve(mongodb): feature mongodb support postpaid to prepaid([#1908](https://github.com/aliyun/terraform-provider-alicloud/issues/1908))
- improve(kvstore_instance_classes): skip unsupported zones([#1901](https://github.com/aliyun/terraform-provider-alicloud/issues/1901))

BUG FIXES:

- fix(pvtz_attachment): fix vpc_ids diff error([#1911](https://github.com/aliyun/terraform-provider-alicloud/issues/1911))
- fix(kafka): remove the const endpoint([#1910](https://github.com/aliyun/terraform-provider-alicloud/issues/1910))
- fix(ess): modify the type of from Set to List.([#1905](https://github.com/aliyun/terraform-provider-alicloud/issues/1905))
- fix managedkubernetes demo  documentation([#1903](https://github.com/aliyun/terraform-provider-alicloud/issues/1903))
- fix the bug of TestAccAlicloudEmrCluster_local_storage failed([#1902](https://github.com/aliyun/terraform-provider-alicloud/issues/1902))
- fix(db_instance): fix postgre testcase([#1899](https://github.com/aliyun/terraform-provider-alicloud/issues/1899))
- fix(db_instance): test case([#1898](https://github.com/aliyun/terraform-provider-alicloud/issues/1898))

## 1.62.1 (November 22, 2019)

IMPROVEMENTS:

- improve(db_instance): add new field auto_upgrade_minor_version to set minor version([#1897](https://github.com/aliyun/terraform-provider-alicloud/issues/1897))
- improve(docs): add AODC warning([#1893](https://github.com/aliyun/terraform-provider-alicloud/issues/1893))
- improve(kvstore_instance): correct its docs([#1891](https://github.com/aliyun/terraform-provider-alicloud/issues/1891))
- improve(pvtz_zone_attachment):make pvtz_zone_attachment support different region vpc([#1890](https://github.com/aliyun/terraform-provider-alicloud/issues/1890))
- improve(db, kvstore): add auto-pay when changing instance charge type([#1889](https://github.com/aliyun/terraform-provider-alicloud/issues/1889))
- improve(cs): Do not assume `private_zone` is returned from API([#1885](https://github.com/aliyun/terraform-provider-alicloud/issues/1885))
- improve(cs): modify the value of 'new_nat_gateway' to avoid errors.([#1882](https://github.com/aliyun/terraform-provider-alicloud/issues/1882))
- improve(docs): Terraform registry docs([#1881](https://github.com/aliyun/terraform-provider-alicloud/issues/1881))
- improve(rds): feature support high security access mode not submitted([#1880](https://github.com/aliyun/terraform-provider-alicloud/issues/1880))
- improve(oss): add transitions to life-cycle([#1879](https://github.com/aliyun/terraform-provider-alicloud/issues/1879))
- improve(db_instance): feature support high security access mode not submitted([#1878](https://github.com/aliyun/terraform-provider-alicloud/issues/1878))
- improve(scalingconfiguration): supports changing password_inherit([#1877](https://github.com/aliyun/terraform-provider-alicloud/issues/1877))
- improve(zones): use describeAvailableResource API to get rds available zones([#1876](https://github.com/aliyun/terraform-provider-alicloud/issues/1876))
- improve(kvstore_instance_classess): improve test case error caused by no stock([#1875](https://github.com/aliyun/terraform-provider-alicloud/issues/1875))
- improve(mns): mns support sts access([#1871](https://github.com/aliyun/terraform-provider-alicloud/issues/1871))
- improve(elasticsearch): Added retry to avoid CreateInstance TokenPreviousRequestProcessError error([#1870](https://github.com/aliyun/terraform-provider-alicloud/issues/1870))
- improve(kvstore_instance_engines): improve its code([#1864](https://github.com/aliyun/terraform-provider-alicloud/issues/1864))
- improve(kvstore): remove memcache filter from datasource test([#1863](https://github.com/aliyun/terraform-provider-alicloud/issues/1863)) 
- improve(oss_bucket_object):make oss_bucket_object support KMS encryption([#1860](https://github.com/aliyun/terraform-provider-alicloud/issues/1860))
- improve(provider): added endpoint for resources.([#1855](https://github.com/aliyun/terraform-provider-alicloud/issues/1855))

BUG FIXES:

- fix(db_backup_policy): add limitation when modify sqlservr policy([#1896](https://github.com/aliyun/terraform-provider-alicloud/issues/1896))
- fix(kvstore): remove the kvstore instance password limitation([#1886](https://github.com/aliyun/terraform-provider-alicloud/issues/1886))
- fix(mongodb_instances): fix filetering bug([#1874](https://github.com/aliyun/terraform-provider-alicloud/issues/1874))
- fix(mongodb_instances): fix name_regex bug([#1865](https://github.com/aliyun/terraform-provider-alicloud/issues/1865))
- fix(key_pair):fix key_pair testcase bug([#1862](https://github.com/aliyun/terraform-provider-alicloud/issues/1862))
- fix(autoscaling): fix autoscaling bugs.([#1832](https://github.com/aliyun/terraform-provider-alicloud/issues/1832))

## 1.62.0 (November 13, 2019)

- **New Resource:** `alicloud_yundun_dbaudit_instance`([#1819](https://github.com/aliyun/terraform-provider-alicloud/issues/1819))
- **New Data Source:** `alicloud_yundun_dbaudit_instances`([#1819](https://github.com/aliyun/terraform-provider-alicloud/issues/1819))

IMPROVEMENTS:

- improve(ess_scalingconfiguration): support password_inherit([#1856](https://github.com/aliyun/terraform-provider-alicloud/issues/1856))
- improve docs and add ci for yundun dbaudit([#1853](https://github.com/aliyun/terraform-provider-alicloud/issues/1853))

BUG FIXES:

- fix(provider): fix the bug: slice bounds out of range([#1854](https://github.com/aliyun/terraform-provider-alicloud/issues/1854))

## 1.61.0 (November 12, 2019)

- **New Resource:** `alicloud_sag_snat_entry`([#1799](https://github.com/aliyun/terraform-provider-alicloud/issues/1799))

IMPROVEMENTS:

- improve(provider): add default value for configuration_source([#1852](https://github.com/aliyun/terraform-provider-alicloud/issues/1852))
- improve(ess): add module guide for the ess resources([#1850](https://github.com/aliyun/terraform-provider-alicloud/issues/1850))
- improve(instance): postpaid instance supported 'dry_run'([#1845](https://github.com/aliyun/terraform-provider-alicloud/issues/1845))
- improve(rds): fix for hidden dts ip list([#1844](https://github.com/aliyun/terraform-provider-alicloud/issues/1844))
- improve(resource_alicloud_db_database): support Mohawk_100_BIN([#1838](https://github.com/aliyun/terraform-provider-alicloud/issues/1838))
- perf(alicloud_db_backup_policy,db_instances):perf rds document desc([#1836](https://github.com/aliyun/terraform-provider-alicloud/issues/1836))
- change sideBar([#1830](https://github.com/aliyun/terraform-provider-alicloud/issues/1830))
- modify CloudConnectNetwork_multi([#1828](https://github.com/aliyun/terraform-provider-alicloud/issues/1828))
- improve(alikafka): Added name for vpcs and vswitches([#1827](https://github.com/aliyun/terraform-provider-alicloud/issues/1827))
- support to create emr gateway cluster instance([#1821](https://github.com/aliyun/terraform-provider-alicloud/issues/1821))

BUG FIXES:

- fix(cs_kubenrnetes): fix terraform docs documentation([#1851](https://github.com/aliyun/terraform-provider-alicloud/issues/1851))
- fix(nat_gateway):fix nat_gateway period bug([#1841](https://github.com/aliyun/terraform-provider-alicloud/issues/1841))
- fix waitfor method nil bug([#1840](https://github.com/aliyun/terraform-provider-alicloud/issues/1840))
- fix(ess): use GetOkExists to avoid some potential bugs([#1835](https://github.com/aliyun/terraform-provider-alicloud/issues/1835))

## 1.60.0 (November 01, 2019)

- **New Data Source:** `alicloud_emr_disk_types`([#1805](https://github.com/aliyun/terraform-provider-alicloud/issues/1805))
- **New Data Source:** `alicloud_dns_resolution_lines`([#1800](https://github.com/aliyun/terraform-provider-alicloud/issues/1800))
- **New Resource:** `alicloud_sag_qos`([#1790](https://github.com/aliyun/terraform-provider-alicloud/issues/1790))
- **New Resource:** `alicloud_sag_qos_policy`([#1790](https://github.com/aliyun/terraform-provider-alicloud/issues/1790))
- **New Resource:** `alicloud_sag_qos_car`([#1790](https://github.com/aliyun/terraform-provider-alicloud/issues/1790))
- **New Resource:** `alicloud_sag_acl`([#1788](https://github.com/aliyun/terraform-provider-alicloud/issues/1788))
- **New Resource:** `alicloud_sag_acl_rule`([#1788](https://github.com/aliyun/terraform-provider-alicloud/issues/1788))
- **New Data Source:** `alicloud_sag_acls`([#1788](https://github.com/aliyun/terraform-provider-alicloud/issues/1788))
- **New Resource:** `alicloud_slb_domain_extension`([#1756](https://github.com/aliyun/terraform-provider-alicloud/issues/1756))
- **New Data Source:** `alicloud_slb_domain_extensions`([#1756](https://github.com/aliyun/terraform-provider-alicloud/issues/1756))

IMPROVEMENTS:

- alicloud_ess_scheduled_task supports Cron type([#1824](https://github.com/aliyun/terraform-provider-alicloud/issues/1824))
- vpc product datasource support resource_group_id([#1822](https://github.com/aliyun/terraform-provider-alicloud/issues/1822))
- improve(instance): modified the argument reference in doc.([#1815](https://github.com/aliyun/terraform-provider-alicloud/issues/1815))
- Add resource_group_id to data_source_alicloud_route_tables([#1814](https://github.com/aliyun/terraform-provider-alicloud/issues/1814))
- use homedir to expand shared_credentials_file value and add environment variable for it([#1811](https://github.com/aliyun/terraform-provider-alicloud/issues/1811))
- Add password to resource_alicloud_ess_scalingconfiguration([#1810](https://github.com/aliyun/terraform-provider-alicloud/issues/1810))
- add ids for db_instance_classes and remove limitation for db_database resource([#1803](https://github.com/aliyun/terraform-provider-alicloud/issues/1803))
- improve(db_instances):update tags type from string to map([#1802](https://github.com/aliyun/terraform-provider-alicloud/issues/1802))
- improve(instance): field 'user_data' supported update([#1798](https://github.com/aliyun/terraform-provider-alicloud/issues/1798))
- add doc of cloud_connect_network([#1791](https://github.com/aliyun/terraform-provider-alicloud/issues/1791))
- improve(slb): updated slb attachment testcase.([#1758](https://github.com/aliyun/terraform-provider-alicloud/issues/1758))

BUG FIXES:

- fix(tag): fix api gw, gpdb, kvstore datasource bug([#1817](https://github.com/aliyun/terraform-provider-alicloud/issues/1817))
- fix(rds): fix creating db account empty pointer bug([#1812](https://github.com/aliyun/terraform-provider-alicloud/issues/1812))
- fix(slb_listener): fix server_certificate_id diff bug and add sag ci([#1808](https://github.com/aliyun/terraform-provider-alicloud/issues/1808))
- fix(vpc): fix DescribeTag bug for vpc's datasource([#1801](https://github.com/aliyun/terraform-provider-alicloud/issues/1801))

## 1.59.0 (October 25, 2019)

- **New Resource:** `alicloud_cloud_connect_network`([#1784](https://github.com/aliyun/terraform-provider-alicloud/issues/1784))
- **New Resource:** `alicloud_alikafka_instance`([#1764](https://github.com/aliyun/terraform-provider-alicloud/issues/1764))
- **New Data Source:** `alicloud_cloud_connect_networks`([#1784](https://github.com/aliyun/terraform-provider-alicloud/issues/1784))
- **New Data Source:** `alicloud_emr_instance_types`([#1773](https://github.com/aliyun/terraform-provider-alicloud/issues/1773))
- **New Data Source:** `alicloud_emr_main_versions`([#1773](https://github.com/aliyun/terraform-provider-alicloud/issues/1773)) 
- **New Data Source:** `alicloud_alikafka_instances`([#1764](https://github.com/aliyun/terraform-provider-alicloud/issues/1764))
- **New Data Source:** `alicloud_file_crc64_checksum`([#1722](https://github.com/aliyun/terraform-provider-alicloud/issues/1722))

IMPROVEMENTS:

- improve(slb_listener): deprecate ssl_certificate_id and use server_certificate_id instead([#1797](https://github.com/aliyun/terraform-provider-alicloud/issues/1797))
- improve(slb): improve slb docs([#1796](https://github.com/aliyun/terraform-provider-alicloud/issues/1796))
- improve(slb_listener): add retry for StartLoadBalancerListener([#1794](https://github.com/aliyun/terraform-provider-alicloud/issues/1794))
- improve(fc_trigger):change testcase dependence resource cdn_domain to new([#1793](https://github.com/aliyun/terraform-provider-alicloud/issues/1793))
- improve(zones): using describeAvailableResource instead of DescribeZones for RKvstore([#1789](https://github.com/aliyun/terraform-provider-alicloud/issues/1789))
- Update ssl_vpn_server.html.markdown([#1786](https://github.com/aliyun/terraform-provider-alicloud/issues/1786))
- add resource_group_id to dns([#1781](https://github.com/aliyun/terraform-provider-alicloud/issues/1781))
- improve(provider): modified the kms field conflict to diffsuppress([#1780](https://github.com/aliyun/terraform-provider-alicloud/issues/1780))
- Always set PolicyDocument for RAM policy update([#1777](https://github.com/aliyun/terraform-provider-alicloud/issues/1777))
- rename cs_serveless_kubernetes to cs_serverless_kubernetes([#1776](https://github.com/aliyun/terraform-provider-alicloud/issues/1776))
- improve(slb): updated slb server_group testcase([#1753](https://github.com/aliyun/terraform-provider-alicloud/issues/1753))
- improve(fc_function):support code_checksum([#1722](https://github.com/aliyun/terraform-provider-alicloud/issues/1722))

BUG FIXES:

- fix(slb): address_type diff bug([#1795](https://github.com/aliyun/terraform-provider-alicloud/issues/1795))
- fix(ddosbgp): the docs error([#1782](https://github.com/aliyun/terraform-provider-alicloud/issues/1782))
- fix(instance):fix credit_specification bug([#1778](https://github.com/aliyun/terraform-provider-alicloud/issues/1778))

## 1.58.1 (October 22, 2019)

IMPROVEMENTS:

- add missing resource ddosbgp_instance docs index([#1775](https://github.com/aliyun/terraform-provider-alicloud/issues/1775))

BUG FIXES:

- fix(common_bandwidth_package): fix common bandwidth package resource_group_id forcenew bug([#1772](https://github.com/aliyun/terraform-provider-alicloud/issues/1772))

## 1.58.0 (October 18, 2019)

- **New Data Source:** `alicloud_cs_serverless_kubernetes_clusters`([#1746](https://github.com/aliyun/terraform-provider-alicloud/issues/1746))
- **New Resource:** `alicloud_cs_serverless_kubernetes`([#1746](https://github.com/aliyun/terraform-provider-alicloud/issues/1746))

IMPROVEMENTS:

- Make `resource_group_id` to computed([#1771](https://github.com/aliyun/terraform-provider-alicloud/issues/1771))
- Add tag for `resource_group_id` in the docs([#1770](https://github.com/aliyun/terraform-provider-alicloud/issues/1770))
- add resource_group_id to vpc, slb resources and data sources and revise corresponding docs([#1769](https://github.com/aliyun/terraform-provider-alicloud/issues/1769))
- improve(security_group):make security_group support resource_group_id([#1762](https://github.com/aliyun/terraform-provider-alicloud/issues/1762))
- Add resource_group_id to common_bandwidth_package(resource&data_source)([#1761](https://github.com/aliyun/terraform-provider-alicloud/issues/1761))
- improve(cen): added precheck for testcases([#1759](https://github.com/aliyun/terraform-provider-alicloud/issues/1759))
- improve(security_group):support security_group_type([#1755](https://github.com/aliyun/terraform-provider-alicloud/issues/1755))
- Add missing routing rules for alicloud_dns_record([#1754](https://github.com/aliyun/terraform-provider-alicloud/issues/1754))
- improve(slb): updated slb serverCertificate testcase([#1751](https://github.com/aliyun/terraform-provider-alicloud/issues/1751))
- improve(slb): updated slb rule testcase([#1748](https://github.com/aliyun/terraform-provider-alicloud/issues/1748))
- Improve(alicloud_ess_scaling_rule): support TargetTrackingScalingRule and StepScalingRule([#1744](https://github.com/aliyun/terraform-provider-alicloud/issues/1744))
- improve(cdn): added adddebug for tags APIs([#1741](https://github.com/aliyun/terraform-provider-alicloud/issues/1741))
- improve(slb): updated slb ca_certificate testcase([#1740](https://github.com/aliyun/terraform-provider-alicloud/issues/1740))
- improve(slb): updated slb acl testcase([#1739](https://github.com/aliyun/terraform-provider-alicloud/issues/1739))
- improve(slb): updated slb slb_attachment testcase([#1738](https://github.com/aliyun/terraform-provider-alicloud/issues/1738))
- use a new ram role instead of hardcode name about emr unit test case and example([#1732](https://github.com/aliyun/terraform-provider-alicloud/issues/1732))
- Revision of goReportCard.com suggestions([#1729](https://github.com/aliyun/terraform-provider-alicloud/issues/1729))
- improve(cs): resources supports timeouts setting([#1679](https://github.com/aliyun/terraform-provider-alicloud/issues/1679))

BUG FIXES:

- fix(instance):fix instance test bug([#1768](https://github.com/aliyun/terraform-provider-alicloud/issues/1768))
- fix slb sweep bug and add region for role test([#1752](https://github.com/aliyun/terraform-provider-alicloud/issues/1752))
- fix (cs) : log_config support create new project([#1745](https://github.com/aliyun/terraform-provider-alicloud/issues/1745))
- fix(cs): modify the new_nat_gateway field in testcase to avoid InstanceRouterEntryNotExist error([#1733](https://github.com/aliyun/terraform-provider-alicloud/issues/1733))
- fix(mongodb):fix password encrypt bug([#1730](https://github.com/aliyun/terraform-provider-alicloud/issues/1730))
- fix typo in worker_instance_types description([#1726](https://github.com/aliyun/terraform-provider-alicloud/issues/1726))

## 1.57.1 (October 11, 2019)

IMPROVEMENTS:

- improve:improve some resource support encrypt password([#1727](https://github.com/aliyun/terraform-provider-alicloud/issues/1727))
- improve(sdk): updated sdk to v1.60.191([#1725](https://github.com/aliyun/terraform-provider-alicloud/issues/1725))
- update tablestore package([#1719](https://github.com/aliyun/terraform-provider-alicloud/issues/1719))
- managekubernetes support sls([#1718](https://github.com/aliyun/terraform-provider-alicloud/issues/1718))
- improve(instance): support encrypt password when creating or updating ecs instance([#1711](https://github.com/aliyun/terraform-provider-alicloud/issues/1711))
- update golang image version([#1709](https://github.com/aliyun/terraform-provider-alicloud/issues/1709))
- Added credit_specification to ECS instance resource([#1705](https://github.com/aliyun/terraform-provider-alicloud/issues/1705))
- improve(slb_rule): remove `name` forcenew and make it can be updated([#1703](https://github.com/aliyun/terraform-provider-alicloud/issues/1703))
- upgrade terraform package([#1702](https://github.com/aliyun/terraform-provider-alicloud/issues/1702))
- improve emr test case, update document([#1698](https://github.com/aliyun/terraform-provider-alicloud/issues/1698))
- improve emr test case([#1697](https://github.com/aliyun/terraform-provider-alicloud/issues/1697))
- improve(provider): update go version to 1.12([#1686](https://github.com/aliyun/terraform-provider-alicloud/issues/1686))
- impove(slb_listener) slb listener support same port([#1655](https://github.com/aliyun/terraform-provider-alicloud/issues/1655))

BUG FIXES:

- fix go clean error in the ci([#1710](https://github.com/aliyun/terraform-provider-alicloud/issues/1710))

## 1.57.0 (September 27, 2019)

- **New Resource:** `alicloud_ddosbgp_instance`([#1650](https://github.com/aliyun/terraform-provider-alicloud/issues/1650))
- **New Data Source:** `alicloud_ddosbgp_instances`([#1650](https://github.com/aliyun/terraform-provider-alicloud/issues/1650))
- **New Resource:** `alicloud_emr_cluster`([#1644](https://github.com/aliyun/terraform-provider-alicloud/issues/1644))
- **New Resource:** `alicloud_vpn_route_entry`([#1613](https://github.com/aliyun/terraform-provider-alicloud/issues/1613))

IMPROVEMENTS:

- improve(ci): add new job emr([#1695](https://github.com/aliyun/terraform-provider-alicloud/issues/1695))
- improve(elasticsearch): added retry setting to avoid InstanceStatusNotSupportCurrentAction and InstanceActivating error([#1693](https://github.com/aliyun/terraform-provider-alicloud/issues/1693))
- improve useragent setting([#1692](https://github.com/aliyun/terraform-provider-alicloud/issues/1692))
- improve(ecs):add resource_group_id to ecs([#1690](https://github.com/aliyun/terraform-provider-alicloud/issues/1690))
- improve(sls): improve sls notfounderror([#1689](https://github.com/aliyun/terraform-provider-alicloud/issues/1689))
- improve(kafka): added retry to aviod GetTopicList Throttling.User error([#1688](https://github.com/aliyun/terraform-provider-alicloud/issues/1688))
- improve(ci): add ddosbgp job([#1687](https://github.com/aliyun/terraform-provider-alicloud/issues/1687))
- improve: rds,redis,mongodb remove the enumeration([#1684](https://github.com/aliyun/terraform-provider-alicloud/issues/1684))
- Update the default period of the ddosbgp instance to 12, add the bandwidth value 201, and update the test case([#1683](https://github.com/aliyun/terraform-provider-alicloud/issues/1683))
- improve(elasticsearch): added wait setting for retry([#1678](https://github.com/aliyun/terraform-provider-alicloud/issues/1678))
- improve(provider): change the ubuntu version to 18([#1677](https://github.com/aliyun/terraform-provider-alicloud/issues/1677))
- improve(provider): support provider test([#1675](https://github.com/aliyun/terraform-provider-alicloud/issues/1675))
- ddoscoo instance only support upgrade currently([#1673](https://github.com/aliyun/terraform-provider-alicloud/issues/1673))

BUG FIXES:

- fix unsupport account site for test([#1696](https://github.com/aliyun/terraform-provider-alicloud/issues/1696))
- fix(ram user): supported backward compatible([#1685](https://github.com/aliyun/terraform-provider-alicloud/issues/1685))

## 1.56.0 (September 20, 2019)

- **New Resource:** `alicloud_alikafka_consumer_group`([#1658](https://github.com/aliyun/terraform-provider-alicloud/issues/1658))
- **New Data Source:** `alicloud_alikafka_consumer_groups`([#1658](https://github.com/aliyun/terraform-provider-alicloud/issues/1658))
- **New Resource:** `alicloud_alikafka_topic`([#1642](https://github.com/aliyun/terraform-provider-alicloud/issues/1642))
- **New Data Source:** `alicloud_alikafka_topics`([#1642](https://github.com/aliyun/terraform-provider-alicloud/issues/1642))

IMPROVEMENTS:

- improve(elasticsearch): Added retry to avoid UpdateInstance ConcurrencyUpdateInstanceConflict error.([#1669](https://github.com/aliyun/terraform-provider-alicloud/issues/1669))
- fix(security_group_rule):fix description bug ([#1668](https://github.com/aliyun/terraform-provider-alicloud/issues/1668))
- improve: rds,redis,mongodb support modify maintain time([#1665](https://github.com/aliyun/terraform-provider-alicloud/issues/1665))
- add missing field ALICLOUD_INSTANCE_ID([#1664](https://github.com/aliyun/terraform-provider-alicloud/issues/1664))
- improve(sdk): update sdk to v1.60.164([#1663](https://github.com/aliyun/terraform-provider-alicloud/issues/1663))
- improve(ci): add ci test for alikafka([#1662](https://github.com/aliyun/terraform-provider-alicloud/issues/1662))
- improve(provider): rename source_name to configuration_source([#1661](https://github.com/aliyun/terraform-provider-alicloud/issues/1661))
- improve(cen): Added wait time to avoid CreateCen Operation.Blocking error([#1660](https://github.com/aliyun/terraform-provider-alicloud/issues/1660))
- improve(provider): add a new field source_name to mark template([#1657](https://github.com/aliyun/terraform-provider-alicloud/issues/1657))
- improve(vpc): Added retry to avoid ListTagResources Throttling error([#1652](https://github.com/aliyun/terraform-provider-alicloud/issues/1652))
- update VPNgateway resource vswitchId field([#1643](https://github.com/aliyun/terraform-provider-alicloud/issues/1643))

BUG FIXES:

- fix(ess_alarm):The 'ForceNew' attribute of input parameter 'scaling_group_id' is set 'True'.([#1671](https://github.com/aliyun/terraform-provider-alicloud/issues/1671))
- fix(testCommon):fix test common bug([#1666](https://github.com/aliyun/terraform-provider-alicloud/issues/1666))

## 1.55.4 (September 17, 2019)

IMPROVEMENTS:

- improve(table store): set primary key to forcenew([#1654](https://github.com/aliyun/terraform-provider-alicloud/issues/1654))
- improve(docs): Added sensitive tag for the doc which has password([#1653](https://github.com/aliyun/terraform-provider-alicloud/issues/1653))
- improve(provider): add the provider version in the useragent([#1651](https://github.com/aliyun/terraform-provider-alicloud/issues/1651))
- improve(images): modified the testcase of images datasource([#1648](https://github.com/aliyun/terraform-provider-alicloud/issues/1648))
- improve(security_group_id):update description to support for modify([#1647](https://github.com/aliyun/terraform-provider-alicloud/issues/1647))
- impove(slb):add new allowed spec for slb([#1646](https://github.com/aliyun/terraform-provider-alicloud/issues/1646))
- improve(provider):support ecs_role_name + assume_role([#1639](https://github.com/aliyun/terraform-provider-alicloud/issues/1639))
- improve(example): update the examples to the format of terraform version 0.12([#1633](https://github.com/aliyun/terraform-provider-alicloud/issues/1633))
- improve(instance):remove bandwidth limit([#1630](https://github.com/aliyun/terraform-provider-alicloud/issues/1630))
- improve(gpdb): gpdb instance supported tags([#1615](https://github.com/aliyun/terraform-provider-alicloud/issues/1615))

BUG FIXES:

- fix(security_group):fix security_group bug([#1640](https://github.com/aliyun/terraform-provider-alicloud/issues/1640))
- fix(rds): add diffsuppressfunc to rds tags([#1602](https://github.com/aliyun/terraform-provider-alicloud/issues/1602))

## 1.55.3 (September 09, 2019)

IMPROVEMENTS:

- improve(slb): midified the sweep rules of slb([#1631](https://github.com/aliyun/terraform-provider-alicloud/issues/1631))
- improve(slb): add new field resource_group_id([#1629](https://github.com/aliyun/terraform-provider-alicloud/issues/1629))
- improve(example): update the examples to the format of the new version([#1625](https://github.com/aliyun/terraform-provider-alicloud/issues/1625))
- improve(api gateway): api gateway app supported tags([#1622](https://github.com/aliyun/terraform-provider-alicloud/issues/1622))
- improve(vpc): vpc resources and datasources supported tags([#1621](https://github.com/aliyun/terraform-provider-alicloud/issues/1621))
- improve(kvstore): kvstore instance supported tags([#1619](https://github.com/aliyun/terraform-provider-alicloud/issues/1619))
- update example to support for snat's creation with multi eips([#1554](https://github.com/aliyun/terraform-provider-alicloud/issues/1554))

BUG FIXES:

- fix(common_bandwidth_package):make ratio ForceNew([#1626](https://github.com/aliyun/terraform-provider-alicloud/issues/1626))
- fix(disk):fix disk detach bug([#1610](https://github.com/aliyun/terraform-provider-alicloud/issues/1610))
- fix:resource security_group 'inner_access_policy' replaces 'inner_access',resource slb 'address_type' replaces 'internet'([#1594](https://github.com/aliyun/terraform-provider-alicloud/issues/1594))

## 1.55.2 (August 30, 2019)

IMPROVEMENTS:

- improve(elasticsearch): modified availability zone of elasticsearch instance.([#1617](https://github.com/aliyun/terraform-provider-alicloud/issues/1617))
- improve(ram & actiontrail): added precheck for resources testcases.([#1616](https://github.com/aliyun/terraform-provider-alicloud/issues/1616))
- improve(cdn): cdn domain supported tags.([#1609](https://github.com/aliyun/terraform-provider-alicloud/issues/1609))
- improve(db_readonly_instance):improve db_readonly_instance testcase([#1607](https://github.com/aliyun/terraform-provider-alicloud/issues/1607))
- improve(cdn) modified wait time of cdn domain creation.([#1606](https://github.com/aliyun/terraform-provider-alicloud/issues/1606))
- improve(drds): modified drds supported regions([#1605](https://github.com/aliyun/terraform-provider-alicloud/issues/1605))
- improve(CI): change sweeper time([#1600](https://github.com/aliyun/terraform-provider-alicloud/issues/1600))
- improve(rds): fix db_instance apply error after import([#1599](https://github.com/aliyun/terraform-provider-alicloud/issues/1599))
- improve(ons_topic):retry when Throttling.User([#1598](https://github.com/aliyun/terraform-provider-alicloud/issues/1598))
- Improve(ddoscoo): Improve its resource and datasource use common method([#1591](https://github.com/aliyun/terraform-provider-alicloud/issues/1591))
- Improve(slb):slb support set AddressIpVersion([#1587](https://github.com/aliyun/terraform-provider-alicloud/issues/1587))
- Improve(cs_kubernetes): Improve its resource and datasource use common method([#1584](https://github.com/aliyun/terraform-provider-alicloud/issues/1584))
- Improve(cs_managed_kubernetes): Improve its resource and datasource use common method([#1581](https://github.com/aliyun/terraform-provider-alicloud/issues/1581))

BUG FIXES:

- fix(ons):fix ons error Throttling.User([#1608](https://github.com/aliyun/terraform-provider-alicloud/issues/1608))
- fix(ons): fix the create group error in testcase([#1604](https://github.com/aliyun/terraform-provider-alicloud/issues/1604))

## 1.55.1 (August 23, 2019)

IMPROVEMENTS:

- improve(ons_instance): set instance name using random([#1597](https://github.com/aliyun/terraform-provider-alicloud/issues/1597))
- add support to Ipsec_pfs field be set with "disabled" and add example files([#1589](https://github.com/aliyun/terraform-provider-alicloud/issues/1589))
- improve(slb): sweep the protected slb([#1588](https://github.com/aliyun/terraform-provider-alicloud/issues/1588))
- Improve(ram): ram resources supports import([#1586](https://github.com/aliyun/terraform-provider-alicloud/issues/1586))
- improve(tags): modified test case to check the upper case letters in tags([#1585](https://github.com/aliyun/terraform-provider-alicloud/issues/1585))
- improve(Document):improve document demo about set([#1580](https://github.com/aliyun/terraform-provider-alicloud/issues/1580))
- Update RouteEntry Resource RouteEntryName Field([#1578](https://github.com/aliyun/terraform-provider-alicloud/issues/1578))
- improve(ci):supplement log([#1577](https://github.com/aliyun/terraform-provider-alicloud/issues/1577))
- improve(sdk):update alibaba-cloud-sdk-go(1.60.107)([#1575](https://github.com/aliyun/terraform-provider-alicloud/issues/1575))
- Rename resource name that is not start with a letter([#1573](https://github.com/aliyun/terraform-provider-alicloud/issues/1573))
- Improve(datahub_topic): Improve resource use common method([#1565](https://github.com/aliyun/terraform-provider-alicloud/issues/1565))
- Improve(datahub_subscription): Improve resource use common method([#1556](https://github.com/aliyun/terraform-provider-alicloud/issues/1556))
- Improve(datahub_project): Improve resource use common method([#1555](https://github.com/aliyun/terraform-provider-alicloud/issues/1555))

BUG FIXES:

- fix(vsw): fix bug from GitHub issue([#1593](https://github.com/aliyun/terraform-provider-alicloud/issues/1593))
- fix(instance):update instance testcase([#1590](https://github.com/aliyun/terraform-provider-alicloud/issues/1590))
- fix(ci):fix CI statistics bug([#1576](https://github.com/aliyun/terraform-provider-alicloud/issues/1576))
- Fix typo([#1574](https://github.com/aliyun/terraform-provider-alicloud/issues/1574))
- fix(disks):fix dataSource test case bug([#1566](https://github.com/aliyun/terraform-provider-alicloud/issues/1566))

## 1.55.0 (August 16, 2019)

- **New Resource:** `alicloud_ess_notification`([#1549](https://github.com/aliyun/terraform-provider-alicloud/issues/1549))

IMPROVEMENTS:

- improve(key_pair):update key_pair document([#1563](https://github.com/aliyun/terraform-provider-alicloud/issues/1563))
- improve(CI): add default bucket and region for CI([#1561](https://github.com/aliyun/terraform-provider-alicloud/issues/1561))
- improve(CI): terraform CI log([#1557](https://github.com/aliyun/terraform-provider-alicloud/issues/1557))
- Improve(ots_instance_attachment): Improve its resource and datasource use common method([#1552](https://github.com/aliyun/terraform-provider-alicloud/issues/1552))
- Improve(ots_instance): Improve its resource and datasource use common method([#1551](https://github.com/aliyun/terraform-provider-alicloud/issues/1551))
- Improve(ram): ram policy attachment resources supports import([#1550](https://github.com/aliyun/terraform-provider-alicloud/issues/1550))
- Improve(ots_table): Improve its resource and datasource use common method([#1546](https://github.com/aliyun/terraform-provider-alicloud/issues/1546))
- Improve(router_interface): modified testcase multi count([#1545](https://github.com/aliyun/terraform-provider-alicloud/issues/1545))
- Improve(images): removed image alinux check in datasource([#1543](https://github.com/aliyun/terraform-provider-alicloud/issues/1543))
- Improve(logtail_config): Improve resource use common method([#1500](https://github.com/aliyun/terraform-provider-alicloud/issues/1500))

BUG FIXES:

- bugfix：throw notFoundError when scalingGroup is not found([#1572](https://github.com/aliyun/terraform-provider-alicloud/issues/1572))
- fix(sweep): modified the error return to run sweep completely([#1569](https://github.com/aliyun/terraform-provider-alicloud/issues/1569))
- fix(CI): remove the useless code([#1564](https://github.com/aliyun/terraform-provider-alicloud/issues/1564))
- fix(CI): fix pipeline grammar error([#1562](https://github.com/aliyun/terraform-provider-alicloud/issues/1562))
- Fix log document([#1559](https://github.com/aliyun/terraform-provider-alicloud/issues/1559))
- modify(cs): skip the testcases of cs_application and cs_swarm([#1553](https://github.com/aliyun/terraform-provider-alicloud/issues/1553))
- fix kvstore unexpected state 'Changing'([#1539](https://github.com/aliyun/terraform-provider-alicloud/issues/1539))

## 1.54.0 (August 12, 2019)

- **New Data Source:** `alicloud_slb_master_slave_server_groups`([#1531](https://github.com/aliyun/terraform-provider-alicloud/issues/1531))
- **New Resource:** `alicloud_slb_master_slave_server_group`([#1531](https://github.com/aliyun/terraform-provider-alicloud/issues/1531))
- **New Data Source:** `alicloud_instance_type_families`([#1519](https://github.com/aliyun/terraform-provider-alicloud/issues/1519))

IMPROVEMENTS:

- improve(provider):profile,role_arn,session_name,session_expiration support ENV([#1537](https://github.com/aliyun/terraform-provider-alicloud/issues/1537))
- support sg description([#1536](https://github.com/aliyun/terraform-provider-alicloud/issues/1536))
- support mac address([#1535](https://github.com/aliyun/terraform-provider-alicloud/issues/1535))
- improve(sdk): update sdk and modify api_gateway strconv([#1533](https://github.com/aliyun/terraform-provider-alicloud/issues/1533))
- Improve(pvtz_zone_record): Improve resource use common method([#1528](https://github.com/aliyun/terraform-provider-alicloud/issues/1528))
- improve(alicloud_ess_scaling_group): support 'COST_OPTIMIZED' mode of autoscaling group([#1527](https://github.com/aliyun/terraform-provider-alicloud/issues/1527))
- Improve(pvtz_zone): Improve its and attachment resources use common method([#1525](https://github.com/aliyun/terraform-provider-alicloud/issues/1525))
- remove useless trigger in vpn ci([#1522](https://github.com/aliyun/terraform-provider-alicloud/issues/1522))
- Improve(cr_repo): Improve resource use common method([#1515](https://github.com/aliyun/terraform-provider-alicloud/issues/1515))
- Improve(cr_namespace): Improve resource use common method([#1509](https://github.com/aliyun/terraform-provider-alicloud/issues/1509))
- improve(kvstore): kvstore_instance resource supports timeouts setting([#1445](https://github.com/aliyun/terraform-provider-alicloud/issues/1445))

BUG FIXES:

- Fix(alicloud_logstore_index) Repair parameter description document([#1532](https://github.com/aliyun/terraform-provider-alicloud/issues/1532))
- fix(sweep): modified the region of prefixes([#1526](https://github.com/aliyun/terraform-provider-alicloud/issues/1526))
- fix(mongodb_instance): fix notfound error when describing it([#1521](https://github.com/aliyun/terraform-provider-alicloud/issues/1521))

## 1.53.0 (August 02, 2019)

- **New Resource:** `alicloud_ons_group`([#1506](https://github.com/aliyun/terraform-provider-alicloud/issues/1506))
- **New Resource:** `alicloud_ess_scalinggroup_vserver_groups`([#1503](https://github.com/aliyun/terraform-provider-alicloud/issues/1503))
- **New Resource:** `alicloud_slb_backend_server`([#1498](https://github.com/aliyun/terraform-provider-alicloud/issues/1498))
- **New Resource:** `alicloud_ons_topic`([#1483](https://github.com/aliyun/terraform-provider-alicloud/issues/1483))
- **New Data Source:** `alicloud_ons_groups`([#1506](https://github.com/aliyun/terraform-provider-alicloud/issues/1506))
- **New Data source:** `alicloud_slb_backend_servers`([#1498](https://github.com/aliyun/terraform-provider-alicloud/issues/1498))
- **New Data Source:** `alicloud_ons_topics`([#1483](https://github.com/aliyun/terraform-provider-alicloud/issues/1483))


IMPROVEMENTS:

- improve(dns_record): add diffsuppressfunc to avoid DomainRecordDuplicate error.([#1518](https://github.com/aliyun/terraform-provider-alicloud/issues/1518))
- remove useless import([#1517](https://github.com/aliyun/terraform-provider-alicloud/issues/1517))
- remove empty fields in managed k8s, add force_update, add multiple az support([#1516](https://github.com/aliyun/terraform-provider-alicloud/issues/1516))
- improve(fc_function):fc_function support sweeper([#1513](https://github.com/aliyun/terraform-provider-alicloud/issues/1513))
- improve(fc_trigger):fc_trigger support sweeper([#1512](https://github.com/aliyun/terraform-provider-alicloud/issues/1512))
- Improve(logtail_attachment): Improve resource use common method([#1508](https://github.com/aliyun/terraform-provider-alicloud/issues/1508)) 
- improve(slb):update testcase([#1507](https://github.com/aliyun/terraform-provider-alicloud/issues/1507))
- improve(disk):update disk_attachment([#1501](https://github.com/aliyun/terraform-provider-alicloud/issues/1501))
- add(slb_backend_server): slb backend server resource & data source([#1498](https://github.com/aliyun/terraform-provider-alicloud/issues/1498))
- Improve(log_machine_group): Improve resources use common method([#1497](https://github.com/aliyun/terraform-provider-alicloud/issues/1497))
- Improve(log_project): Improve resource use common method([#1496](https://github.com/aliyun/terraform-provider-alicloud/issues/1496))
- improve(network_interface): enhance sweeper test([#1495](https://github.com/aliyun/terraform-provider-alicloud/issues/1495))
- Improve(log_store): Improve resources use common method([#1494](https://github.com/aliyun/terraform-provider-alicloud/issues/1494))
- improve(instance_type):update testcase config([#1493](https://github.com/aliyun/terraform-provider-alicloud/issues/1493))
- Improve(mns_topic_subscription): Improve its resource use common method([#1492](https://github.com/aliyun/terraform-provider-alicloud/issues/1492))
- improve(disk):support delete_auto_snapshot delete_with_instance enable_auto_snapshot([#1491](https://github.com/aliyun/terraform-provider-alicloud/issues/1491))
- Improve(mns_topic): Improve its resource use common method([#1488](https://github.com/aliyun/terraform-provider-alicloud/issues/1488))
- Improve(api_gateway): api_gateway_api added testcases([#1487](https://github.com/aliyun/terraform-provider-alicloud/issues/1487))
- Improve(mns_queue): Improve its resource use common method([#1485](https://github.com/aliyun/terraform-provider-alicloud/issues/1485))
- improve(customer_gateway):create add retry([#1477](https://github.com/aliyun/terraform-provider-alicloud/issues/1477))
- improve(gpdb): resources supports timeouts setting([#1476](https://github.com/aliyun/terraform-provider-alicloud/issues/1476))
- improve(fc_triggers): Added ids filter to datasource([#1475](https://github.com/aliyun/terraform-provider-alicloud/issues/1475))
- improve(fc_services): Added ids filter to datasource([#1474](https://github.com/aliyun/terraform-provider-alicloud/issues/1474))
- improve(fc_functions): Added ids filter to datasource([#1473](https://github.com/aliyun/terraform-provider-alicloud/issues/1473))
- improve(instance_types):update instance_types filter condition([#1472](https://github.com/aliyun/terraform-provider-alicloud/issues/1472))
- improve(pvtz_zone__domain): Added ids filter to datasource([#1471](https://github.com/aliyun/terraform-provider-alicloud/issues/1471))
- improve(cr_repos): Added names to datasource attributes([#1470](https://github.com/aliyun/terraform-provider-alicloud/issues/1470))
- improve(cr_namespaces): Added names to datasource attributes([#1469](https://github.com/aliyun/terraform-provider-alicloud/issues/1469))
- improve(cdn): Added region to domain name and modified sweep rules([#1466](https://github.com/aliyun/terraform-provider-alicloud/issues/1466))
- improve(ram_roles): Added ids filter to datasource([#1461](https://github.com/aliyun/terraform-provider-alicloud/issues/1461))
- improve(ram_users): Added ids filter to datasource([#1459](https://github.com/aliyun/terraform-provider-alicloud/issues/1459))
- improve(pvtz_zones): Added ids filter and added names to datasource attributes([#1458](https://github.com/aliyun/terraform-provider-alicloud/issues/1458))
- improve(nas_mount_targets): Added ids filter to datasource([#1453](https://github.com/aliyun/terraform-provider-alicloud/issues/1453))
- improve(nas_file_systems): Added descriptions to datasource attributes([#1450](https://github.com/aliyun/terraform-provider-alicloud/issues/1450))
- improve(nas_access_rules): Added ids filter to datasource([#1448](https://github.com/aliyun/terraform-provider-alicloud/issues/1448))
- improve(mongodb_instance): supports timeouts setting([#1446](https://github.com/aliyun/terraform-provider-alicloud/issues/1446))
- improve(nas_access_groups): Added names to its attributes([#1444](https://github.com/aliyun/terraform-provider-alicloud/issues/1444))
- improve(mns_topics): Added names to datasource attributes([#1442](https://github.com/aliyun/terraform-provider-alicloud/issues/1442))
- improve(mns_topic_subscriptions): Added names to datasource attributes([#1441](https://github.com/aliyun/terraform-provider-alicloud/issues/1441))
- improve(mns_queues): Added names to datasource attributes([#1439](https://github.com/aliyun/terraform-provider-alicloud/issues/1439))

BUG FIXES:

- Fix(logstore_index): Invalid update parameter change([#1505](https://github.com/aliyun/terraform-provider-alicloud/issues/1505))
- fix(api_gateway): fix can't get resource id when stage_names set([#1486](https://github.com/aliyun/terraform-provider-alicloud/issues/1486))
- fix(kvstore_instance): resource kvstore_instance add Retry while ModifyInstanceSpec err([#1484](https://github.com/aliyun/terraform-provider-alicloud/issues/1484))
- fix(cen): modified the timeouts of cen instance to avoid errors([#1451](https://github.com/aliyun/terraform-provider-alicloud/issues/1451))

## 1.52.2 (July 20, 2019)

IMPROVEMENTS:

- improve(eip_association): supporting to set PrivateIPAddress  documentation([#1480](https://github.com/aliyun/terraform-provider-alicloud/issues/1480))
- improve(mongodb_instances): Added ids filter to datasource([#1478](https://github.com/aliyun/terraform-provider-alicloud/issues/1478))
- improve(dns_domain): Added ids filter to datasource([#1468](https://github.com/aliyun/terraform-provider-alicloud/issues/1468))
- improve(cdn): Added retry to avoid ServiceBusy error([#1467](https://github.com/aliyun/terraform-provider-alicloud/issues/1467))
- improve(dns_records): Added ids filter to datasource([#1464](https://github.com/aliyun/terraform-provider-alicloud/issues/1464))
- improve(dns_groups): Added ids filter and added names to datasource attributes([#1463](https://github.com/aliyun/terraform-provider-alicloud/issues/1463))
- improve(stateConfig):update stateConfig error([#1462](https://github.com/aliyun/terraform-provider-alicloud/issues/1462))
- improve(kvstore): Added ids filter to datasource([#1457](https://github.com/aliyun/terraform-provider-alicloud/issues/1457))
- improve(cas): Added precheck to testcases([#1456](https://github.com/aliyun/terraform-provider-alicloud/issues/1456))
- improve(rds): db_instance and db_readonly_instance resource modify timeouts 20mins to 30mins([#1455](https://github.com/aliyun/terraform-provider-alicloud/issues/1455))
- add CI for the alicloud provider([#1449](https://github.com/aliyun/terraform-provider-alicloud/issues/1449))
- improve(api_gateway_apps): Deprecated api_id([#1426](https://github.com/aliyun/terraform-provider-alicloud/issues/1426))
- improve(api_gateway_apis): Added ids filter to datasource([#1425](https://github.com/aliyun/terraform-provider-alicloud/issues/1425))
- improve(slb_server_group): remove the maximum limitation of adding backend servers([#1416](https://github.com/aliyun/terraform-provider-alicloud/issues/1416))
- improve(cdn): cdn_domain_config added testcases([#1405](https://github.com/aliyun/terraform-provider-alicloud/issues/1405))

BUG FIXES:

- fix(kvstore_instance): resource kvstore_instance add Retry while ModifyInstanceSpec err([#1465](https://github.com/aliyun/terraform-provider-alicloud/issues/1465))
- fix(slb): fix slb testcase can not find instance types' bug([#1454](https://github.com/aliyun/terraform-provider-alicloud/issues/1454))

## 1.52.1 (July 16, 2019)

IMPROVEMENTS:

- improve(disk): support online resize([#1447](https://github.com/aliyun/terraform-provider-alicloud/issues/1447))
- improve(rds): db_readonly_instance resource supports timeouts setting([#1438](https://github.com/aliyun/terraform-provider-alicloud/issues/1438))
- improve(rds):improve db_readonly_instance TestAccAlicloudDBReadonlyInstance_multi testcase([#1432](https://github.com/aliyun/terraform-provider-alicloud/issues/1432))
- improve(key_pairs): Added ids filter to datasource([#1431](https://github.com/aliyun/terraform-provider-alicloud/issues/1431))
- improve(elasticsearch): Added ids filter and added descriptions to datasource attributes([#1430](https://github.com/aliyun/terraform-provider-alicloud/issues/1430))
- improve(drds): Added descriptions to attributes of datasource([#1429](https://github.com/aliyun/terraform-provider-alicloud/issues/1429))
- improve(rds):update ppas not support regions([#1428](https://github.com/aliyun/terraform-provider-alicloud/issues/1428))
- improve(api_gateway_groups): Added ids filter to datasource([#1427](https://github.com/aliyun/terraform-provider-alicloud/issues/1427))
- improve(docs): Reformat abnormal inline HCL code in docs([#1423](https://github.com/aliyun/terraform-provider-alicloud/issues/1423))
- improve(mns):modified mns_queues.html([#1422](https://github.com/aliyun/terraform-provider-alicloud/issues/1422))
- improve(rds): db_instance resource supports timeouts setting([#1409](https://github.com/aliyun/terraform-provider-alicloud/issues/1409))
- improve(kms): modified the args of kms_keys datasource([#1407](https://github.com/aliyun/terraform-provider-alicloud/issues/1407))
- improve(kms_key): modify the param `description` to forcenew([#1406](https://github.com/aliyun/terraform-provider-alicloud/issues/1406))

BUG FIXES:

- fix(db_instance): modified the target state of state config([#1437](https://github.com/aliyun/terraform-provider-alicloud/issues/1437))
- fix(db_readonly_instance): fix invalid status error when updating and deleting([#1435](https://github.com/aliyun/terraform-provider-alicloud/issues/1435))
- fix(ots_table): fix setting deviation_cell_version_in_sec error([#1434](https://github.com/aliyun/terraform-provider-alicloud/issues/1434))
- fix(db_backup_policy): resource db_backup_policy testcase use datasource db_instance_classes([#1424](https://github.com/aliyun/terraform-provider-alicloud/issues/1424))

## 1.52.0 (July 12, 2019)

- **New Datasource:** `alicloud_ons_instances`([#1411](https://github.com/aliyun/terraform-provider-alicloud/issues/1411))

IMPROVEMENTS:

- improve(vpc):add ids filter([#1420](https://github.com/aliyun/terraform-provider-alicloud/issues/1420))
- improve(db_instances): Added ids filter and added names to datasource attributes([#1419](https://github.com/aliyun/terraform-provider-alicloud/issues/1419))
- improve(cas): Added ids filter and added names to datasource attributes([#1417](https://github.com/aliyun/terraform-provider-alicloud/issues/1417))
- docs(format): Convert inline HCL configs to canonical format([#1415](https://github.com/aliyun/terraform-provider-alicloud/issues/1415))
- improve(gpdb_instance):add vpc name([#1413](https://github.com/aliyun/terraform-provider-alicloud/issues/1413))
- improve(provider): add a new parameter `skip_region_validation` in the provider config([#1404](https://github.com/aliyun/terraform-provider-alicloud/issues/1404))
- improve(cdn): cdn_domain support certificate config([#1393](https://github.com/aliyun/terraform-provider-alicloud/issues/1393))
- improve(rds): resource db_instance support update for instance_charge_type([#1389](https://github.com/aliyun/terraform-provider-alicloud/issues/1389))

BUG FIXES:

- fix(db_instance):fix db_instance testcase vsw availability_zone([#1418](https://github.com/aliyun/terraform-provider-alicloud/issues/1418))
- fix(api_gateway): modified the testcase to avoid errors([#1410](https://github.com/aliyun/terraform-provider-alicloud/issues/1410))
- fix(db_readonly_instance): extend the waiting time for spec modification([#1408](https://github.com/aliyun/terraform-provider-alicloud/issues/1408))
- fix(db_readonly_instance): add retryable error content in instance spec modification and deletion([#1403](https://github.com/aliyun/terraform-provider-alicloud/issues/1403))

## 1.51.0 (July 08, 2019)

- **New Date Source:** `alicloud_kvstore_instance_engines`([#1371](https://github.com/aliyun/terraform-provider-alicloud/issues/1371))
- **New Resource:** `alicloud_ons_instance`([#1333](https://github.com/aliyun/terraform-provider-alicloud/issues/1333))

IMPROVEMENTS:

- improve(db_instance): improve db_instance MAZ testcase([#1391](https://github.com/aliyun/terraform-provider-alicloud/issues/1391))
- improve(cs_kubernetes): add importIgnore parameters in the importer testcase([#1387](https://github.com/aliyun/terraform-provider-alicloud/issues/1387))
- Remove govendor commands in CI([#1386](https://github.com/aliyun/terraform-provider-alicloud/issues/1386))
- improve(slb_vserver_group): support attaching eni([#1384](https://github.com/aliyun/terraform-provider-alicloud/issues/1384))
- improve(db_instance_classes): add new parameter db_instance_class([#1383](https://github.com/aliyun/terraform-provider-alicloud/issues/1383))
- improve(images): Add os_name_en to the attributes of images datasource([#1380](https://github.com/aliyun/terraform-provider-alicloud/issues/1380))
- improve(disk): the snapshot_id conflicts with encrypted([#1378](https://github.com/aliyun/terraform-provider-alicloud/issues/1378))
- Improve(cs_kubernetes): add some importState ignore fields in the importer testcase([#1377](https://github.com/aliyun/terraform-provider-alicloud/issues/1377))
- Improve(oss_bucket): Add names for its attributes of datasource([#1374](https://github.com/aliyun/terraform-provider-alicloud/issues/1374))
- improve(common_test):update common_test for terraform 0.12([#1372](https://github.com/aliyun/terraform-provider-alicloud/issues/1372))
- Improve(cs_kubernetes): add import ignore parameter `log_config`([#1370](https://github.com/aliyun/terraform-provider-alicloud/issues/1370))
- improve(slb):support slb instance delete protection([#1369](https://github.com/aliyun/terraform-provider-alicloud/issues/1369))
- improve(slb_rule): support health check config([#1367](https://github.com/aliyun/terraform-provider-alicloud/issues/1367))
- Improve(oss_bucket_object): Improve its use common method([#1366](https://github.com/aliyun/terraform-provider-alicloud/issues/1366))
- improve(drds_instance): Added precheck to its testcases([#1364](https://github.com/aliyun/terraform-provider-alicloud/issues/1364))
- Improve(oss_bucket): Improve its resource use common method([#1353](https://github.com/aliyun/terraform-provider-alicloud/issues/1353))
- improve(launch_template): support update method([#1327](https://github.com/aliyun/terraform-provider-alicloud/issues/1327))
- improve(snapshot): support setting timeouts([#1304](https://github.com/aliyun/terraform-provider-alicloud/issues/1304))
- improve(instance):update testcase([#1199](https://github.com/aliyun/terraform-provider-alicloud/issues/1199))

BUG FIXES:

- fix(instance): fix missing dry_run when creating instance([#1401](https://github.com/aliyun/terraform-provider-alicloud/issues/1401))
- fix(oss_bucket): fix oss bucket deleting timeout error([#1400](https://github.com/aliyun/terraform-provider-alicloud/issues/1400))
- fix(route_entry):fix route_entry create bug([#1398](https://github.com/aliyun/terraform-provider-alicloud/issues/1398))
- fix(instance):fix testcase name too length bug([#1396](https://github.com/aliyun/terraform-provider-alicloud/issues/1396))
- fix(vswitch):fix vswitch describe method wrapErrorf bug([#1392](https://github.com/aliyun/terraform-provider-alicloud/issues/1392))
- fix(slb_rule): fix testcase bug([#1390](https://github.com/aliyun/terraform-provider-alicloud/issues/1390))
- fix(db_backup_policy): pg10 of category 'basic' modify log_backup error([#1388](https://github.com/aliyun/terraform-provider-alicloud/issues/1388))
- fix(cen):Add deadline to cen datasources and modify timeout for DescribeCenBandwidthPackages([#1381](https://github.com/aliyun/terraform-provider-alicloud/issues/1381))
- fix(kvstore): kvstore_instance PostPaid to PrePaid error([#1375](https://github.com/aliyun/terraform-provider-alicloud/issues/1375))
- fix(cen): fixed its not display error message, added CenThrottlingUser retry([#1373](https://github.com/aliyun/terraform-provider-alicloud/issues/1373))

## 1.50.0 (July 01, 2019)

IMPROVEMENTS:

- Remove cs kubernetes autovpc testcases([#1368](https://github.com/aliyun/terraform-provider-alicloud/issues/1368))
- disable nav-visible in the alicloud.erb file([#1365](https://github.com/aliyun/terraform-provider-alicloud/issues/1365))
- Improve sweeper test and remove some needless waiting([#1361](https://github.com/aliyun/terraform-provider-alicloud/issues/1361))
- This is a Terraform 0.12 compatible release of this provider([#1356](https://github.com/aliyun/terraform-provider-alicloud/issues/1356))
- Deprecated resource `alicloud_cms_alarm` parameter start_time, end_time and removed notify_type based on the latest go sdk([#1356](https://github.com/aliyun/terraform-provider-alicloud/issues/1356))
- Adapt to new parameters of dedicated kubernetes cluster([#1354](https://github.com/aliyun/terraform-provider-alicloud/issues/1354))

BUG FIXES:

- Fix alicloud_cas_certificate setId bug([#1368](https://github.com/aliyun/terraform-provider-alicloud/issues/1368))
- Fix oss bucket datasource testcase based on the 0.12 syntax([#1362](https://github.com/aliyun/terraform-provider-alicloud/issues/1362))
- Fix deleting mongodb instance "NotFound" bug([#1359](https://github.com/aliyun/terraform-provider-alicloud/issues/1359))

## 1.49.0 (June 28, 2019)

- **New Date Source:** `alicloud_kvstore_instance_classes`([#1315](https://github.com/aliyun/terraform-provider-alicloud/issues/1315))

IMPROVEMENTS:

- remove the skipped testcase([#1349](https://github.com/aliyun/terraform-provider-alicloud/issues/1349))
- Move some import testcase into resource testcase([#1348](https://github.com/aliyun/terraform-provider-alicloud/issues/1348))
- Support attach & detach operation for loadbalancers and dbinstances([#1346](https://github.com/aliyun/terraform-provider-alicloud/issues/1346))
- update security_group_rule md([#1345](https://github.com/aliyun/terraform-provider-alicloud/issues/1345))
- Improve mongodb,rds testcase([#1339](https://github.com/aliyun/terraform-provider-alicloud/issues/1339))
- Deprecate field statement and use field document to replace([#1338](https://github.com/aliyun/terraform-provider-alicloud/issues/1338))
- Add function BuildStateConf for common timeouts setting([#1330](https://github.com/aliyun/terraform-provider-alicloud/issues/1330))
- drds_instance resource supports timeouts setting([#1329](https://github.com/aliyun/terraform-provider-alicloud/issues/1329))
- add support get Ak from config file([#1328](https://github.com/aliyun/terraform-provider-alicloud/issues/1328))
- Improve api_gateway_vpc use common method.([#1323](https://github.com/aliyun/terraform-provider-alicloud/issues/1323))
- Organize official documents in alphabetical order([#1322](https://github.com/aliyun/terraform-provider-alicloud/issues/1322))
- improve snapshot_policy testcase([#1313](https://github.com/aliyun/terraform-provider-alicloud/issues/1313))
- Improve api_gateway_group use common method([#1311](https://github.com/aliyun/terraform-provider-alicloud/issues/1311))
- Improve api_gateway_app use common method([#1306](https://github.com/aliyun/terraform-provider-alicloud/issues/1306))

BUG FIXES:

- bugfix: modify ess loadbalancers batch size([#1352](https://github.com/aliyun/terraform-provider-alicloud/issues/1352))
- fix instance OperationConflict bug([#1351](https://github.com/aliyun/terraform-provider-alicloud/issues/1351))
- fix(nas): convert some retrable error to nonretryable([#1344](https://github.com/aliyun/terraform-provider-alicloud/issues/1344))
- fix mongodb testcase([#1341](https://github.com/aliyun/terraform-provider-alicloud/issues/1341))
- fix log_store fields cannot be changed([#1337](https://github.com/aliyun/terraform-provider-alicloud/issues/1337))
- fix(nas): fix error handling([#1336](https://github.com/aliyun/terraform-provider-alicloud/issues/1336))
- fix db_instance_classes,db_instance_engines([#1331](https://github.com/aliyun/terraform-provider-alicloud/issues/1331))
- fix sls-logconfig config_name field to name([#1326](https://github.com/aliyun/terraform-provider-alicloud/issues/1326))
- fix db_instance_engines testcase([#1325](https://github.com/aliyun/terraform-provider-alicloud/issues/1325))
- fix forward_entries testcase bug([#1324](https://github.com/aliyun/terraform-provider-alicloud/issues/1324))

## 1.48.0 (June 21, 2019)

- **New Resource:** `alicloud_gpdb_connection`([#1290](https://github.com/aliyun/terraform-provider-alicloud/issues/1290))

IMPROVEMENTS:

- Improve rds testcase zone_id([#1321](https://github.com/aliyun/terraform-provider-alicloud/issues/1321))
- feature: support enable/disable action for resource alicloud_ess_alarm([#1320](https://github.com/aliyun/terraform-provider-alicloud/issues/1320))
- cen_instance resource supports timeouts setting([#1318](https://github.com/aliyun/terraform-provider-alicloud/issues/1318))
- added importer support for security_group_rule([#1317](https://github.com/aliyun/terraform-provider-alicloud/issues/1317))
- add multi_zone for db_instance_classes and db_instance_engines([#1310](https://github.com/aliyun/terraform-provider-alicloud/issues/1310))
- Update Eip Resource Isp Field([#1303](https://github.com/aliyun/terraform-provider-alicloud/issues/1303))
- Improve db_instance,db_read_write_splitting_connection,db_readonly_instance testcase([#1300](https://github.com/aliyun/terraform-provider-alicloud/issues/1300))
- Improve api_gateway_api use common method([#1299](https://github.com/aliyun/terraform-provider-alicloud/issues/1299))
- Add name for cen bandwidth package testcase([#1298](https://github.com/aliyun/terraform-provider-alicloud/issues/1298))
- Improve db testcase([#1294](https://github.com/aliyun/terraform-provider-alicloud/issues/1294))
- elasticsearch_instance resource supports timeouts setting([#1268](https://github.com/aliyun/terraform-provider-alicloud/issues/1268))

BUG FIXES:

- bugfix: remove the 'ForceNew' attribute of 'vswitch_ids' from resource alicloud_ess_scaling_group([#1316](https://github.com/aliyun/terraform-provider-alicloud/issues/1316))
- managed k8s no longer returns vswitchids and instancetypes, fix crash([#1314](https://github.com/aliyun/terraform-provider-alicloud/issues/1314))
- fix db_instance_classes([#1309](https://github.com/aliyun/terraform-provider-alicloud/issues/1309))
- fix oss lifecycle nil pointer bug([#1307](https://github.com/aliyun/terraform-provider-alicloud/issues/1307))
- Fix cen_bandwidth_limit Throttling.User bug([#1305](https://github.com/aliyun/terraform-provider-alicloud/issues/1305))
- fix disk_attachment test bug([#1302](https://github.com/aliyun/terraform-provider-alicloud/issues/1302))

## 1.47.0 (June 17, 2019)

- **New Date Source:** `alicloud_gpdb_instances`([#1279](https://github.com/aliyun/terraform-provider-alicloud/issues/1279))
- **New Resource:** `alicloud_gpdb_instance`([#1260](https://github.com/aliyun/terraform-provider-alicloud/issues/1260))

IMPROVEMENTS:

- fc_trigger datasource support outputting ids and names([#1286](https://github.com/aliyun/terraform-provider-alicloud/issues/1286))
- add fc_trigger support cdn_events([#1285](https://github.com/aliyun/terraform-provider-alicloud/issues/1285))
- modify apigateway-fc example([#1284](https://github.com/aliyun/terraform-provider-alicloud/issues/1284))
- Added PGP encrypt Support for ram access key([#1280](https://github.com/aliyun/terraform-provider-alicloud/issues/1280))
- Update Eip Resource Isp Field([#1275](https://github.com/aliyun/terraform-provider-alicloud/issues/1275))
- Improve fc_service use common method([#1269](https://github.com/aliyun/terraform-provider-alicloud/issues/1269))
- Improve fc_function use common method([#1266](https://github.com/aliyun/terraform-provider-alicloud/issues/1266))
- update dns_group testcase name([#1265](https://github.com/aliyun/terraform-provider-alicloud/issues/1265))
- update slb sdk([#1263](https://github.com/aliyun/terraform-provider-alicloud/issues/1263))
- improve vpn_connection testcase([#1257](https://github.com/aliyun/terraform-provider-alicloud/issues/1257))
- Improve cen_route_entries use common method([#1249](https://github.com/aliyun/terraform-provider-alicloud/issues/1249))
- Improve cen_bandwidth_package_attachment resource use common method([#1240](https://github.com/aliyun/terraform-provider-alicloud/issues/1240))
- Improve cen_bandwidth_package resource use common method([#1237](https://github.com/aliyun/terraform-provider-alicloud/issues/1237))

BUG FIXES:

- feat(nas): fix error report([#1293](https://github.com/aliyun/terraform-provider-alicloud/issues/1293))
- temp fix no value returned by cs openapi([#1289](https://github.com/aliyun/terraform-provider-alicloud/issues/1289))
- fix disk device_name bug([#1288](https://github.com/aliyun/terraform-provider-alicloud/issues/1288))
- fix sql server instance storage set bug([#1283](https://github.com/aliyun/terraform-provider-alicloud/issues/1283))
- fix db_instance_classes storage_range bug([#1282](https://github.com/aliyun/terraform-provider-alicloud/issues/1282))
- fc_service datasource support outputting ids and names([#1278](https://github.com/aliyun/terraform-provider-alicloud/issues/1278))
- fix log_store ListShards InternalServerError bug([#1277](https://github.com/aliyun/terraform-provider-alicloud/issues/1277))
- fix slb_listener docs bug([#1276](https://github.com/aliyun/terraform-provider-alicloud/issues/1276))
- fix clientToken bug([#1272](https://github.com/aliyun/terraform-provider-alicloud/issues/1272))
- fix(nas): fix document and nas_access_rules([#1271](https://github.com/aliyun/terraform-provider-alicloud/issues/1271))
- docs(version) Added 6.7 supported and fixed bug of version difference([#1270](https://github.com/aliyun/terraform-provider-alicloud/issues/1270))
- fix(nas): fix documents([#1267](https://github.com/aliyun/terraform-provider-alicloud/issues/1267))
- fix(nas): describe mount target & access rule([#1264](https://github.com/aliyun/terraform-provider-alicloud/issues/1264))

## 1.46.0 (June 10, 2019)

- **New Resource:** `alicloud_ram_account_password_policy`([#1212](https://github.com/aliyun/terraform-provider-alicloud/issues/1212))
- **New Date Source:** `alicloud_db_instance_engines`([#1201](https://github.com/aliyun/terraform-provider-alicloud/issues/1201))
- **New Date Source:** `alicloud_db_instance_classes`([#1201](https://github.com/aliyun/terraform-provider-alicloud/issues/1201))

IMPROVEMENTS:

- refactor(nas): move import to resource([#1254](https://github.com/aliyun/terraform-provider-alicloud/issues/1254))
- Improve ess_scalingconfiguration use common method([#1250](https://github.com/aliyun/terraform-provider-alicloud/issues/1250))
- improve ssl_vpn_client_cert testcase([#1248](https://github.com/aliyun/terraform-provider-alicloud/issues/1248))
- Improve ram_account_password_policy resource use common method([#1247](https://github.com/aliyun/terraform-provider-alicloud/issues/1247))
- add pending status for resource instance when creating([#1245](https://github.com/aliyun/terraform-provider-alicloud/issues/1245))
- resource instance supports timeouts configure([#1244](https://github.com/aliyun/terraform-provider-alicloud/issues/1244))
- added webhook support for alarms([#1243](https://github.com/aliyun/terraform-provider-alicloud/issues/1243))
- improve common test method([#1242](https://github.com/aliyun/terraform-provider-alicloud/issues/1242))
- Update Eip Association Resource([#1238](https://github.com/aliyun/terraform-provider-alicloud/issues/1238))
- improve ssl_vpn_server testcase([#1235](https://github.com/aliyun/terraform-provider-alicloud/issues/1235))
- Improve ess_scalingconfigurations datasource use common method([#1234](https://github.com/aliyun/terraform-provider-alicloud/issues/1234))
- improve vpn_customer_gateway testcase([#1232](https://github.com/aliyun/terraform-provider-alicloud/issues/1232))
- Improve cen_instance_grant use common method([#1230](https://github.com/aliyun/terraform-provider-alicloud/issues/1230))
- improve vpn_gateway testcase([#1229](https://github.com/aliyun/terraform-provider-alicloud/issues/1229))
- Improve cen_bandwidth_limit use common method([#1227](https://github.com/aliyun/terraform-provider-alicloud/issues/1227))
- Feature/support multi instance types([#1226](https://github.com/aliyun/terraform-provider-alicloud/issues/1226))
- Improve ess_attachment use common method([#1225](https://github.com/aliyun/terraform-provider-alicloud/issues/1225))
- Improve ess_alarm use common method([#1218](https://github.com/aliyun/terraform-provider-alicloud/issues/1218))
- Add support for assume_role in provider block([#1217](https://github.com/aliyun/terraform-provider-alicloud/issues/1217))
- Improve cen_instance_attachment resource use common method.([#1216](https://github.com/aliyun/terraform-provider-alicloud/issues/1216))
- add db instance engines and db instance classes data source support([#1201](https://github.com/aliyun/terraform-provider-alicloud/issues/1201))
- Handle alicloud_cs_*_kubernetes resource NotFound error properly([#1191](https://github.com/aliyun/terraform-provider-alicloud/issues/1191))

BUG FIXES:

- fix slb_attachment classic testcase([#1259](https://github.com/aliyun/terraform-provider-alicloud/issues/1259))
- fix oss bucket update bug([#1258](https://github.com/aliyun/terraform-provider-alicloud/issues/1258))
- fix scalingConfiguration is inconsistent with the information that is returned by describe, when the input parameter user_data is base64([#1256](https://github.com/aliyun/terraform-provider-alicloud/issues/1256))
- fix slb_attachment err ObtainIpFail([#1253](https://github.com/aliyun/terraform-provider-alicloud/issues/1253))
- Fix password to comliant with the default password policy([#1241](https://github.com/aliyun/terraform-provider-alicloud/issues/1241))
- fix cr repo details, improve cs and cr docs([#1239](https://github.com/aliyun/terraform-provider-alicloud/issues/1239))
- fix(nas): fix unittest bugs([#1236](https://github.com/aliyun/terraform-provider-alicloud/issues/1236))
- fix slb_ca_certificate err ServiceIsConfiguring([#1233](https://github.com/aliyun/terraform-provider-alicloud/issues/1233))
- fix reset account_password don't work([#1231](https://github.com/aliyun/terraform-provider-alicloud/issues/1231))
- fix(nas): fix testcase errors([#1184](https://github.com/aliyun/terraform-provider-alicloud/issues/1184))

## 1.45.0 (May 29, 2019)

FEATURES:

- **New Resource:** `alicloud_network_acl_entries`([#1208](https://github.com/aliyun/terraform-provider-alicloud/issues/1208))

IMPROVEMENTS:

- update changeLog([#1224](https://github.com/aliyun/terraform-provider-alicloud/issues/1224))
- support oss object versioning([#1121](https://github.com/aliyun/terraform-provider-alicloud/issues/1121))
- update instance dataSource doc([#1215](https://github.com/aliyun/terraform-provider-alicloud/issues/1215))
- update oss buket encryption configuration([#1214](https://github.com/aliyun/terraform-provider-alicloud/issues/1214))
- support oss bucket tags([#1213](https://github.com/aliyun/terraform-provider-alicloud/issues/1213))
- support oss bucket encryption configuration([#1210](https://github.com/aliyun/terraform-provider-alicloud/issues/1210))
- Improve cen_instances use common method([#1206](https://github.com/aliyun/terraform-provider-alicloud/issues/1206))
- support set oss bucket stroage class([#1204](https://github.com/aliyun/terraform-provider-alicloud/issues/1204))
- Improve ess_lifecyclehook resource use common method([#1196](https://github.com/aliyun/terraform-provider-alicloud/issues/1196))
- Improve ess_scalinggroup use common method([#1192](https://github.com/aliyun/terraform-provider-alicloud/issues/1192))
- Improve ess_scheduled_task resource use common method([#1175](https://github.com/aliyun/terraform-provider-alicloud/issues/1175))
- improve route_table testcase([#1109](https://github.com/aliyun/terraform-provider-alicloud/issues/1109))

BUG FIXES:

- fix nat_gateway and network_interface testcase bug([#1211](https://github.com/aliyun/terraform-provider-alicloud/issues/1211))
- Fix ram testcases name length bug([#1205](https://github.com/aliyun/terraform-provider-alicloud/issues/1205))
- fix actiontrail bug([#1203](https://github.com/aliyun/terraform-provider-alicloud/issues/1203))

## 1.44.0 (May 24, 2019)

FEATURES:

- **New Resource:** `alicloud_network_acl_attachment`([#1187](https://github.com/aliyun/terraform-provider-alicloud/issues/1187))

IMPROVEMENTS:

- update CHANGELOG.md([#1209](https://github.com/aliyun/terraform-provider-alicloud/issues/1209))
- Skip instance some testcases to avoid qouta limit([#1195](https://github.com/aliyun/terraform-provider-alicloud/issues/1195))
- Added the multi zone's instance supported([#1194](https://github.com/aliyun/terraform-provider-alicloud/issues/1194))
- remove multi test of ram_account_alias([#1186](https://github.com/aliyun/terraform-provider-alicloud/issues/1186))
- Improve ram_role_attachment resource use common method([#1185](https://github.com/aliyun/terraform-provider-alicloud/issues/1185))
- Improve ess_scalingrule use common method([#1183](https://github.com/aliyun/terraform-provider-alicloud/issues/1183))
- update mongodb instance resource document([#1182](https://github.com/aliyun/terraform-provider-alicloud/issues/1182))
- Improve ram_role resource use common method([#1181](https://github.com/aliyun/terraform-provider-alicloud/issues/1181))
- Correct the oss bucket docs([#1178](https://github.com/aliyun/terraform-provider-alicloud/issues/1178))
- add slb classic not support regions([#1176](https://github.com/aliyun/terraform-provider-alicloud/issues/1176))
- Dev versioning([#1174](https://github.com/aliyun/terraform-provider-alicloud/issues/1174))
- Improve ram_user_policy_attachment resource use common method([#1172](https://github.com/aliyun/terraform-provider-alicloud/issues/1172))
- Improve ram_role_policy_attachment resource use common method([#1171](https://github.com/aliyun/terraform-provider-alicloud/issues/1171))
- improve router_interface testcase([#1170](https://github.com/aliyun/terraform-provider-alicloud/issues/1170))
- Improve ram_policy resource use common method([#1166](https://github.com/aliyun/terraform-provider-alicloud/issues/1166))
- Improve slb_listeners datasource use common method([#1165](https://github.com/aliyun/terraform-provider-alicloud/issues/1165))
- add name attribute for forward_entry([#1164](https://github.com/aliyun/terraform-provider-alicloud/issues/1164))
- Improve ram_group_policy_attachment resource use common method([#1163](https://github.com/aliyun/terraform-provider-alicloud/issues/1163))
- Improve ram_group_membership resource use common method([#1159](https://github.com/aliyun/terraform-provider-alicloud/issues/1159))
- Improve ram_login_profile resource use common method([#1158](https://github.com/aliyun/terraform-provider-alicloud/issues/1158))
- Improve ram_group resource use common method([#1150](https://github.com/aliyun/terraform-provider-alicloud/issues/1150))

BUG FIXES:

- Fix ram_user sweeper([#1200](https://github.com/aliyun/terraform-provider-alicloud/issues/1200))
- Fix ram group import bug([#1198](https://github.com/aliyun/terraform-provider-alicloud/issues/1198))
- fix router_interface dataSource testcase bug([#1197](https://github.com/aliyun/terraform-provider-alicloud/issues/1197))
- fix forward_entry multi testcase bug([#1189](https://github.com/aliyun/terraform-provider-alicloud/issues/1189))
- fix api gw and network acl sweeper test error([#1180](https://github.com/aliyun/terraform-provider-alicloud/issues/1180))
- fix ram user diff bug([#1179](https://github.com/aliyun/terraform-provider-alicloud/issues/1179))
- Fix ram account alias multi testcase bug([#1169](https://github.com/aliyun/terraform-provider-alicloud/issues/1169))

## 1.43.0 (May 17, 2019)

FEATURES:

- **New Resource:** `alicloud_network_acl` (([#1151](https://github.com/aliyun/terraform-provider-alicloud/issues/1151))

IMPROVEMENTS:

- change ecs instance instance_charge_type modifying position([#1168](https://github.com/aliyun/terraform-provider-alicloud/issues/1168))
- AutoScaling support multiple security groups([#1167](https://github.com/aliyun/terraform-provider-alicloud/issues/1167))
- Update ots and vpc document([#1162](https://github.com/aliyun/terraform-provider-alicloud/issues/1162))
- Improve some slb datasource([#1155](https://github.com/aliyun/terraform-provider-alicloud/issues/1155))
- improve forward_entry testcase([#1152](https://github.com/aliyun/terraform-provider-alicloud/issues/1152))
- improve slb_attachment resource use common method([#1148](https://github.com/aliyun/terraform-provider-alicloud/issues/1148))
- Improve ram_account_alias resource use common method ([#1147](https://github.com/aliyun/terraform-provider-alicloud/issues/1147))
- slb instance support updating specification([#1145](https://github.com/aliyun/terraform-provider-alicloud/issues/1145))
- improve slb_server_group resource use common method([#1144](https://github.com/aliyun/terraform-provider-alicloud/issues/1144))
- add note for SLB that intl account does not support creating PrePaid instance([#1143](https://github.com/aliyun/terraform-provider-alicloud/issues/1143))
- Update ots document([#1142](https://github.com/aliyun/terraform-provider-alicloud/issues/1142))
- improve slb_server_certificate resource use common method([#1139](https://github.com/aliyun/terraform-provider-alicloud/issues/1139))

BUG FIXES:

- Fix ram account alias notfound bug([#1161](https://github.com/aliyun/terraform-provider-alicloud/issues/1161))
- fix(nas): refactor testcases([#1157](https://github.com/aliyun/terraform-provider-alicloud/issues/1157))

## 1.42.0 (May 10, 2019)

FEATURES:

- **New Resource:** `alicloud_snapshot_policy`([#989](https://github.com/aliyun/terraform-provider-alicloud/issues/989))

IMPROVEMENTS:

- improve mongodb and db sweeper test([#1138](https://github.com/aliyun/terraform-provider-alicloud/issues/1138))
- Alicloud_ots_table: add max version offset([#1137](https://github.com/aliyun/terraform-provider-alicloud/issues/1137))
- update disk category([#1135](https://github.com/aliyun/terraform-provider-alicloud/issues/1135))
- Update Route Entry Resource([#1134](https://github.com/aliyun/terraform-provider-alicloud/issues/1134))
- update images testcase check condition([#1133](https://github.com/aliyun/terraform-provider-alicloud/issues/1133))
- bugfix: ess alarm apply recreate([#1131](https://github.com/aliyun/terraform-provider-alicloud/issues/1131))
- improve slb_listener resource use common method([#1130](https://github.com/aliyun/terraform-provider-alicloud/issues/1130))
- mongodb sharding instance add backup policy support([#1127](https://github.com/aliyun/terraform-provider-alicloud/issues/1127))
- Improve ram_users datasource use common method([#1126](https://github.com/aliyun/terraform-provider-alicloud/issues/1126))
- Improve ram_policies datasource use common method([#1125](https://github.com/aliyun/terraform-provider-alicloud/issues/1125))
- rds datasource test case remove connection mode check([#1124](https://github.com/aliyun/terraform-provider-alicloud/issues/1124))
- Add missing bracket([#1123](https://github.com/aliyun/terraform-provider-alicloud/issues/1123))
- add support sha256([#1122](https://github.com/aliyun/terraform-provider-alicloud/issues/1122))
- Improve ram_groups datasource use common method([#1121](https://github.com/aliyun/terraform-provider-alicloud/issues/1121))
- Modified the sweep rules in ram_roles testcases([#1116](https://github.com/aliyun/terraform-provider-alicloud/issues/1116))
- improve instance testcase([#1114](https://github.com/aliyun/terraform-provider-alicloud/issues/1114))
- Improve slb_ca_certificate resource use common method([#1113](https://github.com/aliyun/terraform-provider-alicloud/issues/1113))
- Improve ram_roles datasource use common method([#1112](https://github.com/aliyun/terraform-provider-alicloud/issues/1112))
- Improve slb datasource use common method([#1111](https://github.com/aliyun/terraform-provider-alicloud/issues/1111))
- Improve ram_account_alias use common method([#1108](https://github.com/aliyun/terraform-provider-alicloud/issues/1108))
- update data_source_alicoud_mongo_instances and add test case([#1107](https://github.com/aliyun/terraform-provider-alicloud/issues/1107))
- add mongodb backup policy support, test case, document([#1106](https://github.com/aliyun/terraform-provider-alicloud/issues/1106))
- update route_entry and forward_entry document([#1096](https://github.com/aliyun/terraform-provider-alicloud/issues/1096))
- Improve slb_acl resource use common method([#1092](https://github.com/aliyun/terraform-provider-alicloud/issues/1092))
- improve snat_entry testcase([#1091](https://github.com/aliyun/terraform-provider-alicloud/issues/1091))
- Improve slb resource use common method([#1090](https://github.com/aliyun/terraform-provider-alicloud/issues/1090))
- improve nat_gateway testcase([#1089](https://github.com/aliyun/terraform-provider-alicloud/issues/1089))
- Modify table to entry([#1088](https://github.com/aliyun/terraform-provider-alicloud/issues/1088))
- Modified the error code returned when timeout of upgrading instance([#1085](https://github.com/aliyun/terraform-provider-alicloud/issues/1085))
- improve db backup policy test case([#1083](https://github.com/aliyun/terraform-provider-alicloud/issues/1083))

BUG FIXES:

- Fix scalinggroup id is not found before creating scaling configuration ([#1119](https://github.com/aliyun/terraform-provider-alicloud/issues/1119))
- fix slb instance sets tags bug([#1105](https://github.com/aliyun/terraform-provider-alicloud/issues/1105))
- fix not support outputfile([#1095](https://github.com/aliyun/terraform-provider-alicloud/issues/1095))
- Bugfix/slb import server group([#1093](https://github.com/aliyun/terraform-provider-alicloud/issues/1093))
- Fix fc_triggers datasource when type is mns_topic([#1086](https://github.com/aliyun/terraform-provider-alicloud/issues/1086))

## 1.41.0 (April 29, 2019)

IMPROVEMENTS:

- Improve fc_trigger support mns_topic modify config([#1082](https://github.com/aliyun/terraform-provider-alicloud/issues/1082))
- Rds sdk-update([#1078](https://github.com/aliyun/terraform-provider-alicloud/issues/1078))
- update some eip method name([#1077](https://github.com/aliyun/terraform-provider-alicloud/issues/1077))
- improve vswitch testcase ([#1076](https://github.com/aliyun/terraform-provider-alicloud/issues/1076))
- add rand for db_instances testcase([#1074](https://github.com/aliyun/terraform-provider-alicloud/issues/1074))
- Improve fc_trigger support mns_topic([#1073](https://github.com/aliyun/terraform-provider-alicloud/issues/1073))
- remove zone_id setting in the db instance testcase([#1069](https://github.com/aliyun/terraform-provider-alicloud/issues/1069))
- change database default zone id to avoid some unsupported cases([#1067](https://github.com/aliyun/terraform-provider-alicloud/issues/1067))
- add oss bucket policy implementation([#1066](https://github.com/aliyun/terraform-provider-alicloud/issues/1066))
- improve vpc testcase([#1065](https://github.com/aliyun/terraform-provider-alicloud/issues/1065))
- Change password to Yourpassword([#1063](https://github.com/aliyun/terraform-provider-alicloud/issues/1063))
- Improve kvstore_instance datasource use common method([#1062](https://github.com/aliyun/terraform-provider-alicloud/issues/1062))
- improve eip testcase([#1058](https://github.com/aliyun/terraform-provider-alicloud/issues/1058))
- Improve kvstore_instance testcase use common method([#1052](https://github.com/aliyun/terraform-provider-alicloud/issues/1052))
- improve mongodb testcase([#1050](https://github.com/aliyun/terraform-provider-alicloud/issues/1050))
- update network_interface dataSource basic testcase config([#1049](https://github.com/aliyun/terraform-provider-alicloud/issues/1049))
- Improve kvstore_backup_policy testcase use common method([#1044](https://github.com/aliyun/terraform-provider-alicloud/issues/1044))

BUG FIXES:

- Fix fc_triggers datasource when type is mns_topic([#1086](https://github.com/aliyun/terraform-provider-alicloud/issues/1086))
- Fix kvstore_instance multi([#1080](https://github.com/aliyun/terraform-provider-alicloud/issues/1080))
- fix eip_association bug when snat or forward be released([#1075](https://github.com/aliyun/terraform-provider-alicloud/issues/1075))
- Fix db_readonly_instance instance_name([#1071](https://github.com/aliyun/terraform-provider-alicloud/issues/1071))
- fixed DB log backup policy bug when the log_retention_period does not input([#1056](https://github.com/aliyun/terraform-provider-alicloud/issues/1056))
- fix cms diff bug and improve its testcases([#1057](https://github.com/aliyun/terraform-provider-alicloud/issues/1057))


## 1.40.0 (April 20, 2019)

FEATURES:

- **New Resource:** `alicloud_mongodb_sharding_instance`([#1017](https://github.com/aliyun/terraform-provider-alicloud/issues/1017))
- **New Data Source:** `alicloud_snapshots`([#988](https://github.com/aliyun/terraform-provider-alicloud/issues/988))
- **New Resource:** `alicloud_snapshot`([#954](https://github.com/aliyun/terraform-provider-alicloud/issues/954))

IMPROVEMENTS:

- Fix db_instance can't find method DescribeDbInstance([#1046](https://github.com/aliyun/terraform-provider-alicloud/issues/1046))
- update network_interface testcase config([#1045](https://github.com/aliyun/terraform-provider-alicloud/issues/1045))
- Update Nat Gateway Resource([#1043](https://github.com/aliyun/terraform-provider-alicloud/issues/1043))
- improve network_interface dataSource testcase([#1042](https://github.com/aliyun/terraform-provider-alicloud/issues/1042))
- improve network_interface resource testcase([#1041](https://github.com/aliyun/terraform-provider-alicloud/issues/1041))
- Improve db_database db_instance db_readonly_instance db_readwrite_splitting_connection([#1040](https://github.com/aliyun/terraform-provider-alicloud/issues/1040))
- improve key_pair resource testcase([#1039](https://github.com/aliyun/terraform-provider-alicloud/issues/1039))
- improve key_pair dataSource testcase([#1038](https://github.com/aliyun/terraform-provider-alicloud/issues/1038))
- make fmt ess_scalinggroups([#1036](https://github.com/aliyun/terraform-provider-alicloud/issues/1036))
- improve test common method([#1030](https://github.com/aliyun/terraform-provider-alicloud/issues/1030))
- Update cen data source document([#1029](https://github.com/aliyun/terraform-provider-alicloud/issues/1029))
- fix Error method([#1024](https://github.com/aliyun/terraform-provider-alicloud/issues/1024)) 
- Update Nat Gateway Token([#1020](https://github.com/aliyun/terraform-provider-alicloud/issues/1020))
- update RAM website document([#1019](https://github.com/aliyun/terraform-provider-alicloud/issues/1019))
- add computed for resource_group_id([#1018](https://github.com/aliyun/terraform-provider-alicloud/issues/1018))
- remove ram validators and update website docs([#1016](https://github.com/aliyun/terraform-provider-alicloud/issues/1016))
- improve test common method, support 'TestMatchResourceAttr' check([#1012](https://github.com/aliyun/terraform-provider-alicloud/issues/1012))
- resource group support for creating new VPC([#1010](https://github.com/aliyun/terraform-provider-alicloud/issues/1010))
- Improve cs_cluster sweeper test removing retained resources([#1002](https://github.com/aliyun/terraform-provider-alicloud/issues/1002))
- improve security_group testcase use common method([#995](https://github.com/aliyun/terraform-provider-alicloud/issues/995))
- fix vpn change local_subnet and remote_subnet bug([#994](https://github.com/aliyun/terraform-provider-alicloud/issues/994))
- improve disk dataSource testcase use common method([#990](https://github.com/aliyun/terraform-provider-alicloud/issues/990))
- fix(nas): use new sdk([#984](https://github.com/aliyun/terraform-provider-alicloud/issues/984))
- Feature/slb listener redirect http to https([#981](https://github.com/aliyun/terraform-provider-alicloud/issues/981))
- improve disk and diskAttachment resource testcase use testCommon method([#978](https://github.com/aliyun/terraform-provider-alicloud/issues/978))
- improve dns dataSource testcase use testCommon method([#971](https://github.com/aliyun/terraform-provider-alicloud/issues/971))

BUG FIXES:

- Fix ess go sdk compatibility([#1032](https://github.com/aliyun/terraform-provider-alicloud/issues/1032))
- Update sdk to fix timeout bug([#1015](https://github.com/aliyun/terraform-provider-alicloud/issues/1015))
- Fix Eip And VSwitch ClientToken bug([#1000](https://github.com/aliyun/terraform-provider-alicloud/issues/1000))
- fix db_account diff bug and add some notes for it([#999](https://github.com/aliyun/terraform-provider-alicloud/issues/999))
- fix vpn gateway Period bug([#993](https://github.com/aliyun/terraform-provider-alicloud/issues/993))


## 1.39.0 (April 09, 2019)

FEATURES:

- **New Data Source:** `alicloud_ots_instance_attachments`([#986](https://github.com/aliyun/terraform-provider-alicloud/issues/986))
- **New Data Source:** `alicloud_ssl_vpc_servers`([#985](https://github.com/aliyun/terraform-provider-alicloud/issues/985))
- **New Data Source:** `alicloud_ssl_vpn_client_certs`([#986](https://github.com/aliyun/terraform-provider-alicloud/issues/986))
- **New Data Source:** `alicloud_ess_scaling_rules`([#976](https://github.com/aliyun/terraform-provider-alicloud/issues/976))
- **New Data Source:** `alicloud_ess_scaling_configurations`([#974](https://github.com/aliyun/terraform-provider-alicloud/issues/974))
- **New Data Source:** `alicloud_ess_scaling_groups`([#973](https://github.com/aliyun/terraform-provider-alicloud/issues/973))
- **New Data Source:** `alicloud_ddoscoo_instances`([#967](https://github.com/aliyun/terraform-provider-alicloud/issues/967))
- **New Data Source:** `alicloud_ots_instances`([#946](https://github.com/aliyun/terraform-provider-alicloud/issues/946))

IMPROVEMENTS:

- Improve instance type updating testcase([#979](https://github.com/aliyun/terraform-provider-alicloud/issues/979))
- support changing prepaid instance type([#977](https://github.com/aliyun/terraform-provider-alicloud/issues/977))
- Improve db_account db_account_privilege db_backup_policy db_connection([#963](https://github.com/aliyun/terraform-provider-alicloud/issues/963))

BUG FIXES:

- Fix Nat GW ClientToken bug([#983](https://github.com/aliyun/terraform-provider-alicloud/issues/983))
- Fix print error bug after DescribeDBInstanceById([#980](https://github.com/aliyun/terraform-provider-alicloud/issues/980))

## 1.38.0 (April 03, 2019)

FEATURES:

- **New Resource:** `alicloud_ddoscoo_instance`([#952](https://github.com/aliyun/terraform-provider-alicloud/issues/952))

IMPROVEMENTS:

- update dns_group describe method([#966](https://github.com/aliyun/terraform-provider-alicloud/issues/966))
- update ram_policy resource testcase([#964](https://github.com/aliyun/terraform-provider-alicloud/issues/964))
- improve ram_policy resource update method([#960](https://github.com/aliyun/terraform-provider-alicloud/issues/960))
- ecs prepaid instance supports changing instance type([#949](https://github.com/aliyun/terraform-provider-alicloud/issues/949))
- update mongodb instance test case for multiAZ([#947](https://github.com/aliyun/terraform-provider-alicloud/issues/947))
- add test common method ,improve dns resource testcase([#927](https://github.com/aliyun/terraform-provider-alicloud/issues/927))


BUG FIXES:

- Fix drds instance sweeper test bug([#955](https://github.com/aliyun/terraform-provider-alicloud/issues/955))

## 1.37.0 (March 29, 2019)

FEATURES:

- **New Resource:** `alicloud_mongodb_instance`([#881](https://github.com/aliyun/terraform-provider-alicloud/issues/881))
- **New Resource:** `alicloud_cen_instance_grant`([#857](https://github.com/aliyun/terraform-provider-alicloud/issues/857))
- **New Data Source:** `alicloud_forward_entries`([#922](https://github.com/aliyun/terraform-provider-alicloud/issues/922))
- **New Data Source:** `alicloud_snat_entries`([#920](https://github.com/aliyun/terraform-provider-alicloud/issues/920))
- **New Data Source:** `alicloud_nat_gateways`([#918](https://github.com/aliyun/terraform-provider-alicloud/issues/918))
- **New Data Source:** `alicloud_route_entries`([#915](https://github.com/aliyun/terraform-provider-alicloud/issues/915))

IMPROVEMENTS:

- Add missing outputs for datasource dns_records, security groups, vpcs and vswitches([#943](https://github.com/aliyun/terraform-provider-alicloud/issues/943))
- datasource dns_records add a output urls([#942](https://github.com/aliyun/terraform-provider-alicloud/issues/942))
- modify stop instance timeout to 5min to avoid the exception timeout([#941](https://github.com/aliyun/terraform-provider-alicloud/issues/941))
- datasource security_groups, vpcs and vswitches support outputs ids and names([#939](https://github.com/aliyun/terraform-provider-alicloud/issues/939))
- Improve all of parameter's tag, like 'Required', 'ForceNew'([#938](https://github.com/aliyun/terraform-provider-alicloud/issues/938))
- Improve pvtz_zone_record WrapError([#934](https://github.com/aliyun/terraform-provider-alicloud/issues/934))
- Improve pvtz_zone_record create record([#933](https://github.com/aliyun/terraform-provider-alicloud/issues/933))
- testSweepCRNamespace skip not supported region ([#932](https://github.com/aliyun/terraform-provider-alicloud/issues/932))
- refine retry logic of resource tablestore to avoid the exception timeout([#931](https://github.com/aliyun/terraform-provider-alicloud/issues/931))
- Improve pvtz resource datasource testcases([#928](https://github.com/aliyun/terraform-provider-alicloud/issues/928))
- cr_repos fix docs link error([#926](https://github.com/aliyun/terraform-provider-alicloud/issues/926))
- resource DB instance supports setting security group([#925](https://github.com/aliyun/terraform-provider-alicloud/issues/925))
- resource DB instance supports setting monitor period([#924](https://github.com/aliyun/terraform-provider-alicloud/issues/924))
- Skipping bandwidth package related test for international site account([#917](https://github.com/aliyun/terraform-provider-alicloud/issues/917))
- Resource snat entry update id and support import([#916](https://github.com/aliyun/terraform-provider-alicloud/issues/916))
- add docs about prerequisites for cs and cr ([#914](https://github.com/aliyun/terraform-provider-alicloud/issues/914))
- add new schema environment_variables to fc_function.html.markdown([#913](https://github.com/aliyun/terraform-provider-alicloud/issues/913))
- add skipping check for datasource route tables' testcases([#911](https://github.com/aliyun/terraform-provider-alicloud/issues/911))
- modify ram_user id by userId([#900](https://github.com/aliyun/terraform-provider-alicloud/issues/900))

BUG FIXES:

- Deprecate bucket `logging_isenable` and fix referer_config diff bug([#937](https://github.com/aliyun/terraform-provider-alicloud/issues/937))
- fix ram user and group sweeper test bug([#929](https://github.com/aliyun/terraform-provider-alicloud/issues/929))
- Fix the parameter bug when actiontrail is created([#921](https://github.com/aliyun/terraform-provider-alicloud/issues/921))
- fix default pod_cidr in k8s docs([#919](https://github.com/aliyun/terraform-provider-alicloud/issues/919))

## 1.36.0 (March 24, 2019)

FEATURES:

- **New Resource:** `alicloud_cas_certificate`([#875](https://github.com/aliyun/terraform-provider-alicloud/issues/875))
- **New Data Source:** `alicloud_route_tables`([#905](https://github.com/aliyun/terraform-provider-alicloud/issues/905))
- **New Data Source:** `alicloud_common_bandwidth_packages`([#897](https://github.com/aliyun/terraform-provider-alicloud/issues/897))
- **New Data Source:** `alicloud_actiontrails`([#891](https://github.com/aliyun/terraform-provider-alicloud/issues/891))
- **New Data Source:** `alicloud_cas_certificates`([#875](https://github.com/aliyun/terraform-provider-alicloud/issues/875))

IMPROVEMENTS:

- Add wait method for disk and disk attachment([#910](https://github.com/aliyun/terraform-provider-alicloud/issues/910))
- Add wait method for cen instance([#909](https://github.com/aliyun/terraform-provider-alicloud/issues/909))
- add dns and dns_group test sweeper([#906](https://github.com/aliyun/terraform-provider-alicloud/issues/906))
- fc_function add new schema environment_variables([#904](https://github.com/aliyun/terraform-provider-alicloud/issues/904))
- support kv-store auto renewal option  documentation([#902](https://github.com/aliyun/terraform-provider-alicloud/issues/902))
- Sort slb slave zone ids to avoid needless error([#898](https://github.com/aliyun/terraform-provider-alicloud/issues/898))
- add region skip for container registry testcase([#896](https://github.com/aliyun/terraform-provider-alicloud/issues/896))
- Add `enable_details` for alicloud_zones and support retrieving slb slave zones([#893](https://github.com/aliyun/terraform-provider-alicloud/issues/893))
- Slb support setting master and slave zone id([#887](https://github.com/aliyun/terraform-provider-alicloud/issues/887))
- improve disk and attachment resource testcase([#886](https://github.com/aliyun/terraform-provider-alicloud/issues/886))
- Remove ModifySecurityGroupPolicy waiting and backend has fixed it([#883](https://github.com/aliyun/terraform-provider-alicloud/issues/883))
- Improve cas resource and datasource testcases([#882](https://github.com/aliyun/terraform-provider-alicloud/issues/882))
- Make db_connection resource code more standard([#879](https://github.com/aliyun/terraform-provider-alicloud/issues/879))

BUG FIXES:

- Fix cen instance deleting bug([#908](https://github.com/aliyun/terraform-provider-alicloud/issues/908))
- Fix cen create bug when one resion is China([#903](https://github.com/aliyun/terraform-provider-alicloud/issues/903))
- fix cas_certificate sweeper test bug([#899](https://github.com/aliyun/terraform-provider-alicloud/issues/899))
- Modify ram group's name's ForceNew to true([#895](https://github.com/aliyun/terraform-provider-alicloud/issues/895))
- fix mount target deletion bugs([#892](https://github.com/aliyun/terraform-provider-alicloud/issues/892))
- Fix link to BatchSetCdnDomainConfig document  documentation([#885](https://github.com/aliyun/terraform-provider-alicloud/issues/885))
- fix rds instance parameter test case issue([#880](https://github.com/aliyun/terraform-provider-alicloud/issues/880))

## 1.35.0 (March 18, 2019)

FEATURES:

- **New Resource:** `alicloud_cr_repo`([#862](https://github.com/aliyun/terraform-provider-alicloud/issues/862))
- **New Resource:** `alicloud_actiontrail`([#858](https://github.com/aliyun/terraform-provider-alicloud/issues/858))
- **New Data Source:** `alicloud_cr_repos`([#868](https://github.com/aliyun/terraform-provider-alicloud/issues/868))
- **New Data Source:** `alicloud_cr_namespaces`([#867](https://github.com/aliyun/terraform-provider-alicloud/issues/867))
- **New Data Source:** `alicloud_nas_file_systems`([#864](https://github.com/aliyun/terraform-provider-alicloud/issues/864))
- **New Data Source:** `alicloud_nas_mount_targets`([#864](https://github.com/aliyun/terraform-provider-alicloud/issues/864))
- **New Data Source:** `alicloud_drds_instances`([#861](https://github.com/aliyun/terraform-provider-alicloud/issues/861))
- **New Data Source:** `alicloud_nas_access_rules`([#860](https://github.com/aliyun/terraform-provider-alicloud/issues/860))
- **New Data Source:** `alicloud_nas_access_groups`([#856](https://github.com/aliyun/terraform-provider-alicloud/issues/856))

IMPROVEMENTS:

- Improve actiontrail docs([#878](https://github.com/aliyun/terraform-provider-alicloud/issues/878))
- Add account pre-check for common bandwidth package to avoid known error([#877](https://github.com/aliyun/terraform-provider-alicloud/issues/877))
- Make dns resource code more standard([#876](https://github.com/aliyun/terraform-provider-alicloud/issues/876))
- Improve dns resources' testcases([#859](https://github.com/aliyun/terraform-provider-alicloud/issues/859))
- Add client token for vpn services([#855](https://github.com/aliyun/terraform-provider-alicloud/issues/855))
- reback the lossing datasource([#866](https://github.com/aliyun/terraform-provider-alicloud/issues/866))
- Improve drds instances testcases  documentation([#863](https://github.com/aliyun/terraform-provider-alicloud/issues/863))
- Update sdk for vpc package([#854](https://github.com/aliyun/terraform-provider-alicloud/issues/854))

BUG FIXES:

- Add waiting method to ensure the security group status is ok([#873](https://github.com/aliyun/terraform-provider-alicloud/issues/873))
- Fix nas mount target notfound bug and improve nas datasource's testcases([#872](https://github.com/aliyun/terraform-provider-alicloud/issues/872))
- Fix dns notfound bug([#871](https://github.com/aliyun/terraform-provider-alicloud/issues/871))
- fix creating slb bug([#870](https://github.com/aliyun/terraform-provider-alicloud/issues/870))
- fix elastic search sweeper test bug([#865](https://github.com/aliyun/terraform-provider-alicloud/issues/865))


## 1.34.0 (March 13, 2019)

FEATURES:

- **New Resource:** `alicloud_nas_mount_target`([#835](https://github.com/aliyun/terraform-provider-alicloud/issues/835))
- **New Resource:** `alicloud_cdn_domain_config`([#829](https://github.com/aliyun/terraform-provider-alicloud/issues/829))
- **New Resource:** `alicloud_cr_namespace`([#827](https://github.com/aliyun/terraform-provider-alicloud/issues/827))
- **New Resource:** `alicloud_nas_access_rule`([#827](https://github.com/aliyun/terraform-provider-alicloud/issues/827))
- **New Resource:** `alicloud_cdn_domain_new`([#787](https://github.com/aliyun/terraform-provider-alicloud/issues/787))
- **New Data Source:** `alicloud_cs_kubernetes_clusters`([#818](https://github.com/aliyun/terraform-provider-alicloud/issues/818))

IMPROVEMENTS:

- Add drds instance docs([#853](https://github.com/aliyun/terraform-provider-alicloud/issues/853))
- Improve resource mount target testcases([#852](https://github.com/aliyun/terraform-provider-alicloud/issues/852))
- Add using note for spot instance([#851](https://github.com/aliyun/terraform-provider-alicloud/issues/851))
- Resource alicloud_slb supports PrePaid([#850](https://github.com/aliyun/terraform-provider-alicloud/issues/850))
- Add ssl_vpn_server and ssl_vpn_client_cert sweeper test([#843](https://github.com/aliyun/terraform-provider-alicloud/issues/843))
- Improve vpn_gateway testcases and some sweeper test([#842](https://github.com/aliyun/terraform-provider-alicloud/issues/842))
- Improve dns datasource testcases([#841](https://github.com/aliyun/terraform-provider-alicloud/issues/841))
- Improve Eip and mns testcase([#840](https://github.com/aliyun/terraform-provider-alicloud/issues/840))
- Add version notes in some docs([#838](https://github.com/aliyun/terraform-provider-alicloud/issues/838))
- RDS resource supports auto-renewal([#836](https://github.com/aliyun/terraform-provider-alicloud/issues/836))
- Deprecate the resource alicloud_cdn_domain([#830](https://github.com/aliyun/terraform-provider-alicloud/issues/830))

BUG FIXES:

- Fix deleting dns record InternalError bug([#848](https://github.com/aliyun/terraform-provider-alicloud/issues/848))
- fix log store and config sweeper test deleting bug([#847](https://github.com/aliyun/terraform-provider-alicloud/issues/847))
- Fix drds resource no supporting client token([#846](https://github.com/aliyun/terraform-provider-alicloud/issues/846))
- fix kms sweeper test deleting bug([#844](https://github.com/aliyun/terraform-provider-alicloud/issues/844))
- fix kubernetes data resource ut and import error([#839](https://github.com/aliyun/terraform-provider-alicloud/issues/839))
- Bugfix: destroying alicloud_ess_attachment timeout([#834](https://github.com/aliyun/terraform-provider-alicloud/issues/834))
- fix cdn service func WaitForCdnDomain([#833](https://github.com/aliyun/terraform-provider-alicloud/issues/833))
- deal with the error message in cen route entry([#831](https://github.com/aliyun/terraform-provider-alicloud/issues/831))
- change bool to *bool in parameters of k8s clusters([#828](https://github.com/aliyun/terraform-provider-alicloud/issues/828))
- Fix nas docs bug([#825](https://github.com/aliyun/terraform-provider-alicloud/issues/825))
- create vpn gateway got "UnnecessarySslConnection" error when enable_ssl is false([#822](https://github.com/aliyun/terraform-provider-alicloud/issues/822))

## 1.33.0 (March 05, 2019)

FEATURES:

- **New Resource:** `alicloud_nas_access_group`([#817](https://github.com/aliyun/terraform-provider-alicloud/issues/817))
- **New Resource:** `alicloud_nas_file_system`([#807](https://github.com/aliyun/terraform-provider-alicloud/issues/807))

IMPROVEMENTS:

- Improve nas resource docs([#824](https://github.com/aliyun/terraform-provider-alicloud/issues/824))

BUG FIXES:

- bugfix: create vpn gateway got "UnnecessarySslConnection" error when enable_ssl is false([#822](https://github.com/aliyun/terraform-provider-alicloud/issues/822))
- fix volume_tags diff bug when running testcases([#816](https://github.com/aliyun/terraform-provider-alicloud/issues/816))

## 1.32.1 (March 03, 2019)

BUG FIXES:

- fix volume_tags diff bug when setting tags by alicloud_disk([#815](https://github.com/aliyun/terraform-provider-alicloud/issues/815))

## 1.32.0 (March 01, 2019)

FEATURES:

- **New Resource:** `alicloud_db_readwrite_splitting_connection`([#753](https://github.com/aliyun/terraform-provider-alicloud/issues/753))

IMPROVEMENTS:

- add slb_internet_enabled to managed kubernetes([#806](https://github.com/aliyun/terraform-provider-alicloud/issues/806))
- update alicloud_slb_attachment usage example([#805](https://github.com/aliyun/terraform-provider-alicloud/issues/805))
- rds support op tags  documentation([#797](https://github.com/aliyun/terraform-provider-alicloud/issues/797))
- ForceNew for resource record and zone id updates for pvtz record([#794](https://github.com/aliyun/terraform-provider-alicloud/issues/794))
- support volume tags for ecs instance disks([#793](https://github.com/aliyun/terraform-provider-alicloud/issues/793))
- Improve instance and security group testcase for different account site([#792](https://github.com/aliyun/terraform-provider-alicloud/issues/792))
- Add account site type setting to skip unsupported test cases automatically([#790](https://github.com/aliyun/terraform-provider-alicloud/issues/790))
- update alibaba-cloud-sdk-go to use lastest useragent and modify errMessage when signature does not match  dependencies([#788](https://github.com/aliyun/terraform-provider-alicloud/issues/788))
- make the timeout longer when cen attach/detach vpc([#786](https://github.com/aliyun/terraform-provider-alicloud/issues/786))
- cen child instance attach after vsw created([#785](https://github.com/aliyun/terraform-provider-alicloud/issues/785))
- kvstore support parameter configuration([#784](https://github.com/aliyun/terraform-provider-alicloud/issues/784))
- Modify useragent to meet the standard of sdk([#778](https://github.com/aliyun/terraform-provider-alicloud/issues/778))
- Modify kms client to dock with the alicloud official GO SDK([#763](https://github.com/aliyun/terraform-provider-alicloud/issues/763))

BUG FIXES:

- fix rds readonly instance name update issue([#812](https://github.com/aliyun/terraform-provider-alicloud/issues/812))
- fix import managed kubernetes test([#809](https://github.com/aliyun/terraform-provider-alicloud/issues/809))
- fix rds parameter update issue([#804](https://github.com/aliyun/terraform-provider-alicloud/issues/804))
- fix first create db with tags([#803](https://github.com/aliyun/terraform-provider-alicloud/issues/803))
- Fix dns record ttl setting error and update bug([#800](https://github.com/aliyun/terraform-provider-alicloud/issues/800))
- Fix vpc return custom route table bug([#799](https://github.com/aliyun/terraform-provider-alicloud/issues/799))
- fix ssl vpn subnet can not pass comma separated string problem([#780](https://github.com/aliyun/terraform-provider-alicloud/issues/780))
- fix(whitelist) Modified whitelist returned and filter the default values([#779](https://github.com/aliyun/terraform-provider-alicloud/issues/779))

## 1.31.0 (February 19, 2019)

FEATURES:

- **New Resource:** `alicloud_db_readonly_instance`([#755](https://github.com/aliyun/terraform-provider-alicloud/issues/755))

IMPROVEMENTS:

- support update deletion_protection option documentation([#771](https://github.com/aliyun/terraform-provider-alicloud/issues/771))
- add three az k8s cluster docs  documentation([#767](https://github.com/aliyun/terraform-provider-alicloud/issues/767))
- kvstore support vpc_auth_mode  dependencies([#765](https://github.com/aliyun/terraform-provider-alicloud/issues/765))
- Fix sls logtail config collection error([#762](https://github.com/aliyun/terraform-provider-alicloud/issues/762))
- Add attribute parameters to resource alicloud_db_instance  documentation([#761](https://github.com/aliyun/terraform-provider-alicloud/issues/761))
- Add attribute parameters to resource alicloud_db_instance([#761](https://github.com/aliyun/terraform-provider-alicloud/issues/761))
- Modify dns client to dock with the alicloud official GO SDK([#750](https://github.com/aliyun/terraform-provider-alicloud/issues/750))

BUG FIXES:

- Fix cms_alarm updating notify_type bug([#773](https://github.com/aliyun/terraform-provider-alicloud/issues/773))
- fix(error) Fixed bug of error code when timeout for upgrade instance([#770](https://github.com/aliyun/terraform-provider-alicloud/issues/770))
- delete success if not found cen route when delete([#753](https://github.com/aliyun/terraform-provider-alicloud/issues/753))

## 1.30.0 (February 04, 2019)

FEATURES:

- **New Resource:** `alicloud_elasticsearch_instance`([#722](https://github.com/aliyun/terraform-provider-alicloud/issues/722))
- **New Resource:** `alicloud_logtail_attachment`([#705](https://github.com/aliyun/terraform-provider-alicloud/issues/705))
- **New Data Source:** `alicloud_elasticsearch_instances`([#739](https://github.com/aliyun/terraform-provider-alicloud/issues/739))

IMPROVEMENTS:

- Improve snat and forward testcases([#749](https://github.com/aliyun/terraform-provider-alicloud/issues/749))
- delete data source roles limit of policy_type and policy_name([#748](https://github.com/aliyun/terraform-provider-alicloud/issues/748))
- make k8s cluster deleting timeout longer([#746](https://github.com/aliyun/terraform-provider-alicloud/issues/746))
- Improve nat_gateway testcases([#743](https://github.com/aliyun/terraform-provider-alicloud/issues/743))
- Improve eip_association testcases([#742](https://github.com/aliyun/terraform-provider-alicloud/issues/742))
- Improve elasticinstnace testcases for IPV6 supported([#741](https://github.com/aliyun/terraform-provider-alicloud/issues/741))
- Add debug for db instance and ess group([#740](https://github.com/aliyun/terraform-provider-alicloud/issues/740))
- Improve api_gateway_vpc_access testcases([#738](https://github.com/aliyun/terraform-provider-alicloud/issues/738))
- Modify errors and  ram client to dock with the GO SDK([#735](https://github.com/aliyun/terraform-provider-alicloud/issues/735))
- provider supports getting credential via ecs role name([#731](https://github.com/aliyun/terraform-provider-alicloud/issues/731))
- Update testcases for cen region domain route entries([#729](https://github.com/aliyun/terraform-provider-alicloud/issues/729))
- cs_kubernetes supports user_ca([#726](https://github.com/aliyun/terraform-provider-alicloud/issues/726))
- Wrap resource elasticserarch_instance's error([#725](https://github.com/aliyun/terraform-provider-alicloud/issues/725))
- Add note for kubernetes resource and improve its testcase([#724](https://github.com/aliyun/terraform-provider-alicloud/issues/724))
- Datasource instance_types supports filter results and used to create kuberneters([#723](https://github.com/aliyun/terraform-provider-alicloud/issues/723))
- Add ids parameter extraction in data source regions,zones,dns_domain,images and instance_types([#718](https://github.com/aliyun/terraform-provider-alicloud/issues/718))
- Improve dns group testcase([#717](https://github.com/aliyun/terraform-provider-alicloud/issues/717))
- Improve security group rule testcase for classic([#716](https://github.com/aliyun/terraform-provider-alicloud/issues/716))
- Improve security group creating request([#715](https://github.com/aliyun/terraform-provider-alicloud/issues/715))
- Route entry supports Nat Gateway([#713](https://github.com/aliyun/terraform-provider-alicloud/issues/713))
- Modify db account returning update to read after creating([#711](https://github.com/aliyun/terraform-provider-alicloud/issues/711))
- Improve cdn testcase([#708](https://github.com/aliyun/terraform-provider-alicloud/issues/708))
- Apply wraperror to security_group, security_group_rule, vswitch, disk([#707](https://github.com/aliyun/terraform-provider-alicloud/issues/707))
- Improve cdn testcase([#705](https://github.com/aliyun/terraform-provider-alicloud/issues/705))
- Add notes for datahub and improve its testcase([#704](https://github.com/aliyun/terraform-provider-alicloud/issues/704))
- Improve security_group_rule resource and data source testcases([#703](https://github.com/aliyun/terraform-provider-alicloud/issues/703))
- Improve kvstore backup policy([#701](https://github.com/aliyun/terraform-provider-alicloud/issues/701))
- Improve pvtz attachment testcase([#700](https://github.com/aliyun/terraform-provider-alicloud/issues/700))
- Modify pagesize on API DescribeVSWitches tp avoid ServiceUnavailable([#698](https://github.com/aliyun/terraform-provider-alicloud/issues/698))
- Improve eip resource and data source testcases([#697](https://github.com/aliyun/terraform-provider-alicloud/issues/697))

BUG FIXES:

- FIx cen route NotFoundRoute error when deleting([#753](https://github.com/aliyun/terraform-provider-alicloud/issues/753))
- Fix log_store InternalServerError error([#737](https://github.com/aliyun/terraform-provider-alicloud/issues/737))
- Fix cen region route entries testcase bug([#734](https://github.com/aliyun/terraform-provider-alicloud/issues/734))
- Fix ots_table StorageServerBusy bug([#733](https://github.com/aliyun/terraform-provider-alicloud/issues/733))
- Fix db_account setting description bug([#732](https://github.com/aliyun/terraform-provider-alicloud/issues/732))
- Fix Router Entry Token Bug([#730](https://github.com/aliyun/terraform-provider-alicloud/issues/730))
- Fix instance diff bug when updating its VPC attributes([#728](https://github.com/aliyun/terraform-provider-alicloud/issues/728))
- Fix snat entry IncorretSnatEntryStatus error when deleting([#714](https://github.com/aliyun/terraform-provider-alicloud/issues/714))
- Fix forward entry UnknownError error([#712](https://github.com/aliyun/terraform-provider-alicloud/issues/712))
- Fix pvtz record Zone.NotExists error when deleting record([#710](https://github.com/aliyun/terraform-provider-alicloud/issues/710))
- Fix modify kvstore policy not working bug([#709](https://github.com/aliyun/terraform-provider-alicloud/issues/709))
- reattach the key pair after update OS image([#699](https://github.com/aliyun/terraform-provider-alicloud/issues/699))
- Fix ServiceUnavailable error on VPC and VSW([#695](https://github.com/aliyun/terraform-provider-alicloud/issues/695))

## 1.29.0 (January 21, 2019)

FEATURES:

- **New Resource:** `alicloud_logtail_config`([#685](https://github.com/aliyun/terraform-provider-alicloud/issues/685))

IMPROVEMENTS:

- Apply wraperror to ess group([#689](https://github.com/aliyun/terraform-provider-alicloud/issues/689))
- Add wraperror and apply it to vpc and eip([#688](https://github.com/aliyun/terraform-provider-alicloud/issues/688))
- Improve vswitch resource and data source testcases([#687](https://github.com/aliyun/terraform-provider-alicloud/issues/687))
- Improve security_group resource and data source testcases([#686](https://github.com/aliyun/terraform-provider-alicloud/issues/686))
- Improve vpc resource and data source testcases([#684](https://github.com/aliyun/terraform-provider-alicloud/issues/684))
- Modify the slb sever group testcase name([#681](https://github.com/aliyun/terraform-provider-alicloud/issues/681))
- Improve sweeper testcases([#680](https://github.com/aliyun/terraform-provider-alicloud/issues/680))
- Improve db instance's testcases([#679](https://github.com/aliyun/terraform-provider-alicloud/issues/679))
- Improve ecs disk's testcases([#678](https://github.com/aliyun/terraform-provider-alicloud/issues/678))
- Add multi_zone_ids for datasource alicloud_zones([#677](https://github.com/aliyun/terraform-provider-alicloud/issues/677))
- Improve redis and memcache instance testcases([#676](https://github.com/aliyun/terraform-provider-alicloud/issues/676))
- Improve ecs instance testcases([#675](https://github.com/aliyun/terraform-provider-alicloud/issues/675))

BUG FIXES:

- Fix oss bucket docs error([#692](https://github.com/aliyun/terraform-provider-alicloud/issues/692))
- Fix pvtz 'Zone.VpcExists' error([#691](https://github.com/aliyun/terraform-provider-alicloud/issues/691))
- Fix multi-k8s testcase failed error([#683](https://github.com/aliyun/terraform-provider-alicloud/issues/683))
- Fix pvtz attchment Zone.NotExists error([#682](https://github.com/aliyun/terraform-provider-alicloud/issues/682))
- Fix deleting ram role error([#674](https://github.com/aliyun/terraform-provider-alicloud/issues/674))
- Fix k8s cluster worker_period_unit type error([#672](https://github.com/aliyun/terraform-provider-alicloud/issues/672))

## 1.28.0 (January 16, 2019)

IMPROVEMENTS:

- Ots service support https([#669](https://github.com/aliyun/terraform-provider-alicloud/issues/669))
- check vswitch id when creating instance  documentation([#668](https://github.com/aliyun/terraform-provider-alicloud/issues/668))
- Improve pvtz attachment test updating case([#663](https://github.com/aliyun/terraform-provider-alicloud/issues/663))
- add vswitch id checker when creating k8s clusters([#656](https://github.com/aliyun/terraform-provider-alicloud/issues/656))
- Improve cen instance testcase to avoid mistake query([#655](https://github.com/aliyun/terraform-provider-alicloud/issues/655))
- Improve route entry retry strategy to avoid concurrence issue([#654](https://github.com/aliyun/terraform-provider-alicloud/issues/654))
- Offline drds resource from website results from drds does not support idempotent([#653](https://github.com/aliyun/terraform-provider-alicloud/issues/653))
- Support customer endpoints in the provider([#652](https://github.com/aliyun/terraform-provider-alicloud/issues/652))
- Reback image filter to meet many non-ecs testcase([#649](https://github.com/aliyun/terraform-provider-alicloud/issues/649))
- Improve ecs instance testcase by update instance type([#646](https://github.com/aliyun/terraform-provider-alicloud/issues/646))
- Support cs client setting customer endpoint([#643](https://github.com/aliyun/terraform-provider-alicloud/issues/643))
- do not poll nodes when k8s cluster is stable([#641](https://github.com/aliyun/terraform-provider-alicloud/issues/641))
- Improve pvtz_zone testcase by using rand([#639](https://github.com/aliyun/terraform-provider-alicloud/issues/639))
- support for zero node clusters in swarm container service([#638](https://github.com/aliyun/terraform-provider-alicloud/issues/638))
- Slb listener can not be updated when load balancer instance is shared-performance([#637](https://github.com/aliyun/terraform-provider-alicloud/issues/637))
- Improve db_account testcase and its docs([#635](https://github.com/aliyun/terraform-provider-alicloud/issues/635))
- Adding https_config options to the alicloud_cdn_domain resource([#605](https://github.com/aliyun/terraform-provider-alicloud/issues/605))

BUG FIXES:

- Fix slb OperationFailed.TokenIsProcessing error([#667](https://github.com/aliyun/terraform-provider-alicloud/issues/667))
- Fix deleting log project requestTimeout error([#666](https://github.com/aliyun/terraform-provider-alicloud/issues/666))
- Fix cs_kubernetes setting int value error([#665](https://github.com/aliyun/terraform-provider-alicloud/issues/665))
- Fix pvtz zone attaching vpc system busy error([#660](https://github.com/aliyun/terraform-provider-alicloud/issues/660))
- Fix ecs and ess tags read bug with ignore system tag([#659](https://github.com/aliyun/terraform-provider-alicloud/issues/659))
- Fix cs cluster not found error and improve its testcase([#658](https://github.com/aliyun/terraform-provider-alicloud/issues/658))
- Fix deleting pvtz zone not exist and internal error([#657](https://github.com/aliyun/terraform-provider-alicloud/issues/657))
- Fix pvtz throttling user bug and improve WrapError([#650](https://github.com/aliyun/terraform-provider-alicloud/issues/650))
- Fix ess group describing error([#644](https://github.com/aliyun/terraform-provider-alicloud/issues/644))
- Fix pvtz throttling user bug and add WrapError([#642](https://github.com/aliyun/terraform-provider-alicloud/issues/642))
- Fix kvstore instance docs([#636](https://github.com/aliyun/terraform-provider-alicloud/issues/636))

## 1.27.0 (January 08, 2019)

IMPROVEMENTS:

- Improve slb instance docs([#632](https://github.com/aliyun/terraform-provider-alicloud/issues/632))
- Upgrade to Go 1.11([#629](https://github.com/aliyun/terraform-provider-alicloud/issues/629))
- Remove ots https schema because of in some region only supports http([#630](https://github.com/aliyun/terraform-provider-alicloud/issues/630))
- Support https for log client([#623](https://github.com/aliyun/terraform-provider-alicloud/issues/623))
- Support https for ram, cdn, kms and fc client([#622](https://github.com/aliyun/terraform-provider-alicloud/issues/622))
- Support https for dns client([#621](https://github.com/aliyun/terraform-provider-alicloud/issues/621))
- Support https for services client using official sdk([#619](https://github.com/aliyun/terraform-provider-alicloud/issues/619))
- Support mns client https and improve mns testcase([#618](https://github.com/aliyun/terraform-provider-alicloud/issues/618))
- Support oss client https([#617](https://github.com/aliyun/terraform-provider-alicloud/issues/617))
- Support change kvstore instance charge type([#602](https://github.com/aliyun/terraform-provider-alicloud/issues/602))
- add region checks to kubernetes, multiaz kubernetes, swarm clusters([#607](https://github.com/aliyun/terraform-provider-alicloud/issues/607))
- Add forcenew for ess lifecycle hook name and improve ess testcase by random name([#603](https://github.com/aliyun/terraform-provider-alicloud/issues/603))
- Improve ess configuration testcase([#600](https://github.com/aliyun/terraform-provider-alicloud/issues/600))
- Improve kvstore and ess schedule testcase([#599](https://github.com/aliyun/terraform-provider-alicloud/issues/599))
- Improve apigateway testcase([#593](https://github.com/aliyun/terraform-provider-alicloud/issues/593))
- Improve ram, ess schedule and cdn testcase([#592](https://github.com/aliyun/terraform-provider-alicloud/issues/592))
- Improve kvstore client token([#586](https://github.com/aliyun/terraform-provider-alicloud/issues/586))

BUG FIXES:

- Fix api gateway deleteing app bug([#633](https://github.com/aliyun/terraform-provider-alicloud/issues/633))
- Fix cs_kubernetes missing name error([#625](https://github.com/aliyun/terraform-provider-alicloud/issues/625))
- Fix api gateway groups filter bug([#624](https://github.com/aliyun/terraform-provider-alicloud/issues/624))
- Fix ots instance description force new bug([#616](https://github.com/aliyun/terraform-provider-alicloud/issues/616))
- Fix oss bucket object testcase destroy bug([#605](https://github.com/aliyun/terraform-provider-alicloud/issues/605))
- Fix deleting ess group timeout bug([#604](https://github.com/aliyun/terraform-provider-alicloud/issues/604))
- Fix deleting mns subscription bug([#601](https://github.com/aliyun/terraform-provider-alicloud/issues/601))
- bug fix for the input of cen bandwidth limit([#598](https://github.com/aliyun/terraform-provider-alicloud/issues/598))
- Fix log service timeout error([#594](https://github.com/aliyun/terraform-provider-alicloud/issues/594))
- Fix record not found issue if pvtz records are more than 50([#590](https://github.com/aliyun/terraform-provider-alicloud/issues/590))
- Fix cen instance and bandwidth multi regions test case bug([#588](https://github.com/aliyun/terraform-provider-alicloud/issues/588))

## 1.26.0 (December 20, 2018)

FEATURES:

- **New Resource:** `alicloud_cs_managed_kubernetes`([#563](https://github.com/aliyun/terraform-provider-alicloud/issues/563))

IMPROVEMENTS:

- Improve ram client endpoint([#584](https://github.com/aliyun/terraform-provider-alicloud/issues/584))
- Remove useless sweeper depencences for alicloud_instance sweeper testcase([#582](https://github.com/aliyun/terraform-provider-alicloud/issues/582))
- Improve kvstore backup policy testcase([#580](https://github.com/aliyun/terraform-provider-alicloud/issues/580))
- Improve the describing endpoint([#579](https://github.com/aliyun/terraform-provider-alicloud/issues/579))
- VPN gateway supports 200/500/1000M bandwidth([#577](https://github.com/aliyun/terraform-provider-alicloud/issues/577))
- skip private ip test in some regions([#575](https://github.com/aliyun/terraform-provider-alicloud/issues/575))
- Add timeout and retry for tablestore client and Improve its testcases([#569](https://github.com/aliyun/terraform-provider-alicloud/issues/569))
- Modify kvstore_instance password to Optional and improve its testcases([#567](https://github.com/aliyun/terraform-provider-alicloud/issues/567))
- Improve datasource alicloud_vpcs testcase([#566](https://github.com/aliyun/terraform-provider-alicloud/issues/566))
- Improve dns_domains testcase([#561](https://github.com/aliyun/terraform-provider-alicloud/issues/561))
- Improve ram_role_attachment testcase([#560](https://github.com/aliyun/terraform-provider-alicloud/issues/560))
- support PrePaid instances, image_id to be set when creating k8s clusters([#559](https://github.com/aliyun/terraform-provider-alicloud/issues/559))
- Add retry and timemout for fc client([#557](https://github.com/aliyun/terraform-provider-alicloud/issues/557))
- Datasource alicloud_zones supports filter FunctionCompute([#555](https://github.com/aliyun/terraform-provider-alicloud/issues/555))
- Fix a bug that caused the alicloud_dns_record.routing attribute([#554](https://github.com/aliyun/terraform-provider-alicloud/issues/554))
- Modify router interface prepaid test case  documentation([#552](https://github.com/aliyun/terraform-provider-alicloud/issues/552))
- Resource alicloud_ess_scalingconfiguration supports system_disk_size([#551](https://github.com/aliyun/terraform-provider-alicloud/issues/551))
- Improve datahub project testcase([#548](https://github.com/aliyun/terraform-provider-alicloud/issues/548))
- resource alicloud_slb_listener support server group([#545](https://github.com/aliyun/terraform-provider-alicloud/issues/545))
- Improve ecs instance and disk testcase with common case([#544](https://github.com/aliyun/terraform-provider-alicloud/issues/544))

BUG FIXES:

- Fix provider compile error on 32bit([#585](https://github.com/aliyun/terraform-provider-alicloud/issues/585))
- Fix table store no such host error with deleting and updating([#583](https://github.com/aliyun/terraform-provider-alicloud/issues/583))
- Fix pvtz_record RecordInvalidConflict bug([#581](https://github.com/aliyun/terraform-provider-alicloud/issues/581))
- fixed bug in backup policy update([#521](https://github.com/aliyun/terraform-provider-alicloud/issues/521))
- Fix docs eip_association([#578](https://github.com/aliyun/terraform-provider-alicloud/issues/578))
- Fix a bug about instance charge type change([#576](https://github.com/aliyun/terraform-provider-alicloud/issues/576))
- Fix describing endpoint failed error([#574](https://github.com/aliyun/terraform-provider-alicloud/issues/574))
- Fix table store describing no such host error([#572](https://github.com/aliyun/terraform-provider-alicloud/issues/572))
- Fix table store creating timeout error([#571](https://github.com/aliyun/terraform-provider-alicloud/issues/571))
- Fix kvstore instance class update error([#570](https://github.com/aliyun/terraform-provider-alicloud/issues/570))
- Fix ess_scaling_group import bugs and improve ess schedule testcase([#565](https://github.com/aliyun/terraform-provider-alicloud/issues/565))
- Fix alicloud rds related IncorrectStatus bug([#558](https://github.com/aliyun/terraform-provider-alicloud/issues/558))
- Fix alicloud_fc_trigger's config diff bug([#556](https://github.com/aliyun/terraform-provider-alicloud/issues/556))
- Fix oss bucket deleting failed error([#550](https://github.com/aliyun/terraform-provider-alicloud/issues/550))
- Fix potential bugs of datahub and ram when the resource has been deleted([#546](https://github.com/aliyun/terraform-provider-alicloud/issues/546))
- Fix pvtz_record describing bug([#543](https://github.com/aliyun/terraform-provider-alicloud/issues/543))

## 1.25.0 (November 30, 2018)

IMPROVEMENTS:

- return a empty list when there is no any data source([#540](https://github.com/aliyun/terraform-provider-alicloud/issues/540))
- Skip automatically the testcases which does not support API gateway([#538](https://github.com/aliyun/terraform-provider-alicloud/issues/538))
- Improve common bandwidth package test case and remove PayBy95([#530](https://github.com/aliyun/terraform-provider-alicloud/issues/530))
- Update resource drds supported regions([#534](https://github.com/aliyun/terraform-provider-alicloud/issues/534))
- Remove DB instance engine_version limitation([#528](https://github.com/aliyun/terraform-provider-alicloud/issues/528))
- Skip automatically the testcases which does not support route table and classic drds([#526](https://github.com/aliyun/terraform-provider-alicloud/issues/526))
- Skip automatically the testcases which does not support classic regions([#524](https://github.com/aliyun/terraform-provider-alicloud/issues/524))
- datasource alicloud_slbs support tags([#523](https://github.com/aliyun/terraform-provider-alicloud/issues/523))
- resouce alicloud_slb support tags([#522](https://github.com/aliyun/terraform-provider-alicloud/issues/522))
- Skip automatically the testcases which does not support multi az regions([#518](https://github.com/aliyun/terraform-provider-alicloud/issues/518))
- Add some region limitation guide for sone resources([#517](https://github.com/aliyun/terraform-provider-alicloud/issues/517))
- Skip automatically the testcases which does not support some known regions([#516](https://github.com/aliyun/terraform-provider-alicloud/issues/516))
- create instance with runinstances([#514](https://github.com/aliyun/terraform-provider-alicloud/issues/514))
- support eni amount in data source instance types([#512](https://github.com/aliyun/terraform-provider-alicloud/issues/512))
- Add a docs guides/getting-account to help user learn alibaba cloud account([#510](https://github.com/aliyun/terraform-provider-alicloud/issues/510))

BUG FIXES:

- Fix route_entry concurrence bug and improve it testcases([#537](https://github.com/aliyun/terraform-provider-alicloud/issues/537))
- Fix router interface prepaid purchase([#529](https://github.com/aliyun/terraform-provider-alicloud/issues/529))
- Fix fc_service sweeper test bug([#536](https://github.com/aliyun/terraform-provider-alicloud/issues/536))
- Fix drds creating VPC instance bug by adding vpc_id([#531](https://github.com/aliyun/terraform-provider-alicloud/issues/531))
- fix a snat_entry bug without set id to empty([#525](https://github.com/aliyun/terraform-provider-alicloud/issues/525))
- fix a bug of ram_use display name([#519](https://github.com/aliyun/terraform-provider-alicloud/issues/519))
- fix a bug of instance testcase([#513](https://github.com/aliyun/terraform-provider-alicloud/issues/513))
- Fix pvtz resource priority bug([#511](https://github.com/aliyun/terraform-provider-alicloud/issues/511))

## 1.24.0 (November 21, 2018)

FEATURES:

- **New Resource:** `alicloud_drds_instance`([#446](https://github.com/aliyun/terraform-provider-alicloud/issues/446))

IMPROVEMENTS:

- Improve drds_instance docs([#509](https://github.com/aliyun/terraform-provider-alicloud/issues/509))
- Add a new test case for drds_instance([#508](https://github.com/aliyun/terraform-provider-alicloud/issues/508))
- Improve provider config with Trim method([#504](https://github.com/aliyun/terraform-provider-alicloud/issues/504))
- api gateway skip app relevant tests([#500](https://github.com/aliyun/terraform-provider-alicloud/issues/500))
- update api resource that support to deploy api([#498](https://github.com/aliyun/terraform-provider-alicloud/issues/498))
- Skip ram_groups a test case([#496](https://github.com/aliyun/terraform-provider-alicloud/issues/496))
- support disk resize([#490](https://github.com/aliyun/terraform-provider-alicloud/issues/490))
- cancel the limit of system disk size([#489](https://github.com/aliyun/terraform-provider-alicloud/issues/489))
- Improve docs alicloud_db_database and alicloud_cs_kubernetes([#488](https://github.com/aliyun/terraform-provider-alicloud/issues/488))
- Support creating data disk with instance([#484](https://github.com/aliyun/terraform-provider-alicloud/issues/484))

BUG FIXES:

- Fix the sweeper test for CEN and CEN bandwidth package([#505](https://github.com/aliyun/terraform-provider-alicloud/issues/505))
- Fix pvtz_zone_record update bug([#503](https://github.com/aliyun/terraform-provider-alicloud/issues/503))
- Fix network_interface_attachment docs error([#502](https://github.com/aliyun/terraform-provider-alicloud/issues/502))
- fix fix datahub bug when visit region of ap-southeast-1([#499](https://github.com/aliyun/terraform-provider-alicloud/issues/499))
- Fix examples/mns-topic parameter error([#497](https://github.com/aliyun/terraform-provider-alicloud/issues/497))
- Fix db_connection not found error when deleting([#495](https://github.com/aliyun/terraform-provider-alicloud/issues/495))
- fix error about the docs format ([#492](https://github.com/aliyun/terraform-provider-alicloud/issues/492))

## 1.23.0 (November 13, 2018)

FEATURES:

- **New Resource:** `alicloud_api_gateway_app_attachment`([#478](https://github.com/aliyun/terraform-provider-alicloud/issues/478))
- **New Resource:** `alicloud_network_interface_attachment`([#474](https://github.com/aliyun/terraform-provider-alicloud/issues/474))
- **New Resource:** `alicloud_api_gateway_vpc_access`([#472](https://github.com/aliyun/terraform-provider-alicloud/issues/472))
- **New Resource:** `alicloud_network_interface`([#469](https://github.com/aliyun/terraform-provider-alicloud/issues/469))
- **New Resource:** `alicloud_common_bandwidth_package`([#468](https://github.com/aliyun/terraform-provider-alicloud/issues/468))
- **New Data Source:** `alicloud_network_interfaces`([#475](https://github.com/aliyun/terraform-provider-alicloud/issues/475))
- **New Data Source:** `alicloud_api_gateway_apps`([#467](https://github.com/aliyun/terraform-provider-alicloud/issues/467))

IMPROVEMENTS:

- Add a new region eu-west-1([#486](https://github.com/aliyun/terraform-provider-alicloud/issues/486))
- remove unreachable codes([#479](https://github.com/aliyun/terraform-provider-alicloud/issues/479))
- support enable/disable security enhancement strategy of alicloud_instance([#471](https://github.com/aliyun/terraform-provider-alicloud/issues/471))
- alicloud_slb_listener support idle_timeout/request_timeout([#463](https://github.com/aliyun/terraform-provider-alicloud/issues/463))

BUG FIXES:

- Fix cs_application cluster not found([#480](https://github.com/aliyun/terraform-provider-alicloud/issues/480))
- fix the bug of security_group inner_access bug([#477](https://github.com/aliyun/terraform-provider-alicloud/issues/477))
- Fix pagenumber built error([#470](https://github.com/aliyun/terraform-provider-alicloud/issues/470))
- Fix cs_application cluster not found([#480](https://github.com/aliyun/terraform-provider-alicloud/issues/480))

## 1.22.0 (November 02, 2018)

FEATURES:

- **New Resource:** `alicloud_api_gateway_api`([#457](https://github.com/aliyun/terraform-provider-alicloud/issues/457))
- **New Resource:** `alicloud_api_gateway_app`([#462](https://github.com/aliyun/terraform-provider-alicloud/issues/462))
- **New Reource:** `alicloud_common_bandwidth_package`([#454](https://github.com/aliyun/terraform-provider-alicloud/issues/454))
- **New Data Source:** `alicloud_api_gateway_apis`([#458](https://github.com/aliyun/terraform-provider-alicloud/issues/458))
- **New Data Source:** `cen_region_route_entries`([#442](https://github.com/aliyun/terraform-provider-alicloud/issues/442))
- **New Data Source:** `alicloud_slb_ca_certificates`([#452](https://github.com/aliyun/terraform-provider-alicloud/issues/452))

IMPROVEMENTS:

- Use product code to get common request domain([#466](https://github.com/aliyun/terraform-provider-alicloud/issues/466))
- KVstore instance password supports at sign([#465](https://github.com/aliyun/terraform-provider-alicloud/issues/465))
- Correct docs spelling error([#464](https://github.com/aliyun/terraform-provider-alicloud/issues/464))
- alicloud_log_service : support update project and shard auto spit([#461](https://github.com/aliyun/terraform-provider-alicloud/issues/461))
- Correct datasource alicloud_cen_route_entries docs error([#460](https://github.com/aliyun/terraform-provider-alicloud/issues/460))
- Remove CDN default configuration([#450](https://github.com/aliyun/terraform-provider-alicloud/issues/450))

BUG FIXES:

- set number of cen instances five for normal alicloud account testcases([#459](https://github.com/aliyun/terraform-provider-alicloud/issues/459))

## 1.21.0 (October 30, 2018)

FEATURES:

- **New Data Source:** `alicloud_slb_server_certificates`([#444](https://github.com/aliyun/terraform-provider-alicloud/issues/444))
- **New Data Source:** `alicloud_slb_acls`([#443](https://github.com/aliyun/terraform-provider-alicloud/issues/443))
- **New Resource:** `alicloud_slb_ca_certificate`([#438](https://github.com/aliyun/terraform-provider-alicloud/issues/438))
- **New Resource:** `alicloud_slb_server_certificate`([#436](https://github.com/aliyun/terraform-provider-alicloud/issues/436))

IMPROVEMENTS:

- resource alicloud_slb_listener tcp protocol support established_timeout parameter([#440](https://github.com/aliyun/terraform-provider-alicloud/issues/440))

BUG FIXES:

- Fix mns resource docs bug([#441](https://github.com/aliyun/terraform-provider-alicloud/issues/441))

## 1.20.0 (October 22, 2018)

FEATURES:

- **New Resource:** `alicloud_slb_acl`([#413](https://github.com/aliyun/terraform-provider-alicloud/issues/413))
- **New Resource:** `alicloud_cen_route_entry`([#415](https://github.com/aliyun/terraform-provider-alicloud/issues/415))
- **New Data Source:** `alicloud_cen_route_entries`([#424](https://github.com/aliyun/terraform-provider-alicloud/issues/424))

IMPROVEMENTS:

- Improve datahub_project sweeper test([#435](https://github.com/aliyun/terraform-provider-alicloud/issues/435))
- Modify mns test case name([#434](https://github.com/aliyun/terraform-provider-alicloud/issues/434))
- Improve fc_service sweeper test([#433](https://github.com/aliyun/terraform-provider-alicloud/issues/433))
- Support provider thread safety([#432](https://github.com/aliyun/terraform-provider-alicloud/issues/432))
- add tags to security group([#423](https://github.com/aliyun/terraform-provider-alicloud/issues/423))
- Resource router_interface support PrePaid([#425](https://github.com/aliyun/terraform-provider-alicloud/issues/425))
- resource alicloud_slb_listener support acl([#426](https://github.com/aliyun/terraform-provider-alicloud/issues/426))
- change child instance type Vbr to VBR and replace some const variables([#422](https://github.com/aliyun/terraform-provider-alicloud/issues/422))
- add slb_internet_enabled to Kubernetes Cluster([#421](https://github.com/aliyun/terraform-provider-alicloud/issues/421))
- Hide AliCloud HaVip Attachment resource docs because of it is not public totally([#420](https://github.com/aliyun/terraform-provider-alicloud/issues/420))
- Improve examples/ots-table([#417](https://github.com/aliyun/terraform-provider-alicloud/issues/417))
- Improve examples ecs-vpc, ecs-new-vpc and api-gateway([#416](https://github.com/aliyun/terraform-provider-alicloud/issues/416))

BUG FIXES:

- Fix reources' id description bugs([#428](https://github.com/aliyun/terraform-provider-alicloud/issues/428))
- Fix alicloud_ess_scaling_configuration setting data_disk failed([#427](https://github.com/aliyun/terraform-provider-alicloud/issues/427))

## 1.19.0 (October 13, 2018)

FEATURES:

- **New Resource:** `alicloud_api_gateway_group`([#409](https://github.com/aliyun/terraform-provider-alicloud/issues/409))
- **New Resource:** `alicloud_datahub_subscription`([#405](https://github.com/aliyun/terraform-provider-alicloud/issues/405))
- **New Resource:** `alicloud_datahub_topic`([#404](https://github.com/aliyun/terraform-provider-alicloud/issues/404))
- **New Resource:** `alicloud_datahub_project`([#403](https://github.com/aliyun/terraform-provider-alicloud/issues/403))
- **New Data Source:** `alicloud_api_gateway_groups`([#412](https://github.com/aliyun/terraform-provider-alicloud/issues/412))
- **New Data Source:** `alicloud_cen_bandwidth_limits`([#402](https://github.com/aliyun/terraform-provider-alicloud/issues/402))

IMPROVEMENTS:

- added need_slb attribute to cs swarm([#414](https://github.com/aliyun/terraform-provider-alicloud/issues/414))
- Add new example/datahub([#407](https://github.com/aliyun/terraform-provider-alicloud/issues/407))
- Add new example/datahub([#406](https://github.com/aliyun/terraform-provider-alicloud/issues/406))
- Format examples([#397](https://github.com/aliyun/terraform-provider-alicloud/issues/397))
- Add new example/kvstore([#396](https://github.com/aliyun/terraform-provider-alicloud/issues/396))
- Remove useless datasource cache file([#395](https://github.com/aliyun/terraform-provider-alicloud/issues/395))
- Add new example/pvtz([#394](https://github.com/aliyun/terraform-provider-alicloud/issues/394))
- Improve example/ecs-key-pair([#393](https://github.com/aliyun/terraform-provider-alicloud/issues/393))
- Change key pair file mode to 400([#392](https://github.com/aliyun/terraform-provider-alicloud/issues/392))

BUG FIXES:

- fix kubernetes's new_nat_gateway issue([#410](https://github.com/aliyun/terraform-provider-alicloud/issues/410))
- modify the mns err info([#400](https://github.com/aliyun/terraform-provider-alicloud/issues/400))
- Skip havip test case([#399](https://github.com/aliyun/terraform-provider-alicloud/issues/399))
- modify the sweeptest nameprefix([#398](https://github.com/aliyun/terraform-provider-alicloud/issues/398))

## 1.18.0 (October 09, 2018)

FEATURES:

- **New Resource:** `alicloud_havip`([#378](https://github.com/aliyun/terraform-provider-alicloud/issues/378))
- **New Resource:** `alicloud_havip_attachment`([#388](https://github.com/aliyun/terraform-provider-alicloud/issues/388))
- **New Resource:** `alicloud_mns_topic_subscription`([#376](https://github.com/aliyun/terraform-provider-alicloud/issues/376))
- **New Resource:** `alicloud_route_table_attachment`([#362](https://github.com/aliyun/terraform-provider-alicloud/issues/362))
- **New Resource:** `alicloud_cen_bandwidth_limit`([#361](https://github.com/aliyun/terraform-provider-alicloud/issues/361))
- **New Resource:** `alicloud_mns_topic`([#374](https://github.com/aliyun/terraform-provider-alicloud/issues/374))
- **New Resource:** `alicloud_mns_queue`([#365](https://github.com/aliyun/terraform-provider-alicloud/issues/365))
- **New Resource:** `alicloud_cen_bandwidth_package_attachment`([#354](https://github.com/aliyun/terraform-provider-alicloud/issues/354))
- **New Resource:** `alicloud_route_table`([#356](https://github.com/aliyun/terraform-provider-alicloud/issues/356))
- **New Data Source:** `alicloud_mns_queues`([#382](https://github.com/aliyun/terraform-provider-alicloud/issues/382))
- **New Data Source:** `alicloud_mns_topics`([#384](https://github.com/aliyun/terraform-provider-alicloud/issues/384))
- **New Data Source:** `alicloud_mns_topic_subscriptions`([#386](https://github.com/aliyun/terraform-provider-alicloud/issues/386))
- **New Data Source:** `alicloud_cen_bandwidth_packages`([#367](https://github.com/aliyun/terraform-provider-alicloud/issues/367))
- **New Data Source:** `alicloud_vpn_connections`([#366](https://github.com/aliyun/terraform-provider-alicloud/issues/366))
- **New Data Source:** `alicloud_vpn_gateways`([#363](https://github.com/aliyun/terraform-provider-alicloud/issues/363))
- **New Data Source:** `alicloud_vpn_customer_gateways`([#364](https://github.com/aliyun/terraform-provider-alicloud/issues/364))
- **New Data Source:** `alicloud_cen_instances`([#342](https://github.com/aliyun/terraform-provider-alicloud/issues/342))

IMPROVEMENTS:

- Improve resource ram_policy's document validatefunc([#385](https://github.com/aliyun/terraform-provider-alicloud/issues/385))
- RAM support useragent([#383](https://github.com/aliyun/terraform-provider-alicloud/issues/383))
- add node_cidr_mas and log_config, fix worker_data_disk issue([#368](https://github.com/aliyun/terraform-provider-alicloud/issues/368))
- Improve WaitForRouteTable and WaitForRouteTableAttachment method([#375](https://github.com/aliyun/terraform-provider-alicloud/issues/375))
- Correct Function Compute conn([#371](https://github.com/aliyun/terraform-provider-alicloud/issues/371))
- Improve datasource `images`'s docs([#370](https://github.com/aliyun/terraform-provider-alicloud/issues/370))
- add worker_data_disk_category and worker_data_disk_size to kubernetes creation([#355](https://github.com/aliyun/terraform-provider-alicloud/issues/355))

BUG FIXES:

- Fix alicloud_ram_user_policy_attachment EntityNotExist.User error([#381](https://github.com/aliyun/terraform-provider-alicloud/issues/381))
- Add parameter 'force_delete' to support deleting 'PrePaid' instance([#377](https://github.com/aliyun/terraform-provider-alicloud/issues/377))
- Add wait time to fix random detaching disk error([#373](https://github.com/aliyun/terraform-provider-alicloud/issues/373))
- Fix cen_instances markdown([#372](https://github.com/aliyun/terraform-provider-alicloud/issues/372))

## 1.17.0 (September 22, 2018)

FEATURES:

- **New Data Source:** `alicloud_fc_triggers`([#351](https://github.com/aliyun/terraform-provider-alicloud/pull/351))
- **New Data Source:** `alicloud_oss_bucket_objects`([#350](https://github.com/aliyun/terraform-provider-alicloud/pull/350))
- **New Data Source:** `alicloud_fc_functions`([#349](https://github.com/aliyun/terraform-provider-alicloud/pull/349))
- **New Data Source:** `alicloud_fc_services`([#348](https://github.com/aliyun/terraform-provider-alicloud/pull/348))
- **New Data Source:** `alicloud_oss_buckets`([#345](https://github.com/aliyun/terraform-provider-alicloud/pull/345))
- **New Data Source:** `alicloud_disks`([#343](https://github.com/aliyun/terraform-provider-alicloud/pull/343))
- **New Resource:** `alicloud_cen_bandwidth_package`([#333](https://github.com/aliyun/terraform-provider-alicloud/pull/333))

IMPROVEMENTS:

- Update OSS Resources' link to English([#352](https://github.com/aliyun/terraform-provider-alicloud/pull/352))
- Improve example/kubernetes to support multi-az([#344](https://github.com/aliyun/terraform-provider-alicloud/pull/344))

## 1.16.0 (September 16, 2018)

FEATURES:

- **New Resource:** `alicloud_cen_instance_attachment`([#327](https://github.com/aliyun/terraform-provider-alicloud/pull/327))

IMPROVEMENTS:

- Allow setting the scaling group balancing policy([#339](https://github.com/aliyun/terraform-provider-alicloud/pull/339))
- cs_kubernetes supports multi-az([#222](https://github.com/aliyun/terraform-provider-alicloud/pull/222))
- Improve client token using timestemp([#326](https://github.com/aliyun/terraform-provider-alicloud/pull/326))

BUG FIXES:

- Fix alicloud db connection([#341](https://github.com/aliyun/terraform-provider-alicloud/pull/341))
- Fix knstore productId([#338](https://github.com/aliyun/terraform-provider-alicloud/pull/338))
- Fix retriving kvstore multi zones bug([#337](https://github.com/aliyun/terraform-provider-alicloud/pull/337))
- Fix kvstore instance period bug([#335](https://github.com/aliyun/terraform-provider-alicloud/pull/335))
- Fix kvstore docs bug([#334](https://github.com/aliyun/terraform-provider-alicloud/pull/334))

## 1.15.0 (September 07, 2018)

FEATURES:

- **New Resource:** `alicloud_kvstore_backup_policy`([#331](https://github.com/aliyun/terraform-provider-alicloud/pull/331))
- **New Resource:** `alicloud_kvstore_instance`([#330](https://github.com/aliyun/terraform-provider-alicloud/pull/330))
- **New Data Source:** `alicloud_kvstore_instances`([#329](https://github.com/aliyun/terraform-provider-alicloud/pull/329))
- **New Resource:** `alicloud_ess_alarm`([#328](https://github.com/aliyun/terraform-provider-alicloud/pull/328))
- **New Resource:** `alicloud_ssl_vpn_client_cert`([#317](https://github.com/aliyun/terraform-provider-alicloud/pull/317))
- **New Resource:** `alicloud_cen_instance`([#312](https://github.com/aliyun/terraform-provider-alicloud/pull/312))
- **New Data Source:** `alicloud_slb_server_groups` ([#324](https://github.com/aliyun/terraform-provider-alicloud/pull/324))
- **New Data Source:** `alicloud_slb_rules` ([#323](https://github.com/aliyun/terraform-provider-alicloud/pull/323))
- **New Data Source:** `alicloud_slb_listeners` ([#323](https://github.com/aliyun/terraform-provider-alicloud/pull/323))
- **New Data Source:** `alicloud_slb_attachments` ([#322](https://github.com/aliyun/terraform-provider-alicloud/pull/322))
- **New Data Source:** `alicloud_slbs` ([#321](https://github.com/aliyun/terraform-provider-alicloud/pull/321))
- **New Data Source:** `alicloud_account` ([#319](https://github.com/aliyun/terraform-provider-alicloud/pull/319))
- **New Resource:** `alicloud_ssl_vpn_server`([#313](https://github.com/aliyun/terraform-provider-alicloud/pull/313))

IMPROVEMENTS:

- Support sweeper to clean some resources coming from failed testcases([#326](https://github.com/aliyun/terraform-provider-alicloud/pull/326))
- Improve function compute tst cases([#325](https://github.com/aliyun/terraform-provider-alicloud/pull/325))
- Improve fc test case using new datasource `alicloud_account`([#320](https://github.com/aliyun/terraform-provider-alicloud/pull/320))
- Base64 encode ESS scaling config user_data([#315](https://github.com/aliyun/terraform-provider-alicloud/pull/315))
- Retrieve the account_id automatically if needed([#314](https://github.com/aliyun/terraform-provider-alicloud/pull/314))

BUG FIXES:

- Fix DNS tests falied error([#318](https://github.com/aliyun/terraform-provider-alicloud/pull/318))
- Fix DB database not found error([#316](https://github.com/aliyun/terraform-provider-alicloud/pull/316))

## 1.14.0 (August 31, 2018)

FEATURES:

- **New Resource:** `alicloud_vpn_connection`([#304](https://github.com/aliyun/terraform-provider-alicloud/pull/304))
- **New Resource:** `alicloud_vpn_customer_gateway`([#299](https://github.com/aliyun/terraform-provider-alicloud/pull/299))

IMPROVEMENTS:

- Add 'force' to make key pair affect immediately([#310](https://github.com/aliyun/terraform-provider-alicloud/pull/310))
- Improve http proxy support([#307](https://github.com/aliyun/terraform-provider-alicloud/pull/307))
- Add flags to skip tests that use features not supported in all regions([#306](https://github.com/aliyun/terraform-provider-alicloud/pull/306))
- Improve data source dns_domains test case([#305](https://github.com/aliyun/terraform-provider-alicloud/pull/305))
- Change SDK config timeout([#302](https://github.com/aliyun/terraform-provider-alicloud/pull/302))
- Support ClientToken for some request([#301](https://github.com/aliyun/terraform-provider-alicloud/pull/301))
- Enlarge sdk default timeout to fix some timeout scenario([#300](https://github.com/aliyun/terraform-provider-alicloud/pull/300))

BUG FIXES:

- Fix container cluster SDK timezone error([#308](https://github.com/aliyun/terraform-provider-alicloud/pull/308))
- Fix network products throttling error([#303](https://github.com/aliyun/terraform-provider-alicloud/pull/303))

## 1.13.0 (August 28, 2018)

FEATURES:

- **New Resource:** `alicloud_vpn_gateway`([#298](https://github.com/aliyun/terraform-provider-alicloud/pull/298))
- **New Data Source:** `alicloud_mongo_instances`([#221](https://github.com/aliyun/terraform-provider-alicloud/pull/221))
- **New Data Source:** `alicloud_pvtz_zone_records`([#288](https://github.com/aliyun/terraform-provider-alicloud/pull/288))
- **New Data Source:** `alicloud_pvtz_zones`([#287](https://github.com/aliyun/terraform-provider-alicloud/pull/287))
- **New Resource:** `alicloud_pvtz_zone_record`([#286](https://github.com/aliyun/terraform-provider-alicloud/pull/286))
- **New Resource:** `alicloud_pvtz_zone_attachment`([#285](https://github.com/aliyun/terraform-provider-alicloud/pull/285))
- **New Resource:** `alicloud_pvtz_zone`([#284](https://github.com/aliyun/terraform-provider-alicloud/pull/284))
- **New Resource:** `alicloud_ess_lifecycle_hook`([#283](https://github.com/aliyun/terraform-provider-alicloud/pull/283))
- **New Data Source:** `alicloud_router_interfaces`([#269](https://github.com/aliyun/terraform-provider-alicloud/pull/269))

IMPROVEMENTS:

- Check pvtzconn error([#295](https://github.com/aliyun/terraform-provider-alicloud/pull/295))
- For internationalize tests([#294](https://github.com/aliyun/terraform-provider-alicloud/pull/294))
- Improve data source docs([#293](https://github.com/aliyun/terraform-provider-alicloud/pull/293))
- Add SLB PayByBandwidth test case([#292](https://github.com/aliyun/terraform-provider-alicloud/pull/292))
- Update vpc sdk to support new resource VPN gateway([#291](https://github.com/aliyun/terraform-provider-alicloud/pull/291))
- Improve snat entry test case([#290](https://github.com/aliyun/terraform-provider-alicloud/pull/290))
- Allow empty list of SLBs as arg to ESG([#289](https://github.com/aliyun/terraform-provider-alicloud/pull/289))
- Improve docs vroute_entry([#281](https://github.com/aliyun/terraform-provider-alicloud/pull/281))
- Improve examples/router_interface([#278](https://github.com/aliyun/terraform-provider-alicloud/pull/278))
- Improve SLB instance test case([#274](https://github.com/aliyun/terraform-provider-alicloud/pull/274))
- Improve alicloud_router_interface's test case([#272](https://github.com/aliyun/terraform-provider-alicloud/pull/272))
- Improve data source alicloud_regions's test case([#271](https://github.com/aliyun/terraform-provider-alicloud/pull/271))
- Add notes about ordering between two alicloud_router_interface_connections([#270](https://github.com/aliyun/terraform-provider-alicloud/pull/270))
- Improve docs spelling error([#268](https://github.com/aliyun/terraform-provider-alicloud/pull/268))
- ECS instance support more tags and update instance test cases([#267](https://github.com/aliyun/terraform-provider-alicloud/pull/267))
- Improve OSS bucket test case([#266](https://github.com/aliyun/terraform-provider-alicloud/pull/266))
- Fixing a broken link([#265](https://github.com/aliyun/terraform-provider-alicloud/pull/265))
- Allow creation of slb vserver group with 0 servers([#264](https://github.com/aliyun/terraform-provider-alicloud/pull/264))
- Improve SLB test cases results from international regions does support PayByBandwidth and ' Guaranteed-performance' instance([#263](https://github.com/aliyun/terraform-provider-alicloud/pull/263))
- Improve EIP test cases results from international regions does support PayByBandwidth([#262](https://github.com/aliyun/terraform-provider-alicloud/pull/262))
- Improve ESS test cases results from some region does support Classic Network([#261](https://github.com/aliyun/terraform-provider-alicloud/pull/261))
- Recover nat gateway bandwidth pacakges to meet stock user requirements([#260](https://github.com/aliyun/terraform-provider-alicloud/pull/260))
- Resource alicloud_slb_listener supports new field 'x-forwarded-for'([#259](https://github.com/aliyun/terraform-provider-alicloud/pull/259))
- Resource alicloud_slb_listener supports new field 'gzip'([#258](https://github.com/aliyun/terraform-provider-alicloud/pull/258))

BUG FIXES:

- Fix getting oss endpoint timeout error([#282](https://github.com/aliyun/terraform-provider-alicloud/pull/282))
- Fix router interface connection error when 'opposite_interface_owner_id' is empty([#277](https://github.com/aliyun/terraform-provider-alicloud/pull/277))
- Fix router interface connection error and deleting error([#275](https://github.com/aliyun/terraform-provider-alicloud/pull/275))
- Fix disk detach error and improve test using dynamic zone and region([#273](https://github.com/aliyun/terraform-provider-alicloud/pull/273))

## 1.12.0 (August 10, 2018)

IMPROVEMENTS:

- Improve `make build`([#256](https://github.com/aliyun/terraform-provider-alicloud/pull/256))
- Improve examples slb and slb-vpc by modifying 'paybytraffic' to 'PayByTraffic'([#256](https://github.com/aliyun/terraform-provider-alicloud/pull/256))
- Improve example/router-interface by adding resource alicloud_router_interface_connection([#255](https://github.com/aliyun/terraform-provider-alicloud/pull/255))
- Support more specification of router interface([#253](https://github.com/aliyun/terraform-provider-alicloud/pull/253))
- Improve resource alicloud_fc_service docs([#252](https://github.com/aliyun/terraform-provider-alicloud/pull/252))
- Modify resource alicloud_fc_function 'handler' is required([#251](https://github.com/aliyun/terraform-provider-alicloud/pull/251))
- Resource alicloud_router_interface support "import" function([#249](https://github.com/aliyun/terraform-provider-alicloud/pull/249))
- Deprecate some field of alicloud_router_interface fields and use new resource instead([#248](https://github.com/aliyun/terraform-provider-alicloud/pull/248))
- *New Resource*: _alicloud_router_interface_connection_([#247](https://github.com/aliyun/terraform-provider-alicloud/pull/247))

BUG FIXES:

- Fix network resource throttling error([#257](https://github.com/aliyun/terraform-provider-alicloud/pull/257))
- Fix resource alicloud_fc_trigger "source_arn" inputting empty error([#253](https://github.com/aliyun/terraform-provider-alicloud/pull/253))
- Fix describing vpcs with name_regex no results error([#250](https://github.com/aliyun/terraform-provider-alicloud/pull/250))
- Fix creating slb listener in international region failed error([#246](https://github.com/aliyun/terraform-provider-alicloud/pull/246))

## 1.11.0 (August 08, 2018)

IMPROVEMENTS:

- Resource alicloud_eip support name and description([#244](https://github.com/aliyun/terraform-provider-alicloud/pull/244))
- Resource alicloud_eip support PrePaid([#243](https://github.com/aliyun/terraform-provider-alicloud/pull/243))
- Correct version writing error([#241](https://github.com/aliyun/terraform-provider-alicloud/pull/241))
- Change slb go sdk to official repo([#240](https://github.com/aliyun/terraform-provider-alicloud/pull/240))
- Remove useless file website/fc_service.html.markdown([#239](https://github.com/aliyun/terraform-provider-alicloud/pull/239))
- Update Go version to 1.10.1 to match new sdk([#237](https://github.com/aliyun/terraform-provider-alicloud/pull/237))
- Support http(s) proxy([#236](https://github.com/aliyun/terraform-provider-alicloud/pull/236))
- Add guide for installing goimports([#233](https://github.com/aliyun/terraform-provider-alicloud/pull/233))
- Improve the makefile and README([#232](https://github.com/aliyun/terraform-provider-alicloud/pull/232))

BUG FIXES:

- Fix losing key pair error after updating ecs instance([#245](https://github.com/aliyun/terraform-provider-alicloud/pull/245))
- Fix BackendServer Configuring error when creating slb rule([#242](https://github.com/aliyun/terraform-provider-alicloud/pull/242))
- Fix bug "...zoneinfo.zip: no such file or directory" happened in windows.([#238](https://github.com/aliyun/terraform-provider-alicloud/pull/238))
- Fix ess_scalingrule InvalidScalingRuleId.NotFound error([#234](https://github.com/aliyun/terraform-provider-alicloud/pull/234))

## 1.10.0 (July 27, 2018)

IMPROVEMENTS:

- Rds supports to create 10.0 PostgreSQL instance.([#230](https://github.com/aliyun/terraform-provider-alicloud/pull/230))
- *New Resource*: _alicloud_fc_trigger_([#228](https://github.com/aliyun/terraform-provider-alicloud/pull/228))
- *New Resource*: _alicloud_fc_function_([#227](https://github.com/aliyun/terraform-provider-alicloud/pull/227))
- *New Resource*: _alicloud_fc_service_ 30([#226](https://github.com/aliyun/terraform-provider-alicloud/pull/226))
- Support new field 'instance_name' for _alicloud_ots_table_([#225](https://github.com/aliyun/terraform-provider-alicloud/pull/225))
- *New Resource*: _alicloud_ots_instance_attachment_([#224](https://github.com/aliyun/terraform-provider-alicloud/pull/224))
- *New Resource*: _alicloud_ots_instance_([#223](https://github.com/aliyun/terraform-provider-alicloud/pull/223))

BUG FIXES:

- Fix Snat entry not found error([#229](https://github.com/aliyun/terraform-provider-alicloud/pull/229))

## 1.9.6 (July 24, 2018)

IMPROVEMENTS:

- Remove the number limitation of vswitch_ids, slb_ids and db_instance_ids([#219](https://github.com/aliyun/terraform-provider-alicloud/pull/219))
- Reduce test nat gateway cost([#218](https://github.com/aliyun/terraform-provider-alicloud/pull/218))
- Support creating zero-node swarm cluster([#217](https://github.com/aliyun/terraform-provider-alicloud/pull/217))
- Improve security group and rule data source test case([#216](https://github.com/aliyun/terraform-provider-alicloud/pull/216))
- Improve dns record resource test case([#215](https://github.com/aliyun/terraform-provider-alicloud/pull/215))
- Improve test case destroy method([#214](https://github.com/aliyun/terraform-provider-alicloud/pull/214))
- Improve ecs instance resource test case([#213](https://github.com/aliyun/terraform-provider-alicloud/pull/213))
- Improve cdn resource test case([#212](https://github.com/aliyun/terraform-provider-alicloud/pull/212))
- Improve kms resource test case([#211](https://github.com/aliyun/terraform-provider-alicloud/pull/211))
- Improve key pair resource test case([#210](https://github.com/aliyun/terraform-provider-alicloud/pull/210))
- Improve rds resource test case([#209](https://github.com/aliyun/terraform-provider-alicloud/pull/209))
- Improve disk resource test case([#208](https://github.com/aliyun/terraform-provider-alicloud/pull/208))
- Improve eip resource test case([#207](https://github.com/aliyun/terraform-provider-alicloud/pull/207))
- Improve scaling service resource test case([#206](https://github.com/aliyun/terraform-provider-alicloud/pull/206))
- Improve vpc and vswitch resource test case([#205](https://github.com/aliyun/terraform-provider-alicloud/pull/205))
- Improve slb resource test case([#204](https://github.com/aliyun/terraform-provider-alicloud/pull/204))
- Improve security group resource test case([#203](https://github.com/aliyun/terraform-provider-alicloud/pull/203))
- Improve ram resource test case([#202](https://github.com/aliyun/terraform-provider-alicloud/pull/202))
- Improve container cluster resource test case([#201](https://github.com/aliyun/terraform-provider-alicloud/pull/201))
- Improve cloud monitor resource test case([#200](https://github.com/aliyun/terraform-provider-alicloud/pull/200))
- Improve route and router interface resource test case([#199](https://github.com/aliyun/terraform-provider-alicloud/pull/199))
- Improve dns resource test case([#198](https://github.com/aliyun/terraform-provider-alicloud/pull/198))
- Improve oss resource test case([#197](https://github.com/aliyun/terraform-provider-alicloud/pull/197))
- Improve ots table resource test case([#196](https://github.com/aliyun/terraform-provider-alicloud/pull/196))
- Improve nat gateway resource test case([#195](https://github.com/aliyun/terraform-provider-alicloud/pull/195))
- Improve log resource test case([#194](https://github.com/aliyun/terraform-provider-alicloud/pull/194))
- Support changing ecs charge type from Prepaid to PostPaid([#192](https://github.com/aliyun/terraform-provider-alicloud/pull/192))
- Add method to compare json template is equal([#187](https://github.com/aliyun/terraform-provider-alicloud/pull/187))
- Remove useless file([#191](https://github.com/aliyun/terraform-provider-alicloud/pull/191))

BUG FIXES:

- Fix CS kubernetes read error and CS app timeout([#217](https://github.com/aliyun/terraform-provider-alicloud/pull/217))
- Fix getting location connection error([#193](https://github.com/aliyun/terraform-provider-alicloud/pull/193))
- Fix CS kubernetes connection error([#190](https://github.com/aliyun/terraform-provider-alicloud/pull/190))
- Fix Oss bucket diff error([#189](https://github.com/aliyun/terraform-provider-alicloud/pull/189))

NOTES:

- From version 1.9.6, the deprecated resource alicloud_ram_alias file has been removed and the resource has been
replaced by alicloud_ram_account_alias. Details refer to [pull 191](https://github.com/aliyun/terraform-provider-alicloud/pull/191/commits/e3fd74591230ccb545bb4309b674d6df33b716b9)

## 1.9.5 (June 20, 2018)

IMPROVEMENTS:

- Improve log machine group docs([#186](https://github.com/aliyun/terraform-provider-alicloud/pull/186))
- Support sts token for some resources([#185](https://github.com/aliyun/terraform-provider-alicloud/pull/185))
- Support user agent for log service([#184](https://github.com/aliyun/terraform-provider-alicloud/pull/184))
- *New Resource*: _alicloud_log_machine_group_([#183](https://github.com/aliyun/terraform-provider-alicloud/pull/183))
- *New Resource*: _alicloud_log_store_index_([#182](https://github.com/aliyun/terraform-provider-alicloud/pull/182))
- *New Resource*: _alicloud_log_store_([#181](https://github.com/aliyun/terraform-provider-alicloud/pull/181))
- *New Resource*: _alicloud_log_project_([#180](https://github.com/aliyun/terraform-provider-alicloud/pull/180))
- Improve example about cs_kubernetes([#179](https://github.com/aliyun/terraform-provider-alicloud/pull/179))
- Add losing docs about cs_kubernetes([#178](https://github.com/aliyun/terraform-provider-alicloud/pull/178))

## 1.9.4 (June 08, 2018)

IMPROVEMENTS:

- cs_kubernetes supports output worker nodes and master nodes([#177](https://github.com/aliyun/terraform-provider-alicloud/pull/177))
- cs_kubernetes supports to output kube config and certificate([#176](https://github.com/aliyun/terraform-provider-alicloud/pull/176))
- Add a example to deploy mysql and wordpress on kubernetes([#175](https://github.com/aliyun/terraform-provider-alicloud/pull/175))
- Add a example to create swarm and deploy wordpress on it([#174](https://github.com/aliyun/terraform-provider-alicloud/pull/174))
- Change ECS and ESS sdk to official go sdk([#173](https://github.com/aliyun/terraform-provider-alicloud/pull/173))


## 1.9.3 (May 27, 2018)

IMPROVEMENTS:

- *New Data Source*: _alicloud_db_instances_([#161](https://github.com/aliyun/terraform-provider-alicloud/pull/161))
- Support to set auto renew for ECS instance([#172](https://github.com/aliyun/terraform-provider-alicloud/pull/172))
- Improve cs_kubernetes, slb_listener and db_database docs([#171](https://github.com/aliyun/terraform-provider-alicloud/pull/171))
- Add missing code for describing RDS zones([#170](https://github.com/aliyun/terraform-provider-alicloud/pull/170))
- Add docs notes for windows os([#169](https://github.com/aliyun/terraform-provider-alicloud/pull/169))
- Add filter parameters and export parameters for instance types data source.([#168](https://github.com/aliyun/terraform-provider-alicloud/pull/168))
- Add filter parameters for zones data source.([#167](https://github.com/aliyun/terraform-provider-alicloud/pull/167))
- Remove kubernetes work_number limitation([#165](https://github.com/aliyun/terraform-provider-alicloud/pull/165))
- Improve kubernetes examples([#163](https://github.com/aliyun/terraform-provider-alicloud/pull/163))

BUG FIXES:

- Fix getting some instance types failed bug([#166](https://github.com/aliyun/terraform-provider-alicloud/pull/166))
- Fix kubernetes out range index error([#164](https://github.com/aliyun/terraform-provider-alicloud/pull/164))

## 1.9.2 (May 09, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_ots_table_([#162](https://github.com/aliyun/terraform-provider-alicloud/pull/162))
- Fix SLB listener "OperationBusy" error([#159](https://github.com/aliyun/terraform-provider-alicloud/pull/159))
- Prolong waiting time for creating kubernetes cluster to avoid timeout([#158](https://github.com/aliyun/terraform-provider-alicloud/pull/158))
- Support load endpoint from environment variable or specified file([#157](https://github.com/aliyun/terraform-provider-alicloud/pull/157))
- Update example([#155](https://github.com/aliyun/terraform-provider-alicloud/pull/155))

BUG FIXES:

- Fix modifying instance host name failed bug([#160](https://github.com/aliyun/terraform-provider-alicloud/pull/160))
- Fix SLB listener "OperationBusy" error([#159](https://github.com/aliyun/terraform-provider-alicloud/pull/159))
- Fix deleting forward table not found error([#154](https://github.com/aliyun/terraform-provider-alicloud/pull/154))
- Fix deleting slb listener error([#150](https://github.com/aliyun/terraform-provider-alicloud/pull/150))
- Fix creating vswitch error([#149](https://github.com/aliyun/terraform-provider-alicloud/pull/149))

## 1.9.1 (April 13, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_cms_alarm_([#146](https://github.com/aliyun/terraform-provider-alicloud/pull/146))
- *New Resource*: _alicloud_cs_application_([#136](https://github.com/aliyun/terraform-provider-alicloud/pull/136))
- *New Datasource*: _alicloud_security_group_rules_([#135](https://github.com/aliyun/terraform-provider-alicloud/pull/135))
- Output application attribution service block([#141](https://github.com/aliyun/terraform-provider-alicloud/pull/141))
- Output swarm attribution 'vpc_id'([#140](https://github.com/aliyun/terraform-provider-alicloud/pull/140))
- Support to release eip after deploying swarm cluster.([#139](https://github.com/aliyun/terraform-provider-alicloud/pull/139))
- Output swarm and kubernetes's nodes information and other attribution([#138](https://github.com/aliyun/terraform-provider-alicloud/pull/138))
- Modify `size` to `node_number`([#137](https://github.com/aliyun/terraform-provider-alicloud/pull/137))
- Set swarm ID before waiting its status([#134](https://github.com/aliyun/terraform-provider-alicloud/pull/134))
- Add 'is_outdated' for cs_swarm and cs_kubernetes([#133](https://github.com/aliyun/terraform-provider-alicloud/pull/133))
- Add warning when creating postgresql and ppas database([#132](https://github.com/aliyun/terraform-provider-alicloud/pull/132))
- Add kubernetes example([#142](https://github.com/aliyun/terraform-provider-alicloud/pull/142))
- Update sdk to support user-agent([#143](https://github.com/aliyun/terraform-provider-alicloud/pull/143))
- Add eip unassociation retry times to avoid needless error([#144](https://github.com/aliyun/terraform-provider-alicloud/pull/144))
- Add connections output for kubernetes cluster([#145](https://github.com/aliyun/terraform-provider-alicloud/pull/145))

BUG FIXES:

- Fix vpc not found when vpc has been deleted([#131](https://github.com/aliyun/terraform-provider-alicloud/pull/131))


## 1.9.0 (March 19, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_cs_kubernetes_([#129](https://github.com/aliyun/terraform-provider-alicloud/pull/129))
- *New DataSource*: _alicloud_eips_([#123](https://github.com/aliyun/terraform-provider-alicloud/pull/123))
- Add server_group_id to slb listener resource([#122](https://github.com/aliyun/terraform-provider-alicloud/pull/122))
- Rename _alicloud_container_cluster_ to _alicloud_cs_swarm_([#128](https://github.com/aliyun/terraform-provider-alicloud/pull/128))

BUG FIXES:

- Fix vpc description validate([#125](https://github.com/aliyun/terraform-provider-alicloud/pull/125))
- Update SDK version to fix unresolving endpoint issue([#126](https://github.com/aliyun/terraform-provider-alicloud/pull/126))
- Add waiting time after ECS bind ECS to ensure network is ok([#127](https://github.com/aliyun/terraform-provider-alicloud/pull/127))

## 1.8.1 (March 09, 2018)

IMPROVEMENTS:

- DB instance supports multiple zone([#120](https://github.com/aliyun/terraform-provider-alicloud/pull/120))
- Data source zones support to retrieve multiple zone([#119](https://github.com/aliyun/terraform-provider-alicloud/pull/119))
- VPC supports alibaba cloud official go sdk([#118](https://github.com/aliyun/terraform-provider-alicloud/pull/118))

BUG FIXES:

- Fix not found db instance bug when allocating connection([#121](https://github.com/aliyun/terraform-provider-alicloud/pull/121))


## 1.8.0 (March 02, 2018)

IMPROVEMENTS:

- Support golang version 1.9([#114](https://github.com/aliyun/terraform-provider-alicloud/pull/114))
- RDS supports alibaba cloud official go sdk([#113](https://github.com/aliyun/terraform-provider-alicloud/pull/113))
- Deprecated 'in_use' in eips datasource to fix conflict([#115](https://github.com/aliyun/terraform-provider-alicloud/pull/115))
- Add encrypted argument to alicloud_disk resource（[#116](https://github.com/aliyun/terraform-provider-alicloud/pull/116))

BUG FIXES:

- Fix reading router interface failed bug([#117](https://github.com/aliyun/terraform-provider-alicloud/pull/117))

## 1.7.2 (February 09, 2018)

IMPROVEMENTS:

- *New DataSource*: _alicloud_eips_([#110](https://github.com/aliyun/terraform-provider-alicloud/pull/110))
- *New DataSource*: _alicloud_vswitches_([#109](https://github.com/aliyun/terraform-provider-alicloud/pull/109))
- Support inner network segregation in one security group([#112](https://github.com/aliyun/terraform-provider-alicloud/pull/112))

BUG FIXES:

- Fix creating Classic instance failed result in role_name([#111](https://github.com/aliyun/terraform-provider-alicloud/pull/111))
- Fix eip is not exist in nat gateway when creating snat([#108](https://github.com/aliyun/terraform-provider-alicloud/pull/108))

## 1.7.1 (February 02, 2018)

IMPROVEMENTS:

- Support setting instance_name for ESS scaling configuration([#107](https://github.com/aliyun/terraform-provider-alicloud/pull/107))
- Support multiple vswitches for ESS scaling group and output slbIds and dbIds([#105](https://github.com/aliyun/terraform-provider-alicloud/pull/105))
- Support to set internet_max_bandwidth_out is 0 for ESS configuration([#103](https://github.com/aliyun/terraform-provider-alicloud/pull/103))
- Modify EIP default to PayByTraffic for international account([#101](https://github.com/aliyun/terraform-provider-alicloud/pull/101))
- Deprecate nat gateway fileds 'spec' and 'bandwidth_packages'([#100](https://github.com/aliyun/terraform-provider-alicloud/pull/100))
- Support to associate EIP with SLB and Nat Gateway([#99](https://github.com/aliyun/terraform-provider-alicloud/pull/99))

BUG FIXES:

- fix a bug that can't create multiple VPC, vswitch and nat gateway at one time([#102](https://github.com/aliyun/terraform-provider-alicloud/pull/102))
- fix a bug that can't import instance 'role_name'([#104](https://github.com/aliyun/terraform-provider-alicloud/pull/104))
- fix a bug that creating ESS scaling group and configuration results from 'Throttling'([#106](https://github.com/aliyun/terraform-provider-alicloud/pull/106))

## 1.7.0 (January 25, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_kms_key_([#91](https://github.com/aliyun/terraform-provider-alicloud/pull/91))
- *New DataSource*: _alicloud_kms_keys_([#93](https://github.com/aliyun/terraform-provider-alicloud/pull/93))
- *New DataSource*: _alicloud_instances_([#94](https://github.com/aliyun/terraform-provider-alicloud/pull/94))
- Add a new output field "arn" for _alicloud_kms_key_([#92](https://github.com/aliyun/terraform-provider-alicloud/pull/92))
- Add a new field "specification" for _alicloud_slb_([#95](https://github.com/aliyun/terraform-provider-alicloud/pull/95))
- Improve security group rule's port range for "-1/-1"([#96](https://github.com/aliyun/terraform-provider-alicloud/pull/96))

BUG FIXES:

- fix slb invalid status error when launching ESS scaling group([#97](https://github.com/aliyun/terraform-provider-alicloud/pull/97))

## 1.6.2 (January 22, 2018)

IMPROVEMENTS:

- Modify db_connection prefix default value to "instance_id + 'tf'"([#90](https://github.com/aliyun/terraform-provider-alicloud/pull/90))
- Modify db_connection ID to make it more simple while importing it([#90](https://github.com/aliyun/terraform-provider-alicloud/pull/90))
- Add wait method to avoid useless status error while creating/modifying account or privilege or connection or database([#90](https://github.com/aliyun/terraform-provider-alicloud/pull/90))
- Support to set instnace name for RDS([#88](https://github.com/aliyun/terraform-provider-alicloud/pull/88))
- Avoid container cluster cidr block conflicts with vswitch's([#88](https://github.com/aliyun/terraform-provider-alicloud/pull/88))
- Output resource import information([#87](https://github.com/aliyun/terraform-provider-alicloud/pull/87))

BUG FIXES:

- fix instance id not found and instane status not supported bug([#90](https://github.com/aliyun/terraform-provider-alicloud/pull/90))
- fix deleting slb_attachment resource failed bug([#86](https://github.com/aliyun/terraform-provider-alicloud/pull/86))


## 1.6.1 (January 18, 2018)

IMPROVEMENTS:

- Support to modify instance type and network spec([#84](https://github.com/aliyun/terraform-provider-alicloud/pull/84))
- Avoid needless error when creating security group rule([#83](https://github.com/aliyun/terraform-provider-alicloud/pull/83))

BUG FIXES:

- fix creating cluster container failed bug([#85](https://github.com/aliyun/terraform-provider-alicloud/pull/85))


## 1.6.0 (January 15, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_ess_attachment_([#80](https://github.com/aliyun/terraform-provider-alicloud/pull/80))
- *New Resource*: _alicloud_slb_rule_([#79](https://github.com/aliyun/terraform-provider-alicloud/pull/79))
- *New Resource*: _alicloud_slb_server_group_([#78](https://github.com/aliyun/terraform-provider-alicloud/pull/78))
- Support Spot Instance([#77](https://github.com/aliyun/terraform-provider-alicloud/pull/77))
- Output tip message when international account create SLB failed([#75](https://github.com/aliyun/terraform-provider-alicloud/pull/75))
- Standardize the order of imports packages([#74](https://github.com/aliyun/terraform-provider-alicloud/pull/74))
- Add "weight" for slb_attachment to improve the resource([#81](https://github.com/aliyun/terraform-provider-alicloud/pull/81))

BUG FIXES:

- fix allocating RDS public connection conflict error([#76](https://github.com/aliyun/terraform-provider-alicloud/pull/76))

## 1.5.3 (January 9, 2018)

BUG FIXES:
  * fix getting OSS endpoint failed error ([#73](https://github.com/aliyun/terraform-provider-alicloud/pull/73))
  * fix describing dns record not found when deleting record([#73](https://github.com/aliyun/terraform-provider-alicloud/pull/73))

## 1.5.2 (January 8, 2018)

BUG FIXES:
  * fix creating rds 'Prepaid' instance failed error ([#70](https://github.com/aliyun/terraform-provider-alicloud/pull/70))

## 1.5.1 (January 5, 2018)

BUG FIXES:
  * modify security_token to Optional([#69](https://github.com/aliyun/terraform-provider-alicloud/pull/69))

## 1.5.0 (January 4, 2018)

IMPROVEMENTS:

- *New Resource*: _alicloud_db_database_([#68](https://github.com/aliyun/terraform-provider-alicloud/pull/68))
- *New Resource*: _alicloud_db_backup_policy_([#68](https://github.com/aliyun/terraform-provider-alicloud/pull/68))
- *New Resource*: _alicloud_db_connection_([#67](https://github.com/aliyun/terraform-provider-alicloud/pull/67))
- *New Resource*: _alicloud_db_account_([#66](https://github.com/aliyun/terraform-provider-alicloud/pull/66))
- *New Resource*: _alicloud_db_account_privilege_([#66](https://github.com/aliyun/terraform-provider-alicloud/pull/66))
- resource/db_instance: remove some field to new resource([#65](https://github.com/aliyun/terraform-provider-alicloud/pull/65))
- resource/instance: support to modify private ip, vswitch_id and instance charge type([#65](https://github.com/aliyun/terraform-provider-alicloud/pull/65))

BUG FIXES:

- resource/dns-record: Fix dns record still exist after deleting it([#65](https://github.com/aliyun/terraform-provider-alicloud/pull/65))
- resource/instance: fix deleting route entry error([#69](https://github.com/aliyun/terraform-provider-alicloud/pull/69))


## 1.2.0 (December 15, 2017)

IMPROVEMENTS:
- resource/slb: wait for SLB active before return back([#61](https://github.com/aliyun/terraform-provider-alicloud/pull/61))

BUG FIXES:

- resource/dns-record: Fix setting dns priority failed([#58](https://github.com/aliyun/terraform-provider-alicloud/pull/58))
- resource/dns-record: Fix ESS attachs SLB failed([#59](https://github.com/aliyun/terraform-provider-alicloud/pull/59))
- resource/dns-record: Fix security group not found error([#59](https://github.com/aliyun/terraform-provider-alicloud/pull/59))


## 1.0.0 (December 11, 2017)

IMPROVEMENTS:

- *New Resource*: _alicloud_slb_listener_([#53](https://github.com/aliyun/terraform-provider-alicloud/pull/53))
- *New Resource*: _alicloud_cdn_domain_([#52](https://github.com/aliyun/terraform-provider-alicloud/pull/52))
- *New Resource*: _alicloud_dns_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- *New Resource*: _alicloud_dns_group_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- *New Resource*: _alicloud_dns_record_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- *New Resource*: _alicloud_ram_account_alias_([#50](https://github.com/aliyun/terraform-provider-alicloud/pull/50))
- *New Resource*: _alicloud_ram_login_profile_([#50](https://github.com/aliyun/terraform-provider-alicloud/pull/50))
- *New Resource*: _alicloud_ram_access_key_([#50](https://github.com/aliyun/terraform-provider-alicloud/pull/50))
- *New Resource*: _alicloud_ram_group_([#49](https://github.com/aliyun/terraform-provider-alicloud/pull/49))
- *New Resource*: _alicloud_ram_group_membership_([#49](https://github.com/aliyun/terraform-provider-alicloud/pull/49))
- *New Resource*: _alicloud_ram_group_policy_attachment_([#49](https://github.com/aliyun/terraform-provider-alicloud/pull/49))
- *New Resource*: _alicloud_ram_role_([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
- *New Resource*: _alicloud_ram_role_attachment_([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
- *New Resource*: _alicloud_ram_role_polocy_attachment_([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
- *New Resource*: _alicloud_container_cluster_([#47](https://github.com/aliyun/terraform-provider-alicloud/pull/47))
- *New Resource:* _alicloud_ram_policy_([#46](https://github.com/aliyun/terraform-provider-alicloud/pull/46))
- *New Resource*: _alicloud_ram_user_policy_attachment_([#46](https://github.com/aliyun/terraform-provider-alicloud/pull/46))
- *New Resource* _alicloud_ram_user_([#44](https://github.com/aliyun/terraform-provider-alicloud/pull/44))
- *New Datasource* _alicloud_ram_policies_([#46](https://github.com/aliyun/terraform-provider-alicloud/pull/46))
- *New Datasource* _alicloud_ram_users_([#44](https://github.com/aliyun/terraform-provider-alicloud/pull/44))
- *New Datasource*: _alicloud_ram_roles_([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
- *New Datasource*: _alicloud_ram_account_aliases_([#50](https://github.com/aliyun/terraform-provider-alicloud/pull/50))
- *New Datasource*: _alicloud_dns_domains_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- *New Datasource*: _alicloud_dns_groups_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- *New Datasource*: _alicloud_dns_records_([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
- resource/instance: add new parameter `role_name`([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
- resource/slb: remove slb schema field `listeners` and using new listener resource to replace([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- resource/ess_scaling_configuration: add new parameters `key_name`, `role_name`, `user_data`, `force_delete` and `tags`([#54](https://github.com/aliyun/terraform-provider-alicloud/pull/54))
- resource/ess_scaling_configuration: remove it importing([#54](https://github.com/aliyun/terraform-provider-alicloud/pull/54))
- resource: format not found error([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- website: improve resource docs([#56](https://github.com/aliyun/terraform-provider-alicloud/pull/56))
- examples: add new examples, like oss, key_pair, router_interface and so on([#56](https://github.com/aliyun/terraform-provider-alicloud/pull/56))

- Added support for importing:
  - `alicloud_container_cluster`([#47](https://github.com/aliyun/terraform-provider-alicloud/pull/47))
  - `alicloud_ram_policy`([#46](https://github.com/aliyun/terraform-provider-alicloud/pull/46))
  - `alicloud_ram_user`([#44](https://github.com/aliyun/terraform-provider-alicloud/pull/44))
  - `alicloud_ram_role`([#48](https://github.com/aliyun/terraform-provider-alicloud/pull/48))
  - `alicloud_ram_groups`([#49](https://github.com/aliyun/terraform-provider-alicloud/pull/49))
  - `alicloud_ram_login_profile`([#50](https://github.com/aliyun/terraform-provider-alicloud/pull/50))
  - `alicloud_dns`([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
  - `alicloud_dns_record`([#51](https://github.com/aliyun/terraform-provider-alicloud/pull/51))
  - `alicloud_slb_listener`([#53](https://github.com/aliyun/terraform-provider-alicloud/pull/53))
  - `alicloud_security_group`([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
  - `alicloud_slb`([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
  - `alicloud_vswitch`([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
  - `alicloud_vroute_entry`([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))

BUG FIXES:

- resource/vroute_entry: Fix building route_entry concurrency issue([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- resource/vswitch: Fix building vswitch concurrency issue([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- resource/router_interface: Fix building router interface concurrency issue([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- resource/vpc: Fix building vpc concurrency issue([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))
- resource/slb_attachment: Fix attaching slb failed([#55](https://github.com/aliyun/terraform-provider-alicloud/pull/55))

## 0.1.1 (December 11, 2017)

IMPROVEMENTS:

- *New Resource:* _alicloud_key_pair_([#27](https://github.com/aliyun/terraform-provider-alicloud/pull/27))
- *New Resource*: _alicloud_key_pair_attachment_([#28](https://github.com/aliyun/terraform-provider-alicloud/pull/28))
- *New Resource*: _alicloud_router_interface_([#40](https://github.com/aliyun/terraform-provider-alicloud/pull/40))
- *New Resource:* _alicloud_oss_bucket_([#10](https://github.com/aliyun/terraform-provider-alicloud/pull/10))
- *New Resource*: _alicloud_oss_bucket_object_([#14](https://github.com/aliyun/terraform-provider-alicloud/pull/14))
- *New Datasource* _alicloud_key_pairs_([#30](https://github.com/aliyun/terraform-provider-alicloud/pull/30))
- *New Datasource* _alicloud_vpcs_([#34](https://github.com/aliyun/terraform-provider-alicloud/pull/34))
- *New output_file* option for data sources: export data to a specified file([#29](https://github.com/aliyun/terraform-provider-alicloud/pull/29))
- resource/instance:add new parameter `key_name`([#31](https://github.com/aliyun/terraform-provider-alicloud/pull/31))
- resource/route_entry: new nexthop type 'RouterInterface' for route entry([#41](https://github.com/aliyun/terraform-provider-alicloud/pull/41))
- resource/security_group_rule: Remove `cidr_ip` contribute "ConflictsWith"([#39](https://github.com/aliyun/terraform-provider-alicloud/pull/39))
- resource/rds: add ability to change instance password([#17](https://github.com/aliyun/terraform-provider-alicloud/pull/17))
- resource/rds: Add ability to import existing RDS resources([#16](https://github.com/aliyun/terraform-provider-alicloud/pull/16))
- datasource/alicloud_zones: Add more options for filtering([#19](https://github.com/aliyun/terraform-provider-alicloud/pull/19))
- Added support for importing:
  - `alicloud_vpc`([#32](https://github.com/aliyun/terraform-provider-alicloud/pull/32))
  - `alicloud_route_entry`([#33](https://github.com/aliyun/terraform-provider-alicloud/pull/33))
  - `alicloud_nat_gateway`([#26](https://github.com/aliyun/terraform-provider-alicloud/pull/26))
  - `alicloud_ess_schedule`([#25](https://github.com/aliyun/terraform-provider-alicloud/pull/25))
  - `alicloud_ess_scaling_group`([#24](https://github.com/aliyun/terraform-provider-alicloud/pull/24))
  - `alicloud_instance`([#23](https://github.com/aliyun/terraform-provider-alicloud/pull/23))
  - `alicloud_eip`([#22](https://github.com/aliyun/terraform-provider-alicloud/pull/22))
  - `alicloud_disk`([#21](https://github.com/aliyun/terraform-provider-alicloud/pull/21))

BUG FIXES:

- resource/disk_attachment: Fix issue attaching multiple disks and set disk_attachment's parameter 'device_name' as deprecated([#9](https://github.com/aliyun/terraform-provider-alicloud/pull/9))
- resource/rds: Fix diff error about rds security_ips([#13](https://github.com/aliyun/terraform-provider-alicloud/pull/13))
- resource/security_group_rule: Fix diff error when authorizing security group rules([#15](https://github.com/aliyun/terraform-provider-alicloud/pull/15))
- resource/security_group_rule: Fix diff bug by modifying 'DestCidrIp' to 'DestGroupId' when running read([#35](https://github.com/aliyun/terraform-provider-alicloud/pull/35))


## 0.1.0 (June 20, 2017)

NOTES:

* Same functionality as that of Terraform 0.9.8. Repacked as part of [Provider Splitout](https://www.hashicorp.com/blog/upcoming-provider-changes-in-terraform-0-10/)

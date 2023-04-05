---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "adguard_dns_config Data Source - adguard"
subcategory: ""
description: |-
  
---

# adguard_dns_config (Data Source)



## Example Usage

```terraform
# get the current DNS config
data "adguard_dns_config" "test" {
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Read-Only

- `blocking_ipv4` (String) When `blocking_mode` is set to `custom_ip`, the IPv4 address to be returned for a blocked A request
- `blocking_ipv6` (String) When `blocking_mode` is set to `custom_ip`, the IPv6 address to be returned for a blocked A request
- `blocking_mode` (String) DNS response sent when request is blocked
- `bootstrap_dns` (List of String) Booststrap DNS servers
- `cache_optimistic` (Boolean) Whether optimistic DNS caching is enabled
- `cache_size` (Number) DNS cache size (in bytes)
- `cache_ttl_max` (Number) Overridden maximum TTL received from upstream DNS servers
- `cache_ttl_min` (Number) Overridden minimum TTL received from upstream DNS servers
- `default_local_ptr_upstreams` (List of String) List of discovered private reverse DNS servers
- `disable_ipv6` (Boolean) Whether dropping of all IPv6 DNS queries is enabled
- `dnssec_enabled` (Boolean) Whether outgoing DNSSEC is enabled
- `edns_cs_enabled` (Boolean) Whether EDNS Client Subnet (ECS) is enabled
- `id` (String) Identifier attribute
- `local_ptr_upstreams` (List of String) List of private reverse DNS servers
- `rate_limit` (Number) The number of requests per second allowed per client
- `resolve_clients` (Boolean) Whether reverse DNS resolution of clients' IP addresses is enabled
- `upstream_dns` (List of String) Upstream DNS servers
- `upstream_mode` (String) Upstream DNS resolvers usage strategy
- `use_private_ptr_resolvers` (Boolean) Whether to use private reverse DNS resolvers


# arbiter

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/arbiter)
[![General Workflow](https://github.com/rolehippie/arbiter/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/arbiter/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/arbiter/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/arbiter/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/arbiter/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/arbiter/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/arbiter)](https://github.com/rolehippie/arbiter/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.arbiter-blue)](https://galaxy.ansible.com/rolehippie/arbiter)

Ansible role to install and configure an MongoDB cluster arbiter.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [arbiter_instances](#arbiter_instances)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### arbiter_instances

List of arbiter instances

#### Default value

```YAML
arbiter_instances: []
```

#### Example usage

```YAML
arbiter_instances:
  - name: foobar
    version: 4.0
    pull: True
    publish: 27017
    replset: rs0
    owner: 999
    group: root
    username: root
    password: p455w0rd
    keyfile: |
      MvQnGS/uVhaRyMn3UJpAL2NCtvw2WMFW7Ob88px2KTNP7PBJNwAJsYwW69NzLRLA
      AWXHLvboJ7DZvgVagmuvT9B8s2rRk95X0I+ET/5aFt74BFcW1Ix/NydF/PfMl1kc
      IaoLWtGD5Tv4iSuG7otlyHQgaBtfOIxbPsehIww10Y5OOMkQLsykmxJyFKPXZ3x0
      Trmha1d6wQRjnd0DpvOxFUMlWch4PXYeMEMMYWZhlBXHHkGYOCzAt+t0WMwx5ljW
      xeY5sZ/75AZLDJ7Oh1+fEAnuHNHcYPCVpD79OoEeod7PmL/wstE/9SWS5qFnIaFv
      +CrJb+zYugUCSPgRQQIEnw+daT/j7fS7+gEef8KAI6NvE4okNXsYhp54V2zmViu5
      K/IVllstrEBZha37oee3UIGBQTDxryTIF3DabZRHHFQWqYpCb8dor2nynYbdTBYA
      +UralOf8cdJUnMvkZwNd968fT6v63NtxQXulC0NBqcBP6Sl4QWKwcmztgY1q/Koo
      Mfr6YNajoDyYjDhXCrN//lFAwKcR67TLEU4GOVDaqkHesW3AOQW08bfNyZe4rwlC
      rZ2wNdjtPiZ+YSua+7dSXCvaqhipkN/5cmDja26vkEmYqoY0bXmUVYiO2hb0+67j
      LbVUOCpMHd+fp/LeuXUMamRlOcaP5VQU+G6Dd5hashOYTU/G+UjKeqoR8hJz4xJC
      M2BTI5BUm3EH+iyAqoyKPCTR12Wd4/cX66SdCoL0NeehNJ06CZhSVwJibyx7LJB1
      J3Uep58uMg49Lz3THuGrs+JRDFKmtmMvgcnk2BBqN7dEirGO7caCN+ecVmXLZCPg
      /fKDsPGmT4fjtg0BWHSbZOIyFM1MJrDEB6mInGaoVGYBZ/h1AbHuq7lcS5E9fGJY
      hQqIKl9iFPsoYpVlMF6jwFBW3vx7pPerEin77aCClTA5/skzZbk+PSRrmwJYbkxh
      QAY4HoQYCQOmBVWZgDfLv37aS23i
```

## Discovered Tags

**_arbiter_**


## Dependencies

- [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)

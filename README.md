# <a name="title"></a> golang (Chef cookbook for Go)

## <a name="description"></a> Description

Chef cookbook for [Go programming language](http://golang.org/).

## <a name="requirements"></a> Requirements

### <a name="requirements-platform"></a> Platform

* Ubuntu (10.04/11.04/12.04/13.04)
* Debian (6.0)

**Notes**: This cookbook has been tested on the listed platforms. It
may work on other platforms with or without modification. Please
[report issues](/issues) any additional platforms so they can be added.

### <a name="requirements-cookbooks"></a> Cookbooks

This cookbook depends on the following external cookbooks:

* git

## <a name="usage"></a> Usage

#### golang::default

Just include `golang` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[golang]"
  ]
}
```

## <a name="attributes"></a> Attributes

#### golang::default
<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['go']['version']</tt></td>
    <td>String</td>
    <td>Go version</td>
    <td><tt>1.0.3</tt></td>
  </tr>
  <tr>
    <td><tt>['go']['platform']</tt></td>
    <td>String</td>
    <td>`amd64` or `i386`</td>
    <td><tt>amd64</tt></td>
  </tr>
</table>

## <a name="testing"></a> Testing

This project have [foodcritic](https://github.com/acrmp/foodcritic) for syntax checking and
[test-kitchen](https://github.com/opscode/test-kitchen) for integration testing. You can run the test suite by
typing: `rake kitchen:all` (may be slow for the first time).

In order to run these tests, the following
[requirements](https://github.com/opscode/kitchen-vagrant#-requirements) must be
satisfied:

* [Vagrant](http://vagrantup.com/) (>= 1.1.0)
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant Berkshelf Plugin](http://rubygems.org/gems/vagrant-berkshelf)

## <a name="contributing"></a> Contributing

1. Fork the repository
2. Create a named feature branch (like `add_component_x`)
3. Write you change
4. Test it by running `rake kitchen:all`
5. Submit a Pull Request

## <a name="contributors"></a> Contributors

* **[@xaprb](https://github.com/xaprb)**
* **[@crowdmatt](https://github.com/crowdmatt)**
* **[@buth](https://github.com/buth)**


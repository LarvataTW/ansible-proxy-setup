# Ansible Role - proxy-setup

Configure a system to use a Proxy Server.   
Using `--skip-tags` to determine which kind of setup tasks should skip.

## Examples

```YAML
# ansible-playbook --skip-tags=apt,git,yarn,docker ...

- hosts: all
  vars:
    proxy:
      addr: my.fqdn
      port: 3128
```

## Linting

```bash
yamllint -c yamllint.yaml .
ansible-lint .
```

## License

MIT

## Original Author Information

Paul Kehle  
@pgkehle ([twitter](https://twitter.com/pgkehle), [github](https://github.com/pgkehle), [linkedin](https://www.linkedin.com/in/pgkehle))

### References

- [From Digital Drummer](http://digitaldrummerj.me/proxy-configurations/)
- [From Ask Ubuntu](http://askubuntu.com/questions/664777/systemwide-proxy-settings-in-ubuntu)
- [From Linux Secrets](http://www.linuxsecrets.com/blog/6managing-linux-systems/2015/05/26/1490-manually-change-ubuntu-proxy-settings-from-cli-command-line-terminal)

# test
...
- name: "NGINX test result"
  debug: 
    msg: "NGINX found"
  when: "'nginx' in ansible_facts.packages"

- name: "NGINX test result"
  debug: 
    msg: "NGINX NOT found"
  when: "'nginx' not in ansible_facts.packages"

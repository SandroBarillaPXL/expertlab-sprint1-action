# expertlab-sprint1-action
This repository serves as a PoC of a custom GitHub Action

## Usage
```yaml
- name: run own action
  id: run-own
  uses: SandroBarillaPXL/expertlab-sprint1-action@v1.2.1
  with:
    input1: "ik geef een input1"
    input2: "deze input is niet verplicht maar ik doe het toch"

- name: use action output
  run: echo "The output of my action is ${{ steps.run-own.outputs.output1 }}"
```	            
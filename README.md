# burgos-documents
#### Hooks for validating CPF and CNPJ documents

##### useValidateCPF
returns a method that receives a string as parameter and returns the boolean validation of this CPF.

```jsx
import { useValidateCPF } from 'burgos-documents'

export const App = () => {
    const validateCPF = useValidateCPF()
    const cpf = '12345678901'

    console.log(validateCPF(cpf)) ## false
}
```

##### useValidateCNPJ
returns a method that receives a string, number or array of digits as parameter and returns the boolean validation of this CNPJ.

```jsx
import { useValidateCNPJ } from 'burgos-documents'

export const App = () => {
    const validateCNPJ = useValidateCNPJ()
    const cnpj = '12345678901234'

    console.log(validateCNPJ(cnpj)) ## false
}
```

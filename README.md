
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/money-manager-sm-output-v2.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/money-manager-lg-output.png)



### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- Initially, Balance Amount, Income Amount, and Expenses Amount should be `0`
- Balance Amount should be calculated by removing the Expenses Amount from the Income Amount in the list of transactions
- Income Amount should be calculated by removing the Expenses Amount in the list of transactions
- Expenses Amount should be calculated by adding only Expenses Amount in the list of transactions
- The `MoneyManager` component is provided with `transactionTypeOptions`. It consists of a list of transaction type objects with the following properties in each object

  |     Key     | Data Type |
  | :---------: | :-------: |
  |  optionId   |  String   |
  | displayText |  String   |

- Initially, the value of the `titleInput` should be empty
- Initially, the value of the `amountInput` should be empty
- Initially, the first option in the list should be selected
- When a transaction is added, by providing the values in the `titleInput`, `amountInput` and `optionId` and **Add** button is clicked,

  - A new transaction should be added to the transaction history list
  - `totalBalance`, `totalIncome` and `totalExpenses` should be updated accordingly

    ```
    totalBalance = totalIncome - totalExpenses
    ```

  - After updating, the values in the `titleInput`,`amountInput` and `optionId` will be updated to their initial values

- When the delete button in the transaction history is clicked,
  - The respective transaction should be deleted from the transaction history list
  - `totalBalance`, `totalIncome` and `totalExpenses` should be updated accordingly

</details>


<details>
<summary>Implementation Files</summary>
<br/>

Used these files to complete the implementation:

- `src/App.js`
- `src/components/MoneyManager/index.js`
- `src/components/MoneyManager/index.css`
- `src/components/MoneyDetails/index.js`
- `src/components/MoneyDetails/index.css`
- `src/components/TransactionItem/index.js`
- `src/components/TransactionItem/index.css`
</details>

<details>
<summary>Image URLs</summary>

- [https://assets.ccbp.in/frontend/react-js/money-manager/money-manager-bg.png](https://assets.ccbp.in/frontend/react-js/money-manager/money-manager-bg.png)
- [https://assets.ccbp.in/frontend/react-js/money-manager/balance-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/balance-image.png) alt should be **balance**
- [https://assets.ccbp.in/frontend/react-js/money-manager/income-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/income-image.png) alt should be **income**
- [https://assets.ccbp.in/frontend/react-js/money-manager/expenses-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/expenses-image.png) alt should be **expenses**
- [https://assets.ccbp.in/frontend/react-js/money-manager/delete.png](https://assets.ccbp.in/frontend/react-js/money-manager/delete.png) alt should be **delete**

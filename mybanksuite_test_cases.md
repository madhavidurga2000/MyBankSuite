# MyBankSuite - Java Swing Banking App: Test Cases

| Test ID     | Module        | Test Description                 | Input                                   | Expected Result                          | Status |
|-------------|---------------|----------------------------------|-----------------------------------------|-------------------------------------------|--------|
| TC-MB-01    | Login         | Valid user login                 | User ID: `1001`, PIN: `1234`            | Redirect to dashboard                     | ✅     |
| TC-MB-02    | Login         | Invalid credentials              | User ID: `0000`, PIN: `abcd`            | Show error message                        | ✅     |
| TC-MB-03    | Transaction   | Deposit money                    | Amount: ₹1000                           | Balance updated                           | ✅     |
| TC-MB-04    | Transaction   | Withdraw money (sufficient funds)| Amount: ₹500                            | Balance deducted                          | ✅     |
| TC-MB-05    | Transaction   | Withdraw money (low balance)     | Amount: ₹10,000, Balance: ₹5000         | Show "Insufficient Balance" error         | ✅     |
| TC-MB-06    | Settings      | Change PIN                       | Old PIN: `1234`, New PIN: `5678`        | PIN updated message shown                 | ✅     |
| TC-MB-07    | Logout        | Logout from app                  | Click "Logout"                          | Return to login screen                    | ✅     |

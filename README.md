# dropzone
dropzone is a backend service that allows users to upload files or folders to AWS S3 using any desired storage class tier. Whether you're uploading hot data, archival content, or backups, this service supports:

Whether you're uploading hot data, archival content, or backups, this service supports:
✅ Direct file & folder uploads
✅ Choice of S3 storage class: Standard, IA, Glacier, and more
✅ Fine-grained cost control via tier selection
✅ Easy integration with any frontend or CLI

**💰 AWS S3 Storage Class Comparison
**
| Storage Class                  | Use Case                        | Durability            | Availability | Retrieval Time | Cost per GB (approx)\*   |
| ------------------------------ | ------------------------------- | --------------------- | ------------ | -------------- | ------------------------ |
| **Standard**                   | Frequent access                 | 99.999999999% (11 9s) | 99.99%       | Milliseconds   | \~\$0.023                |
| **Intelligent-Tiering**        | Unknown/variable access pattern | 99.999999999%         | 99.9–99.99%  | Milliseconds   | \~\$0.023 (auto adjusts) |
| **Standard-IA**                | Infrequent access               | 99.999999999%         | 99.9%        | Milliseconds   | \~\$0.0125               |
| **One Zone-IA**                | Infrequent, non-critical        | 99.999999999%         | 99.5%        | Milliseconds   | \~\$0.01                 |
| **Glacier Instant Retrieval**  | Archive, but fast access        | 99.999999999%         | 99.9%        | Milliseconds   | \~\$0.004                |
| **Glacier Flexible Retrieval** | Archive, less frequent          | 99.999999999%         | 99.9%        | Minutes–Hours  | \~\$0.0038               |
| **Glacier Deep Archive**       | Long-term archive (years)       | 99.999999999%         | 99.9%        | \~12 hours     | \~\$0.00099              |


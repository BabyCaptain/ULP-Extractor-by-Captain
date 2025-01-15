# ULP-Extractor-by-Captain
ULP Extractor by Captain


The **ULP Extractor by Captain** is a tool designed to extract credentials (such as emails and passwords) from text files, typically used for extracting account information that is in a specific format. The tool is likely aimed at processing text files, which could contain data like login credentials, and organizing or filtering them based on certain domains.

Here's a breakdown of what the tool does:

### Key Features:
1. **Folder and Domain Selection**:
   - The user selects a folder that contains `.txt` files (which presumably have credentials in them).
   - The user can specify a list of **domains** (such as `example.com, example2.com`) that the tool will focus on while extracting the credentials.

2. **Credential Extraction**:
   - The tool extracts credentials from the text files based on specific patterns (like URLs, emails, and passwords).
   - These credentials are extracted if the domain from the extracted URL matches one of the user-provided domains.

3. **Log and Stats**:
   - The tool maintains logs and displays information about the extraction process, such as how many files were processed, how many credentials were found, and if there were any errors.
   - A "Password Found" count is updated in real time, and the tool logs success or failure messages.

4. **Handling of Duplicates**:
   - After the extraction, the tool offers a **Duplicate Cleaner** feature to remove duplicate credentials that may exist within the result files.

5. **Exporting Results**:
   - The extracted credentials are saved into separate text files for each domain. For example, credentials found for `example.com` will be saved in a `example.com.txt` file.

6. **Stopping and Exiting**:
   - The user can stop the extraction process at any time, and the tool ensures to stop any ongoing operations.
   - The user can also exit the application with a confirmation prompt.

7. **Graphical User Interface (GUI)**:
   - The tool is built using **PyQt6**, which means it comes with a GUI that allows users to interact with the application through forms, buttons, and logs.
   - The user can browse for the folder where `.txt` files are stored and view detailed logs on the extraction process.

### How It Works:
1. The user starts by selecting the folder containing `.txt` files and specifying the domains they want to extract credentials from.
2. The tool scans the `.txt` files, searches for matching patterns (URL, email, password), and extracts the relevant credentials if they match the specified domains.
3. It then stores the results in new text files named according to the domain (e.g., `example.com.txt`).
4. The tool also offers a feature to clean duplicate credentials from the result files.
5. Users can stop the extraction anytime and get a summary of the results.

### Intended Use:
The tool is likely useful for someone needing to extract, organize, and clean credentials from various text sources, perhaps for security or auditing purposes. It might be used in scenarios where large sets of credentials are stored in multiple `.txt` files, and the user needs to quickly filter and clean the data based on specific domains.

### The "Captain" Branding:
The **"by Captain"** part of the name is likely a personal or branding reference. It could imply that the creator or developer of the tool goes by the name "Captain" or has given the tool that name as a way to brand it for distribution.

### Caution:
While the tool has legitimate uses, extracting and handling credentials requires caution. Users should ensure they have explicit permission to handle the data they are processing, as extracting login information from unauthorized sources can lead to legal and ethical issues.

In short, **ULP Extractor by Captain** is a **credentials extraction and cleaning tool** designed to help users efficiently process `.txt` files containing login information, filter them based on domain, and remove duplicates. It is packaged with a simple and user-friendly interface to guide users through the extraction process.

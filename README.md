# ASP-CLIENT-SERVER-FINAL
Client Server Mini Bash Application for Linux coded in C

Project Title: File Transfer System with Server-Mirror Architecture

Description:
This client-server project allows clients to request files from a server. The server searches its directory for files and returns them in tar.gz format. Multiple clients can connect from different machines using sockets. Key features include:

Server and mirror processes run on separate machines.
Clients request files using custom commands.
Server forks a child process for each client request.
Clients verify command syntax before sending them to the server.
List of supported client commands includes file retrieval, file search, and more.
Server alternates between handling client connections and mirroring them.
Client Commands:

fgets file1 file2 file3 file4: Retrieve files if found.
tarfgetz size1 size2 <-u>: Retrieve files within a size range.
filesrch filename: Search for files by name.
targzf <extension list> <-u>: Retrieve files by extension.
getdirf date1 date2 <-u>: Retrieve files by creation date range.
quit: Terminate the client process.

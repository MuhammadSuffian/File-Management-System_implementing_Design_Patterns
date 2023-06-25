Project Description
This project is a file management system implemented in Java, showcasing the usage of three design patterns: Composite, Command, and Decorator. The system provides functionality for creating directories and files, executing commands such as copying/moving files, and adding additional features through decorators.

Design Patterns
1. Composite Pattern
The Composite pattern is utilized to represent directories and files in a hierarchical structure. The Composite class serves as the base class for both directories and files. It provides methods for adding and removing child components, retrieving child components, and listing the components. The Directorycompositive and Filecomposite classes extend the Composite class to represent directories and files, respectively. The DirectoryIterator class implements the Iterator interface to traverse and iterate over the components within the composite structure.

2. Command Pattern
The Command pattern is employed to encapsulate different operations as commands. The Command interface defines the execute method, which is implemented by various command classes such as CreateFileCommand, CreateDirectoryCommand, CopyFileCommand, and MoveFileCommand. Each command encapsulates a specific operation, such as creating files or directories, copying/moving files. The Main class demonstrates the usage of these commands by executing them and performing corresponding operations on the file management system.

3. Decorator Pattern
The Decorator pattern is applied to add additional functionalities to files and directories. The Decorator class extends the Composite class and wraps a component to enhance its behavior. In this project, decorators such as CompressionDecorator and EncryptionDecorator are implemented to provide compression and encryption functionalities to files and directories, respectively. These decorators override the list method to add the additional functionality and then invoke the list method of the wrapped component.

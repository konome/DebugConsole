# Debug Console
Attach a console window to a .NET project for debugging purposes. Useful while developing GUI projects such as WinForms and WPF.

## Sample
```csharp
internal static class Program
{
    /// <summary>
    ///  The main entry point for the application.
    /// </summary>
    [STAThread]
    static void Main()
    {
        // Attach console window for debugging purpose.
        DebugConsole.Create(0, 0, 620, 240);
        
        ApplicationConfiguration.Initialize();
        Application.Run(new Form1());
    }
}
```

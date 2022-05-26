# DebugConsole
Attach a console window to a .NET project for debugging purposes. Useful for GUI projects such as WinForms and WPF.

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
        Debug.Writeline("Debugging...")
        
        ApplicationConfiguration.Initialize();
        Application.Run(new Form1());
    }
}
```
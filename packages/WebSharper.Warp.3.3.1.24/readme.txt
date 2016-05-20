To use Warp from an F# script, add the following lines at the top of your file:

    #I "packages/Owin.1.0/lib/net40"
    #I "packages/Microsoft.Owin.3.0.1/lib/net45"
    #I "packages/Microsoft.Owin.Host.HttpListener.3.0.1/lib/net45"
    #I "packages/Microsoft.Owin.Hosting.3.0.1/lib/net45"
    #I "packages/Microsoft.Owin.FileSystems.3.0.1/lib/net45"
    #I "packages/Microsoft.Owin.StaticFiles.3.0.1/lib/net45"
    #I "packages/WebSharper.3.3.1.177/lib/net40"
    #I "packages/WebSharper.Compiler.3.3.1.177/lib/net40"
    #I "packages/WebSharper.Owin.3.3.1.93/lib/net45"
    #load "packages/WebSharper.Warp.3.3.1.24/tools/reference.fsx"

If you install NuGet packages without version number in the path
(for example if you use Paket), then you can simply add this instead:

    #load "packages/WebSharper.Warp/tools/reference-nover.fsx"

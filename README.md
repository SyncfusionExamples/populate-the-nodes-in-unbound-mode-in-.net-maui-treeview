# populate-the-nodes-in-unbound-mode-in-.net-maui-treeview

This repository demonstrates how to manually add and manage nodes in unbound mode using the .NET MAUI TreeView (SfTreeView) control. It provides a sample implementation that shows how to define the tree structure directly in XAML without data binding, enabling flexible and straightforward creation of hierarchical views.


## Sample

### XAML

```xaml
<ContentPage.Content>
    <syncfusion:SfTreeView x:Name="treeView" ExpandActionTarget="Node" FullRowSelect="True">
        <syncfusion:SfTreeView.Nodes>
            <treeviewengine:TreeViewNode Content="Australia" IsExpanded="True">
                <treeviewengine:TreeViewNode.ChildNodes>
                    <treeviewengine:TreeViewNode Content="New South Wales" IsExpanded="True">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="Sydney" IsExpanded="True"/>
                            <treeviewengine:TreeViewNode Content="Canberra" IsExpanded="True"/>
                            <treeviewengine:TreeViewNode Content="Newcastle–Maitland" IsExpanded="True"/>
                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                    <treeviewengine:TreeViewNode Content="Victoria" IsExpanded="True">
                        <treeviewengine:TreeViewNode.ChildNodes>
                            <treeviewengine:TreeViewNode Content="Melbourne" IsExpanded="True"/>
                        </treeviewengine:TreeViewNode.ChildNodes>
                    </treeviewengine:TreeViewNode>
                </treeviewengine:TreeViewNode.ChildNodes>
            </treeviewengine:TreeViewNode>
        </syncfusion:SfTreeView.Nodes>
    </syncfusion:SfTreeView>
</ContentPage.Content>
```

## Requirements to run the demo

To run the demo, refer to [System Requirements for .NET MAUI](https://help.syncfusion.com/maui/system-requirements).

Make sure that you have the compatible versions of [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/ ) with the Dot NET MAUI workload and [.NET Core SDK 7.0](https://dotnet.microsoft.com/en-us/download/dotnet/7.0) or later version in your machine before starting to work on this project.

## Troubleshooting:
### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

## License

Syncfusion® has no liability for any damage or consequence that may arise from using or viewing the samples. The samples are for demonstrative purposes. If you choose to use or access the samples, you agree to not hold Syncfusion® liable, in any form, for any damage related to use, for accessing, or viewing the samples. By accessing, viewing, or seeing the samples, you acknowledge and agree Syncfusion®'s samples will not allow you seek injunctive relief in any form for any claim related to the sample. If you do not agree to this, do not view, access, utilize, or otherwise do anything with Syncfusion®'s samples.

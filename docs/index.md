using Hkmp.Api.Client;

namespace ExampleAddon {
    public class ExampleClientAddon : ClientAddon {
        public override void Initialize(IClientApi clientApi) {
            Logger.Info("Initializing client-side example addon!");
        }

        protected override string Name => "ExampleAddon";
        protected override string Version => "0.0.1";
        public override bool NeedsNetwork => true;
    }
}


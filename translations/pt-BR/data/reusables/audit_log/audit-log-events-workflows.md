| Ação | Descrição |
| ---- | --------- |
|      |           |
{%- ifversion fpt or ghes > 3.1 or ghae or ghec %}
| `workflows.approve_workflow_job` | A workflow job was approved. Para obter mais informações, consulte "[Revisando implantações](/actions/managing-workflow-runs/reviewing-deployments)." | `workflows.cancel_workflow_run` | A workflow run was cancelled. Para obter mais informações, consulte "[Cancelar um fluxo de trabalho](/actions/managing-workflow-runs/canceling-a-workflow)". | `workflows.delete_workflow_run` | A workflow run was deleted. Para obter mais informações, consulte "[Excluir uma execução de fluxo de trabalho](/actions/managing-workflow-runs/deleting-a-workflow-run)". | `workflows.disable_workflow` | A workflow was disabled. | `workflows.enable_workflow` | A workflow was enabled, after previously being disabled by `disable_workflow`. | `workflows.reject_workflow_job` | A workflow job was rejected. Para obter mais informações, consulte "[Revisando implantações](/actions/managing-workflow-runs/reviewing-deployments)." | `workflows.rerun_workflow_run` | A workflow run was re-run. Para obter mais informações, consulte "[Executar novamente um fluxo de trabalho](/actions/managing-workflow-runs/re-running-a-workflow)".
{%- endif %}
{%- ifversion fpt or ghec or ghes > 3.2 or ghae-issue-4963 %}
| `workflows.completed_workflow_run` | A workflow status changed to `completed`. Só pode ser visto usando a API REST; não visível na interface do usuário ou na exportação do JSON/CSV. For more information, see "[Viewing workflow run history](/actions/managing-workflow-runs/viewing-workflow-run-history). | `workflows.created_workflow_run` | A workflow run was created. Só pode ser visto usando a API REST; não visível na interface do usuário ou na exportação do JSON/CSV. Para obter mais informações, consulte "[Criar um exemplo de fluxo de trabalho](/actions/learn-github-actions/introduction-to-github-actions#create-an-example-workflow)". | `workflows.prepared_workflow_job` | A workflow job was started. Inclui a lista de segredos que foram fornecidos ao trabalho. Só pode ser visto usando a API REST. Não é visível na interface da web de {% data variables.product.prodname_dotcom %} ou incluído na exportação do JSON/CSV. Para obter mais informações, consulte "[Eventos que acionam fluxos de trabalho](/actions/reference/events-that-trigger-workflows)".
{%- endif %}